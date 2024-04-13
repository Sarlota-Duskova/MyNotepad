# Questions

1.  You are writing a shell script using Bash and need to print the contents of a variable. Which of the following commands can be used to do so?

    1. `echo`
    2. `lf`
    3. `sp`
    4. `varpt`

    Answer:

    A.  The `echo` command is used to send output from a Bash script. The other options are not valid commands.
2.  Which of the following packages provides orchestration for Linux in an agentless manner?

    1. Ansible
    2. Puppet
    3. Automat
    4. vid

    Answer:

    A.  Ansible is agentless, using SSH and Python for orchestration. Puppet does have an agentless mode but typically uses agents for orchestration. The others are not valid orchestration packages.
3.  Which of the following commands can be used to execute a command with a customized environment?

    1. `set`
    2. `env`
    3. `run`
    4. `crun`

    Answer:

    B.  The `env` command executes a command and enables a custom environment for that command execution. The `set` command changes environment variables but does not change variables for the single command execution, as specified in the scenario. The other options are not valid commands.
4.  Which of the following commands, when used with `git`, retrieves the latest objects from a repository and attempts to incorporate those changes into the local working copy of the repository?

    1. `fetch`
    2. `pull`
    3. `retr`
    4. `get`

    Answer:

    B.  The `pull` command in git fetches the changes and incorporates them into the current working copy. The `fetch` command retrieves but does not incorporate the changes. The other options are not valid `git` subcommands.
5.  Which of the following best describes the concept of infrastructure as code?

    1. The management of switches and routers using compiled programs
    2. The management of servers and other systems using scripting, source code management, and automation
    3. The deployment of hardware using Agile methodologies
    4. Planning for bugs in infrastructure code and allowing time to fix them

    Answer:

    B.  Infrastructure as code typically means managing infrastructure components using some of the same tools that developers would use, such as source code management along with programs or scripts and automation for deployments and configuration changes. These practices help to facilitate continuous integration/continuous deployment (CI/CD) scenarios by automating many processes.
6.  Which of the following commands changes a file called `script.sh`, which is located in your home directory, such that it can be executed by the owner of the file and no one else?

    1. `chmod 700 ~/script.sh`
    2. `chown +x /script.sh`
    3. `chmod` \~/`script.sh +x`
    4. `chmod 777 /home/script.sh`

    Answer:

    A.  The `chmod` command will be used for this solution. The option granting 700 enables execute privileges for the owner. The other options have incorrect syntax, an incorrect path, or inappropriate permissions for the scenario described. It is important to differentiate between relative and absolute paths, noting that `~/` is an alias for your home directory.
7.  Which command can be used to add functions and variables to the current shell?

    1. `source`
    2. `echo`
    3. `en`
    4. `src`

    Answer:

    A.  The `source` command adds functions found in the file argument to the current shell. The `source` command is frequently used for software installs to ensure that the environment is set up properly prior to execution of the install scripts.
8.  Which of the following is the correct method for invoking the Bash shell for a script, typically found as the first line of the script?

    1. `#!/BASH`
    2. `#!bash`
    3. `#!/bash`
    4. `#!/bin/bash`

    Answer:

    D.  The character sequence `#!/bin/bash` invokes the commands that follow as a Bash script.
9.  You need to send output from a command to a log file. Overwriting the contents of the log file is acceptable. Which of the following characters is used to redirect output in such a way as to fulfill this scenario?

    1. `|`
    2. `<`
    3. `>`
    4. `&`

    Answer:

    C.  The greater-than sign is used to redirect output to a file and will overwrite the file if it already exists. The pipe character can be used to chain output but is not considered redirection of output. The less-than sign will redirect input and the ampersand will send a process into the background.
10. You need to create a new empty git repository called `repo`. Which of the following sequences accomplishes this task?

    1. `mkdir repo`; `cd repo`; `git init --bare`
    2. `mkdir repo`; `git init repo/`
    3. `git init repo –md`
    4. `git create repo/`

    Answer:

    A.  Creating a git repository requires creating the directory, changing the current working directory to the new directory, and then running `git init --bare`. The other commands will not create an empty git repository.
11. Which of the following terms is used in orchestration and automation scenarios to refer to the collection of devices being managed?

    1. Device collection
    2. Inventory
    3. Machines
    4. UsableObjects

    Answer:

    B.  The term _inventory_ is most often used in orchestration to refer to the collection of devices under management.
