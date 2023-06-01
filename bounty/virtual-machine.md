# Virtual machine

View certificate at website, download it and then:

```
sudo cp Downloads/tmczroot.pem /usr/local/share/ca-certificates/tmczroot.crt
```

```
sudo update-ca-certificates
```

then reboot system and try curl command for example:

```
curl google.com
```

**VS Code Error:**

```
code . --ignore-certificate-errors
```

Fixing problem:

```
sudo apt install libnss3-tools
```

Then try to find certs:

```
sudo find ~/ -name "cert9.db"
```

or

```
sudo find ~/ -name "cert8.db"
```

Then:

```
sudo certutil -A -n tmcz -t "C,," -i ./Downloads/tmczroot.pem -d sql:/home/sarlot/.pki/nssdb
```

Then if something went wrong, go there:

{% embed url="https://chromium.googlesource.com/chromium/src/+/master/docs/linux/cert_management.md#linux-cert-management" %}







