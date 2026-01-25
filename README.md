# Linux System Administration Labs

## Overview
This repository demonstrates my practical Linux system administration skills.
All tasks were performed on a Linux OS.

The labs focus on real-world administrative tasks such as:
- User and group management
- File permissions
- Package management
- Service management
- System monitoring

---

## Environment
- Host OS: Kali Linux
- Tools: Bash, core Linux utilities

---
## How to run

### System Update & Package Management

### command: sudo apt update

***Description:**
Updates the local package index from repositories.

**Why it matters:**
Ensures the system knows about the latest available package versions.

**Example:**
```bash
sudo apt update
```

### command: sudo apt upgrade

**Description:**
Upgrades installed packages to the latest versions.

**Why it matters:**
Keeps the system secure and up to date.

**Example:***
```bash
sudo apt upgrade
```
### Screenshot
<img width="1366" height="768" alt="ad3" src="https://github.com/user-attachments/assets/0a3ca79e-f409-4de5-ac4e-4f933ba5526c" />

### command: sudo apt install htop

**Description:**
Installs the htop process monitoring tool.

**Why it matters:**
htop provides a clearer, interactive view of system processes than top.

**Example**
````bash
sudo apt install htop
````
### Screenshot
<img width="1366" height="768" alt="ad2" src="https://github.com/user-attachments/assets/c84bbb94-e113-4ce3-9fbc-c88bf2dcb437" />

## Permissions & Ownership

### command chmod

**Descreption**
Permission meaning:

7 → owner: read, write, execute

0 → group: no access

0 → others: no access

**Why it matters:**
Restricts access to sensitive directories (owner-only access).

**Example:**
```bash
chmod 700 admin_test
```
### screenshot
<img width="1366" height="733" alt="pm" src="https://github.com/user-attachments/assets/3236b8ea-271a-4779-939f-ef54d0057a17" />


### System Resource Monitoring

### command: df -h

**Description:**
Displays disk space usage for mounted filesystems.

**Common Options:**

-h → human-readable sizes

**Example***
```bash
df -h
```
### command: free -m

**Description:**
Displays memory usage.

**Common Options:**

-m → show values in megabytes
**Example**
```bash
free -m
```
### Screenshot
<img width="1366" height="768" alt="ad6" src="https://github.com/user-attachments/assets/97e14cab-ba15-4ada-9882-ebd893902417" />

---
## basics/navigation
### Command: ls

**Description:**  
Lists files and directories in a directory.

**Common Options:**
- `-l` → long listing format
- `-a` → include hidden files
- `-h` → human-readable sizes

**Example:**
```bash
ls -lah
```
<img width="1366" height="733" alt="ls lah" src="https://github.com/user-attachments/assets/f755bb15-28a5-41ad-af43-dc2fbfb5ac8c" />

### Command: pwd

**Description:**  
Prints the full path of the current working directory.

**Example:**
```bash
pwd
```
### Command: cd

**Description:**
Changes the current working directory.


**Common Options:**

cd .. → move to parent directory

cd ~ → move to home directory

cd - → return to previous directory

**Example:**

````bash
cd ..
cd ~
cd -
cd /path
````
### Command: mkdir

**Description:**  
Creates directories.

**Example:**
```bash
mkdir admin_test
```
Command: mv

Description:
Moves or renames files and directories.

Example:
```bash
mv simple.c admin_test
```

### Command: cp

**Description:**
Copies files and directories.

**Common Options:**

-r → copy directories recursively

-a → preserve attributes

**Example:**
```bash
cp 
```
### Command: touch

**Description:**
Creates empty files or updates file timestamps.

**Example:**
```bash
touch notes.txt
```
### Command: find

**Description:**
Searches for files and directories.

 **Common Options**:

-name → search by name
 
-type → filter by file type

**Example:**

```bash
find a.out
```

### Command: ln

**Description:**
Creates links between files.

**Common Options:**

-s → create symbolic link

**Example:**
```bash
ln -s /usr/bin/python3 python
```
### screenshot

<img width="1366" height="733" alt="com" src="https://github.com/user-attachments/assets/5fe53030-64ea-453b-b7b5-ebb76b6dd232" />

---

## Networking and Connectivity Tools

### Command: ping

**Description:**  
Sends ICMP echo requests to test network connectivity between the local machine and a remote host.

**Common Options:**
- `-c <count>` → number of packets to send
- `-i <interval>` → time between packets

**Example:**
```bash
ping -c 4 google.com
```
### Command: traceroute

**Description:**
Displays the path packets take to reach a destination host.

**Common Options:**

-n → do not resolve IP addresses to hostnames

-m <max> → set maximum hop count

**Example:**
```bash
traceroute google.com
```

### Command: ss

**Description:**
Displays socket statistics and active network connections.

**Common Options:**

-l → show listening sockets

-t → TCP sockets

-u → UDP sockets

-n → do not resolve service names

**Example:**

```bash
ss -tuln
```

### Command: ip

**Description:**
Displays and manages network interfaces, routes, and IP addresses.

**Common Options:**

addr → show IP addresses

link → show network interfaces

route → display routing table

**Example:**
```bash
ip addr show
```

### Command: hostname

**Description:**
Displays or sets the system hostname.

**Example:**
```bash
hostname
```
## screenshot

<img width="1366" height="733" alt="net2" src="https://github.com/user-attachments/assets/bd43ea0f-8d18-4cf9-996d-578d023926fd" />
<img width="1366" height="733" alt="net" src="https://github.com/user-attachments/assets/614b3c1b-6324-4b66-9cfa-052a86412e99" />