12. You need to print output from a Bash script such that single quotes appear in the outputted string. Which character should be used as an escape sequence in order to get the single quotes into the output?

    1. `/`
    2. `'`
    3. `?`
    4. `\`

    Answer:

    D.  A backslash is used to escape characters such as a single quote in a Bash script. The other characters will not achieve the desired result.
13. Which exit code indicates success for a Bash script?

    1. 0
    2. 1
    3. 2
    4. EOF

    Answer:

    A.  An exit code of 0 indicates that the script did not encounter an error. This exit code is generally associated with a successful execution of a program in Linux.
14. Which of the following commands produces output `sit sat set?`

    1. `echo s{i,a,e}t`
    2. `echo s(i,a,e)t`
    3. `echo s[i,a,e]t`
    4. `echo s/i,a,e/t`

    Answer:

    A.  Shell expansion, or more accurately, brace expansion, can be used to create the output shown. The other options will not produce output as shown.
15. Which of the following characters or character sequences begins a comment in a Bash script?

    1. `/*`
    2. `//`
    3. `#`
    4. `'`

    Answer:

    C.  The pound sign (`#`) is used to indicate that what follows is a comment and will not be executed for the remainder of the line. The other options are valid comment styles in other languages but not for a Bash script.
16. Which, if any, file extension is required in order for a Bash script to execute?

    1. `.sh`
    2. `.bash`
    3. `.bat`
    4. No special extension is necessary.

    Answer:

    D.  No special extension is necessary for a Bash script to be executed. The extension `.sh` shown as an option is a common extension that you will see for shell scripts of any variety, but the extension isn't required.
17. After fetching changes for a previously cloned git repository, which git command is used to incorporate the changes from that branch into the local copy?

    1. `put`
    2. `push`
    3. `merge`
    4. `inc`

    Answer:

    C.  The `merge` command incorporates changes to a previously cloned git repository. The `push` command is valid but is used to send code to a remote repository or origin. The other commands are not valid.
18. Which of the following best describes the role of an agent in software orchestration?

    1. An agent is software that listens for and executes commands from the server.
    2. An agent is used to migrate from one operating system to another.
    3. An agent is a hardware-based token used for authentication.
    4. An agent is not used in software orchestration.

    Answer:

    A.  An agent is software that runs on clients and listens for commands from the server in an orchestration architecture.
19. Being able to deploy additional servers in response to high demand or load is an example of which type of automation?

    1. Build
    2. Compile
    3. Infrastructure
    4. Config

    Answer:

    C.  _Infrastructure automation_ is the term most closely associated with adding (and removing) servers in response to load and demand and is frequently associated with continuous integration/continuous deployment (CI/CD) concepts.
20. Which command can be used to indicate a local variable within a Bash script?

    1. `localvar`
    2. `ll`
    3. `local`
    4. `%local%`

    Answer:

    C.  When executed as part of a function, the `local` command can be used to create a local variable in a Bash script.
21. Which git command is used to retrieve a repository from a remote server?

    1. `clone`
    2. `checkout`
    3. `co`
    4. `retr`

    Answer:

    A.  The `clone` command retrieves a copy of the repository for local use. The `checkout` and `co` commands are used with Subversion and not with git.
22. You need to echo the name of the script back to the user for usage or help output. Which positional parameter can be used for this purpose?

    1. `$me`
    2. `$1`
    3. `$myname`
    4. `$0`

    Answer:

    D.  The `$0` parameter contains the name of the script being called. The other answers do not fulfill the requirements of this scenario.
23. Which of the following commands can be used to print the contents of the current shell environment?

    1. `echoenv`
    2. `printenv`
    3. `showenv`
    4. `envvar`

    Answer:

    B.  The `printenv` command can be used to print the contents of the current shell environment such as environment variables. Within the output you'll find things like the `$SHELL` variable, which specifies the current shell. The other options shown are not valid commands.
24. You are writing a `while` loop in a Bash script and need to compare two string values. Which operator is used for this purpose?

    1. `-ne`
    2. `=`
    3. `equal`
    4. `eq`

    Answer:

    B.  A single equal sign is used for string comparison in a Bash script. Of the other answers, `-ne` is valid but is used when comparing integers. The string _eq_ would be an operator if preceded by a single dash, as in `-eq`. In that case, `-eq` is used for integer comparison.
25. You need to create a Bash script that will loop continually and perform some commands within the loop. Which of the following lines will accomplish this task?

    1. `if [ $exit -eq “exit” ]`
    2. `while true; do`
    3. `for ($i = 0, $i++)`
    4. `continue until ($exit)`

    Answer:

    B.  A `while` loop that evaluates boolean `true` will accomplish the task described. The other options given are syntactically incorrect in various ways.
26. Which of the following commands changes the location to which `HEAD` is pointing with git?

    1. `git point`
    2. `git checkout`
    3. `git change`
    4. `git load`

    Answer:

    B.  The `git checkout` command switches the working copy to the specified branch and points the `HEAD` toward that branch. The other commands shown as options are not valid with git.
27. You need to declare a variable as part of the environment prior to running a Bash script. Which of the following commands accomplishes this?

    1. `dec`
    2. `create`
    3. `export`
    4. `get`

    Answer:

    C.  The `export` command adds a variable to the current environment and is frequently used for the scenario described. The other options are not valid commands.
28. Which of the following commands displays the contents of the `PATH` variable in Bash?

    1. `echo PATH`
    2. `echo` $`PATH`
    3. `echo $CURPATH`
    4. `ext $PATH`

    Answer:

    B.  The current contents of the `PATH` variable, or any other shell environment variable, can be displayed using the `echo` command. Variables in Bash use a `$` as part of the identifier. Therefore, any option without the `$` would not work.
29. Which character sequence is used to execute a command within a subshell in a Bash script?

    1. `$()`
    2. `subs()`
    3. `$%`
    4. `$(~`

    Answer:

    A.  The `$()` sequence executes a command within a subshell, which is helpful for ensuring that global variables in a Bash script cannot be modified. The other sequences shown are not valid for the scenario described.
30. You need to make a change to the configuration of the SSH daemon across your infrastructure. Being able to do so from a central server is an example of which type of automation?

    1. Security
    2. Automated configuration management
    3. Development configuration management
    4. Usability management

    Answer:

    B.  Managing configuration with orchestration is described in this scenario, so option B is the closest response.
31. Which option is used with the `env` command in order to remove a variable from the environment?

    1. `-r`
    2. `-u`
    3. `-n`
    4. `-d`

    Answer:

    B.  The `-u` option or `--unset` will remove a variable from the environment. The other options are not valid with the `env` command.
32. Within a Bash script, you need to run two commands but only run the second command if the first succeeds. Which of the following metacharacters can be used to accomplish this task?

    1. `<>`
    2. `&`
    3. `& &`
    4. `|`

    Answer:

    C.  The double-ampersand metacharacter executes the right-hand command only if the first command exits with a successful exit code. A single ampersand sends the command into the background, thus making option B incorrect. A pipe character executes the second command but does so regardless of the success or failure of the first command, thus making option D incorrect.
33. You need to redirect the output from a command and append that output to a file. Which of the following character sequences accomplishes this task?

    1. `>`
    2. `>>`
    3. `|`
    4. `^`

    Answer:

    B.  Two greater-than signs append output to the specified destination. Option A includes only one greater-than sign, which overwrites rather than appends output. The pipe character in option C does not send output to a file, and option D does not work for the purpose described.
34. You need to obtain a directory listing of all files and directories except those that begin with the letter _p_. Which of the following commands accomplishes this task?

    1. `ls -l !p`
    2. `ls -l [!p]`
    3. `ls -l [^p]`
    4. `ls -l [^p]*`

    Answer:

    D.  File globbing is the process of expansion of special characters, which is required for this scenario. In this case, the negation character is the caret, thus making option D correct. Option C is missing the crucial globbing pattern needed for this scenario.
35. Which of the following files is used within a git repository in order to indicate files and file patterns that should not be versioned?

    1. `novers`
    2. `.gitignore`
    3. `gitignore.txt`
    4. `gitnover`

    Answer:

    B.  The `.gitignore` file is used to store files that will not be versioned.
36. You need to iterate through a directory listing and perform an operation on certain files within it. To accomplish this task, you will be using a Bash script and a looping construct. Which looping construct is most appropriate for this purpose?

    1. `until`
    2. `do`
    3. `for`
    4. `foreach`

    Answer:

    C.  The `for` loop should be used for this purpose because it iterates through a list. An `until` loop would require additional code, thus making it a less-preferable construct for the purpose described. There is no `do` loop or `foreach` loop in Bash, thus making those options incorrect.
37. You are debugging a Bash script written by a different system administrator. Within the script, you see a command surrounded by backquotes, or `‘`. What will be the result of surrounding the command with backquotes?

    1. The command will execute and send all output to the console.
    2. The command will not execute.
    3. The command will execute as if the `$()` command substitution was used.
    4. The command will execute and send all output to `/dev/null`.

    Answer:

    C.  Command substitution can be accomplished using backquotes or `$()`. These two methods are substantially but not completely equivalent.
38. Which `git` command displays a short history of commits along with the commit ID?

    1. `showhist`
    2. `list`
    3. `log`
    4. `hist`

    Answer:

    C.  The `git log` command is used to show a commit history. The other commands shown are not valid with `git`.
39. You are committing code to a git repository and need to include a message on the command line. Which option enables this behavior?

    1. `-m`
    2. `-h`
    3. `-f`
    4. `-l`

    Answer:

    A.  The `-m` option enables a message to be included in the commit, thereby alleviating the need to go into an editor to create the commit message. The other options shown do not accomplish the required task.
40. Compiling software when a developer commits code to a certain branch in a repository is an example of which type of automation?

    1. Infrastructure
    2. Build
    3. Complex
    4. DevOps

    Answer:

    B.  Build automation is the most appropriate name for kicking off the compilation of software on commit and is frequently found in organizations that use continuous integration/continuous deployment (CI/CD).
41. You are working with a MySQL database and need to read in several SQL commands from a file and send them into the MySQL CLI for execution. You will be using `STDIN` redirection for this. Which of the following commands is correct, assuming a filename of `customers.sql`?

    1. `mysql < customers.sql`
    2. `mysql | customers.sql`
    3. `mysql > customers.sql`
    4. `mysql >< customers.sql`

    Answer:

    A.  In this scenario, `STDIN` redirection is accomplished with a less-than sign to take the contents of `customers.sql` and send those contents into the `mysql` command. It's also likely that the `mysql` command would have things like `-u` for the username and `-p` to prompt for the password, but those were not relevant to the scenario and are not required in all circumstances. The other options shown are not valid for the purpose described. Options B and C take output from the `mysql` command, while option D is an invalid character sequence.
42. You are collaborating on a coding project using git as the source code management tool. Teammates are saying that they cannot see your code, although you have been committing code regularly. Which of the following is most likely the problem?

    1. You have not added commit messages.
    2. You need to send the commit IDs to the teammates.
    3. You have not executed `git push` to send the code to the server.
    4. You are committing using the `-h` flag.

    Answer:

    C.  More than likely you have not executed `git push` to send the code to the server. Of the other options, you do not need to send commit IDs to teammates and there is nothing to indicate that you have been having problems committing the code itself.
43. Which option to the `chmod` command performs a recursive change?

    1. `-re`
    2. `-R`
    3. `-c`
    4. `-v`

    Answer:

    B.  The `-R` option performs a recursive change to the targets identified by the `chmod` command. The other options do not perform recursive changes for `chmod`.
44. Which character sequence is used to indicate the default case within a `case` statement in a Bash script?

    1. `()`
    2. `*.*`
    3. `**`
    4. `*)`

    Answer:

    D.  The closing parenthesis is used to denote a case; when preceded by an asterisk, the default case is indicated.
45. Which character sequence indicates the end of an `if` conditional in a Bash script?

    1. `}`
    2. `fi`
    3. `end`
    4. `endif`

    Answer:

    B.  The character sequence `fi`, which is the `if` statement backward, indicates the end of an `if` conditional within a Bash script. The other sequences shown as options may be used in other languages.
46. What is the name of the default branch in a git repository?

    1. `source`
    2. `main`
    3. `primary`
    4. `first`

    Answer:

    B.  The `main` branch is the branch created by default within a git repository. The other names shown can be used but are not the default.
47. You need to use the output from a command as input for another command. Which character facilitates this scenario?

    1. `>`
    2. `|`
    3. `!`
    4. `‘`

    Answer:

    B.  The pipe character sends, or pipes, the output from one command into another and is commonly used in a Linux environment for creating complex command sequences, whether through scripting or directly on the command line. The other options shown are not used for the purpose described in the scenario.
48. Which `git` command shows the current state of the working copy of a repository?

    1. `git list`
    2. `git status`
    3. `git state`
    4. `git view`

    Answer:

    B.  The `git status` command is used to show the current state of the working copy, displaying things like untracked files, files staged for commit, and so on. The other options shown are not valid for the scenario.
49. Which option to the `echo` command suppresses the ending newline character that is normally included?

    1. `-a`
    2. `-n`
    3. `-d`
    4. `-y`

    Answer:

    B.  The `-n` option suppresses the trailing newline character from the `echo` command and is quite useful in scripting scenarios. The other options are not valid for the command.
50. Determining the version of software installed on each client node is an example of collecting information for which collection in an automated infrastructure?

    1. Inventory
    2. Group
    3. Procedure
    4. Build

    Answer:

    A.  The inventory of an infrastructure contains things like the version of software installed on clients.
51. You need to redirect `STDERR` from a command into a file to capture the errors. Which character sequence can be used for this purpose?

    1. `>`
    2. `%2>`
    3. `2>`
    4. `%%>`

    Answer:

    C.  Redirecting `STDERR` is accomplished with the character sequence `2>`. The plain greater-than sign redirects `STDOUT`. The other character sequences shown as options are not valid for the purpose described.
52. You need to make a change to your git environment because your email address has changed. Which of the following commands ensures that your new email address will be used for all subsequent commits?

    1. `git config user.email`
    2. `git change email`
    3. `git config email.addr`
    4. `git config email.address`

    Answer:

    A.  The `git config` command will be used for this purpose, and the parameter is `user.email`.
53. Which shell built-in command is used to display a list of read-only variables?

    1. `ro`
    2. `readonly`
    3. `env-ro`
    4. `ro-env`

    Answer:

    B.  The `readonly` command displays the list of read-only variables that have been declared in the current session. The other commands listed for this question do not exist.
54. Assume that you're using the Bash shell and want to prevent output redirects from accidentally overwriting existing files. Which command and option can be used to invoke this behavior?

    1. `setoutput -f`
    2. `overwrite=no`
    3. `overwrite -n`
    4. `set -C`

    Answer:

    D.  The `set` command can be used for a variety of purposes to change how the shell environment works. One such option is `–C`, which prevents output redirection such as that done with `>` from overwriting a file if the file already exists.
55. You have received a file that does not have a file extension. Which command can you run to help determine what type of file it might be?

    1. `grep`
    2. `telnet`
    3. `file`
    4. `export`

    Answer:

    C.  The `file` command can be used to determine which type of file is being used. This can be particularly helpful for files without extensions, where you are unsure if you should view the contents of the file. Option A, `grep`, is used to look within files but would not be helpful in this case. The `telnet` and `export` commands are not used for this purpose.
56. Which of the following commands will display the last 50 lines of your command history when using Bash, including commands from the current session?

    1. `bashhist 50`
    2. `history 50`
    3. `cat .bash_history`
    4. `tail -f .bash_history`

    Answer:

    B.  The `history` command will display your command history, including commands from the current session. You can specify how many lines of history to display, as shown in the answer for this question. Note that `.bash_history` will not show the current session's history.
57. When using Bash, how would you execute the last command starting with a certain string, even if that command was not the last one that you typed?

    1. Precede the command with `!` and then the string to search for.
    2. Search for the command in history.
    3. Precede the command with a `?` and then the string to search for.
    4. This is not possible with Bash.

    Answer:

    A.  Preceding the command with a `!` will search history and execute the specified command. For example, `!vi` will start your last Vi session.
58. Which shell built-in command can be used to determine the location from which a given command will be run?

    1. `type`
    2. `when`
    3. `find`
    4. `help`

    Answer:

    A.  The `type` built-in command returns the location that the shell will use in order to run the given command. The `find` command cannot be used for this purpose, and the other commands do not exist.
59. Which command is used to read and execute commands from a file in the Bash shell?

    1. `run`
    2. `execute`
    3. `source`
    4. `func`

    Answer:

    C.  The `source` command is used to execute commands from a file. A typical use case is to create functions or variables that are then available for use within the current session. The other commands listed do not exist.
60. You need a command to be executed on logout for all users. Within which file should this be placed (assume all users are using Bash)?

    1. `~/.bash_logout`
    2. `/etc/bash.bash_logout`
    3. `/home/.bash_logout`
    4. `/etc/bash_logout`

    Answer:

    B.  While it's true that every user has a `.bash_logout`, the file exists in their home directory and therefore can be edited by the user. Therefore, to ensure that the required command is executed at logout, the file `/etc/bash.bash_logout` must be used.
61. Which of the following commands removes an environment variable that has been set?

    1. `profile --unset`
    2. `env -u`
    3. `set -u`
    4. `import`

    Answer:

    B.  The `env -u` command will unset an environment variable for the current session. The `unset` command can also be used for this purpose.
62. When setting the shebang line of a shell script, which of the following commands will help to determine the location of the interpreter automatically?

    1. `#!/usr/bin/env bash`
    2. `#!/bin/bash`
    3. `#!env`
    4. `/bin/int bash`

    Answer:

    A.  The `env` command, when used as `#!/usr/bin/env bash`, will determine the location of the Bash interpreter automatically. This makes the resulting script more portable for systems where Bash may not be located in `/bin/`.
63. Which of the following best describes the `PS1` environment variable?

    1. `PS1` is used to set the location of the `PostScript` command.
    2. `PS1` is used to define the default shell prompt for Bash.
    3. `PS1` is used as a per-system variable.
    4. `PS1` is user-defined and does not have a default value or setting.

    Answer:

    B.  The `PS1` variable usually has its default set in `/etc/profile` and is used as the shell prompt. Users can customize the prompt to include hostname, working directory, and other elements.
64. Which variable within a Bash script is used to access the first command-line parameter?

    1. `$ARG`
    2. `$0`
    3. `$1`
    4. `$ARG0`

    Answer:

    C.  The `$1` variable is automatically available within Bash scripts and represents the first command-line argument. The `$0` variable is the script itself. The other variables listed in this question do not exist by default.
65. Which of the following commands will print a list of six numbers beginning at 0?

    1. `list 0-5`
    2. `seq 0 1 5`
    3. `echo 0-5`
    4. `seq 0 1 6`

    Answer:

    B.  The `seq` command is used to print a sequence of numbers in a variety of formats. The answer for this question provides a starting point (0), an increment (1), and the final number (5), thus resulting in six numbers being displayed as output.
66. Which of the following commands will execute a script and then exit the shell?

    1. `run`
    2. `source`
    3. `./`
    4. `exec`

    Answer:

    D.  The `exec` command executes the command given as its argument and will then exit the shell. The `source` command does not exit the shell.
67. Which command within a shell script awaits user input and places that input into a variable?

    1. `exec`
    2. `get`
    3. `read`
    4. `prompt`

    Answer:

    C.  The `read` command awaits user input and places that input into the specified variable. The `exec` command is used to execute commands, and the other options are not valid for the purpose described.
68. What characters are used to mark a sequence of commands as a function within a shell script?

    1. Parentheses to declare the function (optional), and curly braces to contain the commands
    2. Curly braces to declare the function, and parentheses to contain the commands
    3. Square brackets to declare the function, and curly braces to contain the commands
    4. Run quotes to denote the function

    Answer:

    A.  Parentheses are used to denote a function, such as `myFunction()`. The parentheses are optional but are then followed by curly braces containing the commands to be executed when the function is called.
69. Which character sequence is used to terminate a `case` statement in a Bash script?

    1. `end`
    2. `done`
    3. `esac`
    4. `caseend`

    Answer:

    C.  The sequence `esac`, which is `case` spelled backward, is used to indicate that a `case` statement has ended. Of the other options, the `done` statement is used for termination of certain loops in Bash.
70. Which option to `declare` displays output in a way that could then be used as input to another command?

    1. `-o`
    2. `-n`
    3. `-p`
    4. `-m`

    Answer:

    C.  The `-p` option displays `declare` statements in a way that the commands are fully qualified and could then be used as input for another command, through either piping or redirection to a script.
71. Which characters are used to denote the beginning and end of the test portion of a `while` loop in a shell script?

    1. Parentheses ( )
    2. Curly braces { }
    3. Square brackets \[ ]
    4. Double quotes “ ”

    Answer:

    C.  Square brackets are used to denote the beginning and end of the test portion of a `while` loop in a shell script. Other languages generally use parentheses for this purpose.
72. When using the `test` built-in with one argument, what will be the return if its argument is not null?

    1. `false`
    2. `true`
    3. `unknown`
    4. `-1`

    Answer:

    B.  The `test` built-in will return true and can be used to test for the value existence of a variable not being null. Note that the behavior of the `test` built-in differs depending on the number of arguments.
73. Which environment variable is used when changing directory with the tilde character, such as `cd ~` ?

    1. `HOMEDIR`
    2. `HOMEPATH`
    3. `HOME`
    4. `MAILPATH`

    Answer:

    C.  The `HOME` environment variable, set automatically to the user's home directory, is consulted when the command `cd ~` is entered. The other paths beginning with `HOME` do not exist by default, and the `MAILPATH` environment variable shown contains a list of locations where mail is checked when the shell is used interactively.
74. You would like to examine the entries for a single file through the `git commit` history. Which command should be used for this purpose, assuming a filename of `nhl_scores.php`?

    1. `git log --history nhl_scores.php`
    2. `git log --follow nhl_scores.php`
    3. `git history nhl_scores.php`
    4. `git commit-history nhl_scores.php`

    Answer:

    B.  The `git log` command will be used for this purpose, with an option of `--follow` and the filename/path to follow through history.
75. Which of the following best describes attributes of an inventory within an automated continuous integration/continuous deployment (CI/CD) infrastructure?

    1. Parameters such as the client IP address and software versions
    2. The number of client nodes
    3. The software used on the server for the orchestration
    4. The architectural pattern for deployment

    Answer:

    A.  Parameters and other facts about the clients are also called _attributes_ in an orchestration.
76. Which operator should be used when comparing integers to determine if one is equal to another in a Bash script?

    1. `-ro`
    2. `===`
    3. `-eq`
    4. `-fe`

    Answer:

    C.  The integer comparison `-eq` is used for comparing integers within Bash scripts. The other answers are not valid for Bash script comparison.
77. You would like to run several commands in succession but not have the output sent into the next command. Which of the following metacharacters will accomplish this task?

    1. `&`
    2. `>`
    3. `;`
    4. `|`

    Answer:

    C.  The semicolon metacharacter chains multiple commands together but does not use the output from one command as input to the next. If the output needs to be sent into the next command, the pipe character (option D) is used. A single ampersand places a task in the background, thus making option A incorrect; a greater-than sign redirects standard output, making option B incorrect as well.
78. Which escape sequence is used to denote the alert or bell?

    1. `\a`
    2. `\b`
    3. `\c`
    4. `\d`

    Answer:

    A.  The `\a` escape sequence, when used with the `echo` command, sounds an alert or bell. The `\b` option is a backspace. The `\c` option indicates that `echo` should not produce any additional output. There is no `\d` option for `echo`.
79. Which of the following is a valid variable declaration in a Bash script, setting the variable `NUM` equal to 1?

    1. `NUM = 1`
    2. `$NUM = 1`
    3. `NUM= 1`
    4. `NUM=1`

    Answer:

    D.  It is important to note that there cannot be any spaces between the variable name and the equal sign. Likewise, there cannot be any spaces between the equal sign and the contents of the variable. This makes option D the only correct answer.
80. Which of the following commands will obtain the date in seconds since the epoch and place it into a variable called `DATE` within a shell script?

    1. `DATE=“$(date +%s)”`
    2. `DATE=“date”`
    3. `DATE=“$(date)”;`
    4. `DATE=“$date %s”`

    Answer:

    A.  The provided answer performs command substitution and places the value from the resulting command into a variable. Note the use of `+%s` formatting on the date, which then formats the output as seconds since the epoch, as specified in the question. Option C will provide the date within the `DATE` variable but will not format it as specified.
81. Which sequence is used to mark the beginning and end of the commands to execute within a `for` loop in a shell script?

    1. Curly braces `{ }`
    2. The keywords `do` and `done`
    3. Semicolons ;
    4. Tabs

    Answer:

    B.  In shell scripts, the commands to execute begin at the `do` keyword and end at the `done` keyword. Other languages generally use either curly braces or tabs.
82. Which option to the `declare` command will create a variable that is read-only?

    1. `-r`
    2. `-ro`
    3. `-p`
    4. `-x`

    Answer:

    A.  The `-r` option to `declare` will create or mark the variable as read-only. The `-p` option prints output in a format that can be reused. The `-x` option declares the variable for export.
83. Which environment variable controls the format of dates and times, such as a 12-hour or 24-hour formatted clock?

    1. `LOCALE_DATE`
    2. `DATE_FORMAT`
    3. `LC_TIME`
    4. `LC_DATE`

    Answer:

    C.  The `LC_TIME` environment variable is used to control the display and behavior of the date and time and can be changed to a different locale in order to achieve the desired display and behavior of date and time formatting. The other options shown for this question do not exist.
84. Which option to `netstat` displays interface information in a table-like format that might be suitable for use with scripting?

    1. `-i`
    2. `-r`
    3. `-t`
    4. `-l`

    Answer:

    A.  The `-i` option shows interface information in a table-like format. This option is used to see information such as transmit and receive bytes as well as the MTU for the interface and other information. The `-r` option shows routes, while `-l` shows listening sockets. There is no `-t` option.
85. You are running a shell script from within your SSH session. Which key combination can be used to terminate the script?

    1. Ctrl+X
    2. Ctrl+-
    3. Ctrl+C
    4. Ctrl+Esc

    Answer:

    C.  The Ctr\l+C key combination kills a shell script that you are running interactively. The other key combinations may have an effect but not within this context or for the desired behavior.
86. Which of the following conditionals in a Bash script will test if the variable `DAY` is equal to `SUNDAY`?

    1. `if ($DAY == “SUNDAY”)`
    2. `if ($DAY -eq “SUNDAY”)`
    3. `if [ $DAY == “SUNDAY” ]`
    4. `if [ DAY = “SUNDAY” ]`

    Answer:

    C.  Shell scripting syntax uses the format shown, with square brackets around the condition to be tested and double equal signs for a string test. Variables are preceded by a dollar sign as shown.
87. Which of the following commands adds `~/code/bin` to the path?

    1. `PATH=~/code/bin:$PATH`
    2. `PATH=/code/bin:$PATH`
    3. `PATH=/home/code/bin:$PATH`
    4. `PATH=PATH:~/code/bin`

    Answer:

    A.  The syntax for setting the `PATH` separates the new path with a colon, as shown in the correct option. A primary difference between the correct and incorrect options for this question is in how the actual specified path is shown.
88. Which option to `git merge` can be used to attempt to roll back a merge that has conflicts?

    1. `--rollback`
    2. `--abort`
    3. `--rewind`
    4. `--restart`

    Answer:

    B.  The `--abort` option attempts to roll back a problematic merge. The other options shown do not exist as options to the `git merge` command.
89. Which environment variable can be used to change the default path for a new git repository created with `git init`?

    1. `GIT_DIR`
    2. `GIT_HOME`
    3. `GIT_DEST`
    4. `GIT_LOC`

    Answer:

    A.  The `GIT_DIR` environment variable can be used to change the default location away from the `./.git` directory in which a new repository would normally be created. The other options are not used by git as environment variables.
90. Which character sequence is used to add a horizontal tab using `echo` with a Bash script?

    1. `\h`
    2.
    3. `\a`
    4. `\f`

    Answer:

    B.  The  escape sequence adds a horizontal tab. The other characters may have different meaning and so are not valid for this question. For example, `\a` is alert or bell.
91. You need to exclude a build file, called `build.o`, from being tracked by git. Which character sequence can be used in the `.gitignore` file to exclude or ignore that file in all directories?

    1. `build.o`
    2. `/build.o`
    3. `**/build.o`
    4. `build.*`

    Answer:

    C.  The double-asterisk sequence has special meaning and indicates that the file will be ignored in all directories.
92. Which file-globbing sequence will match all files that begin with an uppercase _A_ or an uppercase _F_?

    1. `[AF]*`
    2. `[af]*`
    3. `*AF*`
    4. `AF*`

    Answer:

    A.  The scenario requires alternation. Therefore, square brackets will be used to indicate the beginning of the sequence. After the brackets, a single asterisk indicates a wildcard. The other options will not work for the scenario described.
93. Assuming a remote name of `origin`, which `git` command can be used to obtain additional information about the remote?

    1. `git show origin`
    2. `git remote show origin`
    3. `git show remotes`
    4. `git remote list`

    Answer:

    B.  The `git remote` command will be used for this purpose, and when the command is given the `show` option and the remote name (`origin`, in this case), additional information about that remote will be displayed. The command is useful for displaying information about the destination for pushed code.
94. Which character sequence displays the number of command-line arguments that were passed to a Bash script?

    1. `$NUM`
    2. `$CLA`
    3. `$+`
    4. `$#`

    Answer:

    D.  The `$#` character sequence contains the number of command-line arguments that were passed to a shell script. The other options shown are not predefined by Bash.
