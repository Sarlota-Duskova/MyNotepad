# PowerShell



https://learn.microsoft.com/en-us/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands?view=powershell-7

`Get-Help Command-Name -examples`

### Basic commands

`Start-Process notepad.exe`

* To start a process.

`Get-Content`

* Similar to `cat` on Linux.
* `type` on the Windows command-line.

`Get-Process`

* Get-Process is useful to list all running processes.
* It can also be used with the “-name” parameter to filter for a specific process name.

Files can be copied and moved with `Copy-Item` and `Move-Item`.

#### Object Manipulation

* The Pipeline(|) is used to pass output from one cmdlet to another.
* Powershell passes an object to the next cmdlet.
* Object has **Properties** and **Method (Function)**

`Verb-Noun | Get-Member`

`Get-Command | Get-Member -MemberType Method`

#### Creating Objects From Previous cmdlets

`Get-ChildItem | Select-Object -Property Mode, Name`

**Following flags to select particular information:**

* `first` - gets the first x object
* `last` - gets the last x object
* `unique` - shows the unique objects
* `skip` - skips x objects

#### Filtering Objects

`Verb-Noun | Where-Object -Property PropertyName -operator Value`

`Verb-Noun | Where-Object {$_.PropertyName -operator Value}`

* The `$_ operator` to iterate through every object passed to the Where-Object cmdlet.

#### Sort Object

`Verb-Noun | Sort-Object`

**Find File:** `Get-ChildItem -Path C:\ -Include *interesting-file.txt* -File -Recurse`

* `-Recurse` for loking in subdirectories

**Read File:**

`Get-Content "C:\Program Files\interesting-text.txt.txt"`

**Find how many cmdlet are installed on system:**

`Get-Command | where-object -Property CommandType -eq Cmdlet | measure`

**MD5 hash of interesting-file.txt:**

`Get-FileHash -Path "C:\Program Files\interesting-text.txt.txt" -Algorithm MD5`

**Get the current working directory:**

`Get-Location`

**Request to a web server:**

`Invoke-WebRequest`

**Decode Base64 file:**

* `$file = "C:\Program Files\interesting-text.txt.txt"`
* `$data = Get-Content $file`
* `[System.Text.Encoding]::ASCII.GetString([System.Convert]::FromBase64String($data)) > decb64.txt`

**How many users are on the machine:**

`Get-LocalUser` `Get-LocalUser -SID <number>`

**Users have their password required values set to False:**

`Get-LocalUser | where-object -Property PasswordRequired -Match false`

**How many local groups exist:**

`Get-LocalGroup | measure`

**Get the IP address info:**

`Get-NetIPAddress`

**Ports are listed as listening:**

`Get-NetTCPConnection | where-object -Property State -eq Listen | measure`

**How many patches have been applied:**

`Get-Hotfix | measure`

**When was the patch with ID KB4023834 installed:**

`Get-Hotfix | where-object -property HotfixID -eq KB4023834`

**Search for all files containing API\_KEY:**

`Get-ChildItem -Path C:\ -recurse | Select-String -pattern API_KEY`

**List all the running processes:**

`Get-Process`

**The path of the scheduled task called new-sched-task:**

`Get-ScheduledTask | where-object -property TaskName -eq new-sched-task`

**Owner of the C:/**

`Get-Acl C:\`

### PowerView

* PowerView is one of the most effective ways to gather information on the domain.
* The module can be downloaded from: https://github.com/PowerShellMafia/PowerSploit/blob/dev/Recon/PowerView.ps1
