# RefreshX | Linux Update Script
## Overview

Make updating debian linux systems easier with a single command that updates and cleans old system files as well as leftover configuration files!

This script is for people like me, too many times I have input the same 6 update commands daily.
 
 ## Features
 - Updates package list | Prints complete text
 - Installs available package updates | Prints complete text
 - Updates available snap packages | Prints complete text
 - Updates local & system flatpaks | Prints complete text
 - Cleans old packages and configurations | Prints complete text
 - Cleans old system packages | It will not clean important system files | Prints complete text
 - Prints "Script Complete" when finished
 - SHA256SUM verification to ensure security for privileged commands

 Each stage of the script is displayed green in the terminal to help view any changes made during the process.

## Usage
Allow Privileges to Execute Script
```bash
chmod +x update.sh
```
Create the SHA256 Verification File
```bash
sha256sum update.sh > update.sh.sha256
```
Run Command (Default File Path (~))
```bash
./update.sh
```
## NOTE:
- Debian Distro Required (Ubuntu, Debian, Kali, etc.)
- Script Requires Sudo Privileges
- SHA256SUM Verification

The SHA256SUM command creates the verification file (sha256sum update.sh > update.sh.sha256).
If local changes are made to the script (update.sh) you must create a new SHA256 for script verification.
Alternativley the user could comment out the verification block (located at the top of the script) to prevent error (Not Recommended).