95. Which environment variable can be set if you wish to automatically log users out of their shell after a certain period of inactivity?

    1. `TIMEOUT`
    2. `TMOUT`
    3. `TO`
    4. `IDLETIME`

    Answer:

    B.  The `TMOUT` variable can be set in a given user's shell, and they will be logged out after the value given (in seconds) of inactivity. The other environment variables listed here do not exist.
96. You are debugging a Bash script and notice a line that contains `echo $NUM #sending $NUM to output`. What will be the result of this line when executed?

    1. It will not output anything because it is commented out.
    2. It will cause a syntax error because it is invalid syntax.
    3. It will output the contents of the `NUM` variable.
    4. It will output the sequence “$NUM”.

    Answer:

    C.  The line will output the contents of the `NUM` variable. The comment occurs after the command on the line, and only code after the `#` appears is ignored.
97. When cloning a repository with `git clone`, you need to change the name of the remote so that it is not called `origin`. Which option can be added to `git clone` to accomplish this task?

    1. `--origin`
    2. `--remote`
    3. `--name`
    4. `--remote-name`

    Answer:

    A.  Using the `--origin` or `-o` option enables the name to be changed from the default of `origin`. The other choices are not options with `git clone`.
98. When working in a virtual server environment, which column within `iostat` output shows the amount (percentage) of time spent in an involuntary wait scenario due to the hypervisor?

    1. `proc`
    2. `wait`
    3. `user`
    4. `steal`

    Answer:

    D.  The `steal` column shows the percentage of time that was spent waiting due to the hypervisor stealing cycles for another virtual processor and can be used with infrastructure automation to indicate that additional CPU resources need to be deployed.
