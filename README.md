# PwnKit Over SSH

A script that uses SSH to test if a remote system is vulnerable to PwnKit

## Dependencies
```
sudo apt-get install python3-pip
pip3 install paramiko
```

## Outline
1. User provides username(s) and password(s)
2. Script connects to other machine over SSH
3. Script uploads binary
4. Script attempts to execute binary and returns whether or not it was succesful
