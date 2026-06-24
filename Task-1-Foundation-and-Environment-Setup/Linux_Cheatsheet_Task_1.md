# Linux Cheat Sheet – Task 1 (Foundation & Environment Setup)

**Internship:** ApexPlanet Software Pvt. Ltd.  
**Domain:** Cybersecurity & Ethical Hacking  
**Task:** Task 1 – Foundation & Environment Setup  
**Name:** VANAM CHENCHU PUNEETH

---

## 1. Print Current Working Directory

```bash
pwd
```

Displays the current directory path.

---

## 2. List Files and Directories

```bash
ls
```

Shows files and folders in the current directory.

---

## 3. List All Files with Details

```bash
ls -la
```

Displays hidden files and detailed information.

---

## 4. Change Directory

```bash
cd directory_name
```

Moves into a specified directory.

---

## 5. Move to Parent Directory

```bash
cd ..
```

Moves one level up.

---

## 6. Create a New Directory

```bash
mkdir folder_name
```

Creates a new folder.

---

## 7. Remove an Empty Directory

```bash
rmdir folder_name
```

Deletes an empty folder.

---

## 8. Create a File

```bash
touch file.txt
```

Creates a new empty file.

---

## 9. Copy Files

```bash
cp source destination
```

Copies files or directories.

---

## 10. Move or Rename Files

```bash
mv oldname newname
```

Moves or renames files and folders.

---

## 11. Delete a File

```bash
rm file.txt
```

Removes a file.

---

## 12. Clear Terminal Screen

```bash
clear
```

Clears the terminal display.

---

## 13. Display Current User

```bash
whoami
```

Shows the logged-in user.

---

## 14. Display Hostname

```bash
hostname
```

Shows the system hostname.

---

## 15. Show System Information

```bash
uname -a
```

Displays kernel and system details.

---

## 16. Display Network Interfaces

```bash
ip a
```

Shows IP addresses and network interfaces.

---

## 17. Display Network Configuration

```bash
ifconfig
```

Displays interface configuration details.

---

## 18. Test Network Connectivity

```bash
ping IP_Address
```

Checks connectivity to another host.

**Example:**

```bash
ping 192.168.56.101
```

---

## 19. Show Listening Ports

```bash
netstat -tuln
```

Displays active listening ports.

---

## 20. Execute Commands as Administrator

```bash
sudo command
```

Runs a command with elevated privileges.

---

## 21. Update Package Lists

```bash
sudo apt update
```

Refreshes package information.

---

## 22. Upgrade Installed Packages

```bash
sudo apt upgrade
```

Updates installed software packages.

---

## 23. Download Files from the Internet

```bash
wget URL
```

Downloads files using a URL.

---

## 24. Display Command History

```bash
history
```

Shows previously executed commands.

---

## 25. Exit Terminal

```bash
exit
```

Closes the current terminal session.

---

# Commands Used in Task 1

## Check IP Address

```bash
ip a
```

Displays network interfaces and assigned IP addresses.

## Verify Connectivity Between VMs

```bash
ping 192.168.56.101
```

Confirms communication between Kali Linux and Metasploitable.

## Display Network Configuration

```bash
ifconfig
```

Shows interface details including IP and MAC addresses.

## Update Kali Linux

```bash
sudo apt update && sudo apt upgrade -y
```

Updates and upgrades installed packages.

## Check Current User

```bash
whoami
```

Displays the logged-in user account.

## View System Information

```bash
uname -a
```

Displays Linux kernel and operating system information.

## Display Hostname

```bash
hostname
```

Shows the machine hostname.

## View Command History

```bash
history
```

Lists previously executed commands.