99. If you need to temporarily reconfigure all locale variables and settings for a given session, which environment variable can be used?

    1. `LC_LIST`
    2. `LC_GLOBAL`
    3. `LC_ALL`
    4. `ALL_LOCALE`

    Answer:

    C.  The `LC_ALL` variable can be used to set environment variables for the locale and will override others. This can be used when there is a need for a temporary change. The other variables listed here are not used for this purpose and are not created by default.
100.    A set of commands to execute on a client node is an example of which type of infrastructure automation?

        1. Procedure
        2. Subset
        3. Agent
        4. Collection

        Answer:

        A.  A procedure is one or more commands that are executed on a client node as part of infrastructure automation.
101.    Which character sequence is used to indicate the end of an individual clause within a `case` statement in a Bash script?

        1. `//`
        2. `'eol`
        3. `;;`
        4. `<`

        Answer:

        C.  Double semicolons are used to indicate the end of an individual clause within a Bash script. The other sequences shown do not accomplish the task described.
102.    Which of the following commands removes a currently defined aliased command?

        1. `remove`
        2. `rm`
        3. `unalias`
        4. `delete`

        Answer:

        C.  The `unalias` command is used to remove a previously defined alias. The `rm` command will remove regular files but not aliases. The other commands do not exist.
103.    Which of the following tests will determine if a file exists in the context of a shell script?

        1. `-a`
        2. `-e`
        3. `-m`
        4. `-i`

        Answer:

        B.  The `-e` option checks to ensure that a file exists and is typically used in the context of a conditional within a shell script. The other options may work within shell scripts but are not tests for file existence.
104.    Which of the following values for the `LANG` environment variable will configure the system to bypass locale translations where possible?

        1. `LANG=COMPAT`
        2. `LANG=NONE`
        3. `LANG=C`
        4. `LANG=END`

        Answer:

        C.  Setting `LANG=C` as an alias for POSIX compatibility will cause programs to bypass locale translations. The other options shown for `LANG` are not valid.
105.    Which option to the `git config` command shows all of the configuration parameters that have been set?

        1. `--list`
        2. `--show`
        3. `-u`
        4. `--display`

        Answer:

        A.  The `--list` option shows the current configuration parameters for git. The other options do not exist as options for the `git config` command.
106.    Which character sequence should be used if you need to redirect `STDERR` to a file and append to the file?

        1. `2>`
        2. `2>>`
        3. `&>>`
        4. `1>>`

        Answer:

        B.  The number 2 indicates `STDERR` redirection, and double greater-than signs indicate that the output will be appended rather than overwriting.
107.    When working with infrastructure as code, you have received a file with a `.yml` extension. What is the likely format for the contents of this file?

        1. YAML
        2. XML
        3. Tab-delimited
        4. Text

        Answer:

        A.  A file with a `.yml` extension usually contains YAML. The question also gave a hint of infrastructure as code, where many tools use YAML for configuration and procedures.
108.    Which of the following best describes the result of the command `cat /etc/passwd | cut -d: -f1 > users.txt`?

        1. The first field will be extracted from the passwd file and placed into a file called `users.txt`.
        2. The second field will be extracted from the passwd file and placed into a file called `users.txt`.
        3. The passwd file will be separated based on a colon and output placed into `users.txt`.
        4. The passwd file will be sent to the terminal where only fields beginning with a colon will be shown and placed into a file called `users.txt`.

        Answer:

        A.  The passwd file will be sent to `STDOUT`, where it will be captured and sent into the `cut` command. The `cut` command will separate the contents of the file line-by-line using a colon as a delimiter. The first field will be sent to `STDOUT` and placed into a file called `users.txt`.
109.    Which shell built-in can be used to move positional parameters down, where `$2` becomes `$1, $3` becomes `$2,` and so on?

        1. `move`
        2. `rev`
        3. `shift`
        4. `dec`

        Answer:

        C.  The `shift` command moves positional parameters down by one. This can be helpful for complex scenarios with several command-line arguments, each containing an option.
110.    You are using `git pull` to obtain changes to a shared repository. Which option should you add to `git pull` in order to prevent autocommit so that you can look at the results of the merge first?

        1. `--pre-merge`
        2. `--no-auto`
        3. `--nc`
        4. `--no-commit`

        Answer:

        D.  The `--no-commit` option should be added to `git pull` to prevent the merge from being automatically committed.
111.    Which of the following pairs indicates the beginning and end of an `until` loop in a Bash script?

        1. `do`; `done`
        2. `start`; `stop`
        3. `beg`; `end`
        4. `until`; `litnu`

        Answer:

        A.  As with the `for` loop, the commands within an `until` loop are delineated with `do` and `done`.
112.    Which exit code is used to indicate a general error within a Bash script?

        1. 0
        2. 1
        3. 256
        4. −1

        Answer:

        B.  An exit code of 1 indicates a general error. The exit code of 0 indicates success, and 256 is out of range. There is no -1 exit code for Bash.
113.    You need to redirect `STDIN` until a certain character combination is encountered. Which of the following operators can be used for this purpose?

        1. `>STDIN`
        2. `<<`
        3. `<&`
        4. `>`

        Answer:

        B.  The `<<` operator is used for this purpose and will read from `STDIN` until the specified character or characters are encountered. This is sometimes called a Here Document or HEREDOC. Among the other options for this, only `>` is valid and causes `STDOUT` to be redirected.
114.    Assuming that a file has been previously added to a repository with `git add`, which option to the `git commit` command can be used to automatically add and commit the file?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        A.  The `-a` option, when added to `git commit`, automatically commits previously known files. The `-c` option invokes the editor for the commit, and the other options do not exist.
115.    Which locale-related environment variable is used for currency-related localization?

        1. `LC_MONE`
        2. `LC_CURRENCY`
        3. `LC_MONETARY`
        4. `LC_CURR`

        Answer:

        C.  The `LC_MONETARY` variable is used by certain programs to determine the localization for currency.
116.    Which of the following lines added to `.profile` in a user's home directory will set their time zone to Central time?

        1. `TZ=/Central ; export TZ`
        2. `TIMEZONE='America/Chicago' ; export TIMEZONE`
        3. `set TZ=/Central`
        4. `TZ='America/Chicago'; export TZ`

        Answer:

        D.  The `TZ` environment variable is used for this purpose, and the general format is as shown, thus making option D the correct answer.
117.    Which of the following creates an array in a Bash script?

        1. `ARRAY=(val1 val2)`
        2. `ARRAY = “val1 val2”`
        3. `ARRAY_PUSH($ARRAY,“val1”,“val2”);`
        4. `ARRAY{0} = “val1”`

        Answer:

        A.  Array creation in a shell script involves parentheses when used in this manner. You can also use square brackets to define individual elements, as in `ARRAY[0] = “val1”`.
118.    Which test within a shell script `while` loop will examine one value to see if it is less than another?

        1. `-less`
        2. `-lessThan`
        3. `-lt`
        4. `-lthan`

        Answer:

        C.  The `-lt` operator is used to test for “less than” conditions within a script. The other operators are not valid for use in a shell script.
119.    Assuming that a space-separated list of values has been defined as `LIST=“one two three four”`, which of the following `for` loop constructs will iterate through the elements in the list?

        1. `for LIST`
        2. `for VAR in LIST`
        3. `for VAR in $LIST`
        4. `for $LIST -> $VAR`

        Answer:

        C.  The `for` loop construct in this case will require the variable name `LIST` to be preceded with a dollar sign (`$`), thus making option C correct. The other options will not work for the purpose described.
120.    Which keyword(s) is/are used to begin an alternate condition within a Bash script?

        1. `if`
        2. `else if`
        3. `elif`
        4. `elsif`

        Answer:

        C.  The `elif` keyword is used to create an alternative execution path within a shell script. The other constructs, such as `else if` and `elsif`, are used in other languages.
121.    Within which directory does git store a local copy of the repository metadata?

        1. `.gitmeta`
        2. `gitlocalmeta`
        3. `.git`
        4. `git`

        Answer:

        C.  The `.git` directory is used for storage of metadata for the repository.
122.    You need to redirect both `STDERR` and `STDOUT` to a file. Which of the following character sequences accomplishes this task?

        1. `2>`
        2. `2>&1`
        3. `2+1`
        4. `+2+1`

        Answer:

        B.  The character sequence shown in option B is the correct sequence to redirect both `STDERR` and `STDOUT`. Of the other options shown, option A will redirect only `STDERR`. The other options shown are not valid.
123.    Within a Bash script, you need to run two commands but only run the second command if the first fails. Which of the following metacharacters can be used to accomplish this task?

        1. `<>`
        2. `&`
        3. `& &`
        4. `||`

        Answer:

        D.  The double-pipe metacharacter executes the right-hand command only if the first command fails. A single ampersand sends the command into the background, thus making option B incorrect. The double-ampersand metacharacter executes the second command, but only if the first command succeeds, thus making option C incorrect.
124.    Which of the following commands creates a new branch called `project1` and points the `HEAD` toward that branch?

        1. `git branch project1`
        2. `git checkout project1`
        3. `git checkout -b project1`
        4. `git create project1 -H`

        Answer:

        C.  The `git checkout` command switches the location to which `HEAD` is pointing. By adding the `-b` option, the branch is also created.
125.    Which of the following best describes the difference between a `while` and an `until` loop in a Bash script?

        1. A `while` loop always executes once; an `until` loop does not.
        2. An `until` loop always executes once; a `while` loop does not.
        3. A `while` loop executes as long as a condition is true; an `until` loop executes until the condition is false.
        4. An `until` loop executes until a condition is true; a `while` loop executes until a condition is false.

        Answer:

        D.  Both `while` and `until` loops execute until a condition changes. The `while` loop stops when the condition is no longer true, and an `until` loop executes until the condition is true.
126.    Which statement can be used in a Bash script to determine if variable `$num1` is greater than `$num2`, assuming both variables contain integers?

        1. `if [ “$num1” -gt “$num2” ]`
        2. `if [ “$num1” > “$num2” ]`
        3. `if ($num1 -gta $num2)`
        4. `if [ $num1 gt $num2 ]`

        Answer:

        A.  Comparing integers is typically accomplished using the binary comparison operators like `-gt`, `-eq`, and so on. Option B is incorrect because the `>` operator is used in square brackets. There is no `-gta` operator or `gt` operator, making both option C and option D incorrect.
127.    Which of the following protocols is typically used for agentless infrastructure orchestration?

        1. SMTP
        2. ICMP
        3. SSH
        4. FTP

        Answer:

        C.  SSH is typically used for communication between nodes in an agentless orchestration. Less common would be a protocol such as HTTPS. The other protocols shown as options would not be used for agentless orchestration.
128.    Which of the following character sequences expands or interpolates a variable called `VAR` within a Bash script?

        1. `VAR`
        2. `$(VAR}`
        3. `${VAR}`
        4. `*VAR*`

        Answer:

        C.  Variable or parameter expansion is accomplished using `${ }` wrapped around the parameter name.
129.    You are creating a configuration file in JSON format for use with Terraform. Which of the following is the expected file extension for this configuration file?

        1. `.tf`
        2. `.txt`
        3. `.tf.json`
        4. `.tfjs`

        Answer:

        C.  Normal Terraform syntax files use a `.tf` extension, while those that use JSON should have a `.tf.json` extension.
130.    Which of the following commands displays the status of a pod on a Kubernetes cluster?

        1. `kubectl status`
        2. `kubectl pod status`
        3. `kubectl status pods`
        4. `kubectl get pod`

        Answer:

        D.  The `kubectl get pod` command displays status of a given pod within a cluster. The other answers shown are not valid.
131.    Which of the following best describes the relationship between pods and containers with Kubernetes?

        1. Pods and containers are the same.
        2. Pods can contain multiple containers.
        3. Containers can contain multiple pods.
        4. There is no relationship between pods and containers.

        Answer:

        B.  Pods can contain multiple containers in Kubernetes and this facilitates a shared resource use case, where containers can share resources within a pod. When two containers work together within a pod, it is sometimes referred to as a sidecar configuration or a sidecar container.
132.    When working with a network configuration, which of the following terms refers to a computer with two network interfaces?

        1. Bridging
        2. Dual-homed
        3. Overlay
        4. Forwarding

        Answer:

        B.  A dual-homed networking configuration is one that has two network interfaces. Bridged networking refers to using the host adapter in a virtualization scenario. An overlay network is one that is built on top of another network. Forwarding is not related to this solution.
133.    You are using a container image for a cloud deployment and are building a stateful application that must store data between deployments. Which type of storage should be used?

        1. Ephemeral volume
        2. Bridged volume
        3. Container image
        4. Persistent volume

        Answer:

        D.  A persistent volume, sometimes called persistent storage, keeps data between deployments of the virtualized environment. A container image is used for the original boot.
134.    Which of the following describes the difference between NAT and bridging in a virtualization environment?

        1. NAT uses the host adapter IP address for all network activity, while bridging enables the virtual machine to get its own IP.
        2. NAT enables the virtual machine to get its own IP, while bridging uses the host adapter IP address for all network activity.
        3. NAT is used to enable external clients to access the virtual machine, and bridging joins two virtual machines together.
        4. NAT and bridging refer to the same thing in virtualization.

        Answer:

        A.  Network Address Translation (NAT) effectively hides the virtual machine behind the host IP address. Bridging enables the virtual machine to get its own IP and thus have external clients access it as well.
135.    When `cloud-init` is used for bootstrapping and deployment of an EC2 instance, which file format should be used for the configuration files?

        1. XML
        2. YAML
        3. HTML
        4. JS

        Answer:

        B.  The YAML format is used for configuration files that will be used with `cloud-init`. XML and the other formats listed are not used for `cloud-init`.
136.    When troubleshooting a file that is not found, you notice that the file location is linked as `../file.txt`. Which type of path has been used for this file?

        1. Virtual
        2. Symbolic
        3. Relative
        4. Absolute

        Answer:

        C.  A relative path begins with something other than a `/` whereas an absolute path always begins with a `/`, indicating the root of the filesystem. The other options, virtual and symbolic, are not valid names used to describe paths.
137.    Working with a file called `test.php` to determine line count, the output from the `wc` command is `14 18 293 test.php`. Which of the three digits corresponds to line count?

        1. `14`
        2. `18`
        3. `293`
        4. None of the options are line count.

        Answer:

        A.  The first number, `14`, is the line count. The second number is word count and the third number is byte count.
138.    Which type of logging driver is the default for Docker containers?

        1. `json-file`
        2. `sql`
        3. `normal`
        4. `yaml-file`

        Answer:

        A.  The `json-file` logging driver is the default logging mechanism for Docker. The other options shown are not valid for Docker logging.
139.    Which docker command removes an image from a host node?

        1. `del`
        2. `rem`
        3. `rmf`
        4. `rmi`

        Answer:

        D.  The `rmi` command removes an image from a host but notably does not remove the image from the registry. The other commands shown are not valid for use with `docker`.
140.    Which of the following best describes an overlay network when used with technology such as Kubernetes?

        1. An overlay network is a newly deployed network that uses real-world IP addresses on top of existing private IP addresses.
        2. An overlay network is a virtual network used for communication between containers.
        3. An overlay network is used for IPv6 communication on top of IPv4 infrastructure.
        4. An overlay network is used for communication between wifi-enabled hosts and containers.

        Answer:

        B.  An overlay network describes virtual networking typically created for and used within the context of virtualization or containerized applications. With Kubernetes, an overlay network facilitates communication within a pod.
141.    Linkerd, Consul Connect, and Istio are examples of software to provide which type of abstraction when working with Kubernetes?

        1. Service mesh
        2. Virus scanning
        3. Multifactor authentication
        4. Mapping

        Answer:

        A.  Linkerd, Consul Connect, and Istio are examples of service mesh frameworks or management systems for Kubernetes. A service mesh is used to provide abstraction and management of microservices and networking.
142.    Which of the following commands will send the contents of `/etc/passwd` to both `STDOUT` and a file called `passwordfile`?

        1. `cat /etc/passwd > passwordfile`
        2. `var /etc/passwd | passwordfile`
        3. `cat /etc/passwd | tee passwordfile`
        4. `echo /etc/passwd | stdout > passwordfile`

        Answer:

        C.  The `tee` command will send output to both `STDOUT` and the specified file, thus making option C correct. Option A will redirect output to the correct file but not to `STDOUT` simultaneously. The other answers will not work for this question.
143.    What is the default delimiter used by the `cut` command?

        1. Colon
        2. Tab
        3. Space
        4. Comma

        Answer:

        B.  The `cut` command uses Tab as its default delimiter. This can be changed with the `-d` option.
144.    What option is used to change the number of lines of output for the `head` and `tail` commands?

        1. `-l`
        2. `-f`
        3. `-g`
        4. `-n`

        Answer:

        D.  The `-n` option changes the number of lines of output for both `head` and `tail` to the number specified. The other options listed in this question are not valid for `head`, and the `-f` option follows a file with `tail` as the file grows.
145.    Which of the following `egrep` commands will examine `/etc/passwd` to find users that are using either `/bin/bash` or `/usr/bin/zsh` for their shell environment?

        1. `grep sh /etc/passwd`
        2. `egrep '/*/.sh$' /etc/passwd`
        3. `grep '/*/.=sh$' /etc/passwd`
        4. `egrep '/*/..?sh$' /etc/passwd`

        Answer:

        D.  Within a regular expression, `*` represents 0 or more characters, and in this case the problem doesn't care whether a person is using `/bin/bash` or `/usr/bin/zsh`. Likewise, `.` matches a single character. But in the case of Bash and zsh, you need to look at the first and optionally a second character: thus the `?`, which makes the second `.` optional. Finally, `$` anchors the pattern at the end of the string and is key for this regular expression.
146.    Which of the following commands searches each user's `.bash_history` file to determine if the user has invoked the `sudo` command?

        1. `find /home -name “bash_history” | grep sudo`
        2. `find /home -name “.bash_history” | xargs grep sudo`
        3. `find /home/.bash_history | xargs grep sudo`
        4. `find /home -type history | xargs grep sudo`

        Answer:

        B.  The `find` command beginning with the path and then the `-name` argument will locate all files called `.bash_history`. The output from the `find` command should be piped to `xargs`, which can then build further commands from standard input. Note that this question and solution assume that all users use the Bash shell and are keeping history.
147.    Which command can be used to convert lowercase letters to uppercase letters across an entire file?

        1. `du`
        2. `touc`
        3. `conv`
        4. `tr`

        Answer:

        D.  The `tr` command can be used for the purpose described. The `tr` command is quite powerful for text conversion and search and replace scenarios. The other commands shown do not exist.
148.    When using `sed` for a search and replace operation, which option must be included so that the substitution applies to the entire line rather than just the first instance?

        1. `g`
        2. `a`
        3. `r`
        4. `y`

        Answer:

        A.  The `g` option, also known as `global` or `greedy`, will apply the matched operation to the entire line rather than just the first instance of the match. The other options apply as they would for a Perl-Compatible Regular Expression.
149.    Which Bash environment variable is used to obtain the exit status of the most recent pipeline?

        1. `$.`
        2. `$E`
        3. `$STAT`
        4. `$?`

        Answer:

        D.  The exit status of the most recently executed pipeline is found with the `$?` environment variable. The other environment variables shown do not exist by default.
150.    Which of the following is valid syntax for creating a pull request with the `git` command?

        1. `pull-req`
        2. `pull`
        3. `request`
        4. `request-pull`

        Answer:

        D.  A git pull request is created with the `request-pull` subcommand. Of the other options shown, there is a `pull` subcommand but that is used to fetch and merge code. The other options shown do not exist.
151.    Which character combination sets the body of the message to `STDIN` when using the `mail` command?

        1. `<`
        2. `>`
        3. `<<<`
        4. `|`

        Answer:

        C.  The `<<<` character combination reads input from `STDIN`, or Standard Input, and uses it as the body of the message for the `mail` command.
152.    Which command will find directories with names beginning with `2019` located beneath the current directory?

        1. `find ./ -name “2019”`
        2. `find ./ -type d -name “2019”`
        3. `find / -type d “2019”`
        4. `find ./ -type d -name “2019*”`

        Answer:

        D.  The `-type` option causes `find` to limit its search to directories only, while the `-name` option limits the names of returned elements. Note the use of the wildcard due to the phrasing of the question. Also note the use of `./` to denote beginning the search in the current directory.
153.    Which of the following best describes the difference between merging and rebasing in Git?

        1. Merging reapplies changes from the first commit of the origin master branch to create a new snapshot and commit.
        2. Rebasing reapplies changes from one branch to the other.
        3. Merging reapplies changes from one branch to the other.
        4. Rebasing uses soft links to re-create the merge history.

        Answer:

        B.  When performing a rebase with Git, the latest common point between the two branches is used and then changes from one branch are reapplied, thus making option B the most accurate. Rebasing does not use soft links, making option D incorrect. Option A is incorrect because the application of changes may or may not come from the origin master branch and may not come from the first commit.
154.    Which of the following formats are used for SaltStack configuration files?

        1. YAML
        2. JSON
        3. TXT
        4. DOC

        Answer:

        A.  YAML is used for SaltStack configuration files. Other configuration management software also uses YAML, while others, like Chef, use JSON. None of the configuration management tools use DOC as a type of file for configuration.
155.    Which option to `git tag` enables searching through the tags for a given repository?

        1. `-s`
        2. `-a`
        3. `-d`
        4. `-l`

        Answer:

        D.  The `-l` option to `git tag` searches the repository for the specified tag. The other options shown as potential answers are not valid for this purpose.
156.    Which of the following is most accurate when referring to host networking with virtualization or containerized applications?

        1. Host networking is necessary for service communication to the outside world.
        2. Communication is limited to localhost through inter-process communication.
        3. Communication will flow through the host network stack.
        4. Virtualization and containerized applications cannot use host networking.

        Answer:

        C.  Host networking typically means that communication will flow through the host network stack in virtualization or containerized applications. You may sometimes see host networking mean that containers can only communicate with the host itself. While option B was similar to that, the option referred to communication exclusively through inter-process communication, thus making it incorrect.
157.    Which command is used to obtain a pre-built docker image from a known repository?

        1. `install`
        2. `inst`
        3. `build`
        4. `pull`

        Answer:

        D.  Performing a `docker pull` will download and prepare an image for use. From the other options, `build` is a valid docker command but is used to create an image from a Dockerfile and other related context files. The other options shown are not valid with Docker.
158.    Which of the following commands is a simple pager that is found on most Linux systems?

        1. `more`
        2. `pg`
        3. `grep`
        4. `mr`

        Answer:

        A.  The `more` command provides simple paging capabilities. Unlike the `less` command, which needs to be installed on many systems, `more` is usually available even on base installs. The `grep` command is not a pager, and the other commands are not valid.
159.    Which of the following docker commands shows the current running containers?

        1. `container show`
        2. `container ls`
        3. `list -containers`
        4. `show container`

        Answer:

        B.  The `container ls` command to docker displays the current list of containers. None of the other commands are valid.
160.    The default format for an OVF template uses which document standard?

        1. YML
        2. XML
        3. OVFMeta
        4. HTML

        Answer:

        B.  OVF files, which are used for certain virtualization scenarios, are formatted in XML. There is a file extension frequently seen as YML that typically contains YAML-formatted data, but that is not related to this question. HTML is a valid document standard but not for OVF files. There is no OVFMeta document standard.
161.    Which command can be used to search the contents of all files below your current location for files that contain the characters _DB_?

        1. `grep -r “DB” *`
        2. `grep -ri “DB” *`
        3. `cat * | less`
        4. `cat *.txt | grep DB`

        Answer:

        A.  The `grep` command will be used for this purpose. Note the difference between `grep -r` and `grep -ri`. The question did not ask for case insensitivity, and therefore the use of `-i` in option B makes it incorrect.
162.    Which docker command creates a container from an image and starts that image?

        1. `run`
        2. `go`
        3. `make`
        4. `start`

        Answer:

        A.  The `run` command creates a container and starts a Docker image. When you're working with containers, the `start` command is used to start a container and the `stop` command subsequently stops the container from running.
163.    Which docker command sends an image to the Docker Hub registry or to a local registry?

        1. `go`
        2. `send`
        3. `push`
        4. `upload`

        Answer:

        C.  The `push` command sends an image to be shared at the configured location. None of the other commands shown are valid for use with Docker.
164.    Which configuration option with a Docker configuration shows the ports that will be opened when the image is started?

        1. `PORT`
        2. `EXPOSE`
        3. `OPEN`
        4. `LISTEN`

        Answer:

        B.  The `EXPOSE` configuration option indicates ports and protocols to be opened. These options can also be given on the command line at runtime by using the `-p` option. The ports to be exposed can also be found when running the `inspect` command and are listed as `ExposedPorts` within the output.
165.    Which of the following commands can be used to connect to a Docker container?

        1. `docker telnet`
        2. `docker open`
        3. `docker go`
        4. `docker attach`

        Answer:

        D.  The `docker attach` command can be used to connect to a running container. None of the other commands shown are valid for this purpose.
166.    Which of the following commands will provide the usernames in a sorted list gathered from the `/etc/passwd` file?

        1. `cat /etc/passwd | awk -F : '{print $1}' | sort`
        2. `sort /etc/passwd | cut`
        3. `echo /etc/passwd`
        4. `cat /etc/passwd | awk '{print $1}' | sort`

        Answer:

        A.  The `cat` command will display the contents of the file `/etc/passwd` and then pipe that output to the `awk` command. The `awk` command then parses its input, splitting along the specified separator for `/etc/passwd`, which is a colon (`:`). The output is then printed and piped to the `sort` command. The `sort` command in option B will not work because the `cut` command requires an argument. Likewise, the `echo` command in option C will only `echo /etc/passwd` to `STDOUT`.
167.    Which option for the `wc` command prints the number of lines given as input?

        1. `-f`
        2. `-a`
        3. `-l`
        4. `-o`

        Answer:

        C.  The `-l` option provides the number of lines given as input. For example, `wc -l /etc/passwd` would print the number of lines in the `/etc/passwd` file. The other options given in this question are not valid for the `wc` command.
168.    What is the default number of lines printed by the `head` and `tail` commands, respectively?

        1. 10 for `head`, 5 for `tail`
        2. 5 for `head`, 10 for `tail`
        3. 10 for both `head` and `tail`
        4. 3 for both `head` and `tail`

        Answer:

        C.  Both `head` and `tail` print 10 lines of output by default.
169.    When using Docker `compose` to create a single-node multi-container application, which format is required for the configuration file?

        1. JSON
        2. YAML
        3. PDF
        4. XML

        Answer:

        B.  YAML is the format used for creating an application with `compose`. The other formats are valid but not for the purpose described.
170.    You have been asked to create a template for virtualization. The template will be in JSON format. Which of the following is the correct name for JSON?

        1. Just Simple Object Nodes
        2. JavaScript Object Notation
        3. Java Standard Object Notation
        4. JavaScript Standard Object Notation

        Answer:

        B.  JSON-formatted files are JavaScript Object Notation. These files, along with YAML files, are frequently used to provide templates and configuration information because both formats are lightweight and descriptive. When working with a VM template or automation, you may encounter these formats.
171.    When you're working to design a Kubernetes-based application, what is the name for a container that acts as a proxy to connect to services outside of the pod?

        1. ProxyCloud
        2. Ambassador
        3. Sideload
        4. Integration Container

        Answer:

        B.  An Ambassador container is a container that acts as a proxy to connect to and provide a single point of connection through which other containers in the pod communicate. Among the other answers, _sideload_ refers to a means to install an application onto a device outside of the normal app store process.
