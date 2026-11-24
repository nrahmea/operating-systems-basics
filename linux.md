
# Linux Overview and Administration

**Course:** Cisco Operating Systems Basics  
**Module:** 2 – Linux Overview  

---

## Table of Contents

1. Introduction to Linux
2. Linux Basics
3. Working in the Linux Shell
4. Linux Servers and Clients
5. Basic Server Administration
6. The Linux File System
7. Working with the Linux GUI
8. Working on a Linux Host
9. Practical Labs
10. Key Takeaways

---

# 1. Introduction to Linux

## 1.1 What Is Linux?

Linux is an open-source operating system kernel used in many different operating systems and distributions.

A Linux distribution combines the Linux kernel with system utilities, software, package management tools and often a graphical desktop environment.

Examples of Linux distributions include:

- Ubuntu
- Debian
- Fedora
- Linux Mint
- Red Hat Enterprise Linux
- Kali Linux

Linux is widely used in:

- Servers and datacenters
- Cloud infrastructure
- Embedded systems
- Desktop computers
- Networking equipment
- Cybersecurity environments

## 1.2 Linux Kernel

The kernel is the core component of an operating system.

It manages communication between software and hardware and is responsible for:

- Process management
- Memory management
- Hardware communication
- Device management
- System resources

## 1.3 Virtual Machines

A virtual machine (VM) is a software-based computer that runs an operating system inside another operating system.

Virtualisation allows multiple operating systems to run on the same physical computer.

A hypervisor manages virtual machines and allocates physical hardware resources to them.

Examples of virtualisation software include:

- Oracle VirtualBox
- VMware Workstation
- Microsoft Hyper-V

### Benefits of Virtualisation

- Run multiple operating systems on one computer.
- Create isolated testing environments.
- Experiment without directly modifying the host operating system.
- Allocate virtual CPU, memory and storage resources.
- Create snapshots to preserve virtual machine states.

---

# 2. Linux Basics

## 2.1 Linux Architecture

A Linux system can be understood through several layers:

1. Hardware – Physical components such as CPU, RAM and storage.
2. Kernel – Manages hardware and system resources.
3. Shell – Provides an interface for executing commands.
4. System utilities and applications – Programs used by the operating system and users.

## 2.2 The Shell

The shell is a command interpreter that allows users to interact with Linux through text commands.

Common Linux shells include:

- Bash (Bourne Again Shell)
- Zsh
- Fish

Bash is commonly used in Linux environments.

## 2.3 Linux Command Syntax

A typical Linux command follows this structure:

```bash
command [options] [arguments]
```

Example:

```bash
ls -l /home
```

- `ls` is the command.
- `-l` is an option.
- `/home` is the argument.

Linux commands are generally case-sensitive.

For example, `Documents` and `documents` can refer to different directories.

---

# 3. Working in the Linux Shell

## 3.1 Navigating the File System

The Linux shell provides commands for navigating directories and managing files.

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory |
| `ls` | Lists directory contents |
| `ls -l` | Displays detailed file information |
| `ls -a` | Displays hidden files |
| `cd` | Changes the current directory |
| `cd ..` | Moves to the parent directory |
| `cd ~` | Moves to the user's home directory |
| `clear` | Clears the terminal |

Example:

```bash
pwd
ls -la
cd /home
cd ..
```

## 3.2 Creating and Managing Files

| Command | Purpose |
|---|---|
| `touch` | Creates an empty file |
| `mkdir` | Creates a directory |
| `rmdir` | Removes an empty directory |
| `cp` | Copies files or directories |
| `mv` | Moves or renames files |
| `rm` | Removes files |
| `cat` | Displays file contents |
| `less` | Displays file contents page by page |
| `head` | Displays the beginning of a file |
| `tail` | Displays the end of a file |

Examples:

```bash
touch example.txt
mkdir projects
cp example.txt backup.txt
mv example.txt renamed.txt
cat renamed.txt
```

Be careful when using `rm`, because deleted files may not be recoverable through the normal desktop trash mechanism.

## 3.3 Searching for Files and Text

| Command | Purpose |
|---|---|
| `find` | Searches for files and directories |
| `grep` | Searches text for matching patterns |
| `locate` | Searches a file-name database |
| `which` | Displays the location of a command |

Examples:

```bash
find /home -name "*.txt"
grep "error" logfile.txt
which python3
```

## 3.4 Working with Text Files

Linux provides several command-line tools for viewing and editing text files.

| Command | Purpose |
|---|---|
| `cat` | Displays file contents |
| `less` | Views files interactively |
| `head` | Displays the first lines |
| `tail` | Displays the last lines |
| `nano` | Opens a simple terminal text editor |
| `vim` | Opens a terminal-based text editor |

Example:

```bash
nano notes.txt
```

## 3.5 Getting Help

Linux provides built-in documentation for commands.

| Command | Purpose |
|---|---|
| `man` | Opens the manual page for a command |
| `command --help` | Displays command usage information |
| `apropos` | Searches manual page descriptions |

Examples:

```bash
man ls
ls --help
apropos network
```

## 3.6 Linux Lab: Getting Familiar with the Linux Shell

The shell lab introduces the Linux command-line environment.

Important skills include:

- Opening and navigating the terminal.
- Identifying the current working directory.
- Listing files and directories.
- Creating and managing files.
- Using commands with options and arguments.
- Accessing command documentation.

---

# 4. Linux Servers and Clients

## 4.1 Client-Server Communication

The client-server model describes how devices communicate to request and provide services.

**Client:**

A client requests information or services from another system.

Examples:
- Web browsers
- Email clients
- SSH clients

**Server:**

A server provides services or resources to clients.

Examples:
- Web servers
- DNS servers
- File servers
- Mail servers

## 4.2 Servers, Services and Ports

A server can run multiple services simultaneously.

A network port identifies a specific application or service endpoint.

Common service ports include:

| Port | Protocol | Service |
|---|---|---|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 143 | TCP | IMAP |
| 443 | TCP | HTTPS |
| 631 | TCP/UDP | IPP |
| 3389 | TCP/UDP | RDP |

## 4.3 Common Linux Server Services

Linux can provide many different network services.

Examples include:

- SSH – Remote administration.
- Apache or Nginx – Web hosting.
- DNS – Domain name resolution.
- DHCP – Automatic network configuration.
- Samba – File and printer sharing.
- CUPS – Printing services.

## 4.4 Network Port Scanning

Port scanning is used to identify open ports and discover services listening on a system.

Administrators and security professionals use port scanning to understand network exposure and identify unexpected services.

Example using Nmap on an authorised lab system:

```bash
nmap -sV 192.168.1.10
```

This performs service and version detection on the specified target.

Only scan systems you own or have explicit permission to assess.

## 4.5 Linux Servers Lab

The Linux server lab focuses on understanding server services and network communication.

Important concepts:

- Client-server communication.
- Services listening on network ports.
- Identifying available services.
- Understanding the purpose of common network ports.
- Examining network service availability.

---

# 5. Basic Server Administration

## 5.1 Service Configuration Files

Linux services use configuration files to determine how they operate.

Configuration files are commonly stored in:

```text
/etc/
```

Examples include:

- `/etc/ssh/sshd_config` – SSH server configuration.
- `/etc/hosts` – Local hostname resolution.
- `/etc/hostname` – System hostname.
- `/etc/fstab` – Filesystem mount configuration.

Configuration files should be edited carefully because incorrect settings can prevent services from operating correctly.

## 5.2 Managing Services

Linux uses service management tools to start, stop and inspect background services.

On systems using systemd, the `systemctl` command is commonly used.

Examples:

```bash
systemctl status ssh
systemctl start ssh
systemctl stop ssh
systemctl restart ssh
```

Service names can differ between Linux distributions.

## 5.3 Hardening Devices

System hardening means reducing the attack surface of a computer by improving its security configuration.

Common security practices include:

- Installing security updates.
- Removing unnecessary software.
- Disabling unused services.
- Using strong authentication.
- Applying appropriate file permissions.
- Configuring firewalls.
- Monitoring system logs.
- Limiting administrative privileges.

## 5.4 Monitoring Service Logs

Linux logs provide information about system activity, errors and service behaviour.

Many Linux distributions store log files in:

```text
/var/log/
```

Common log files include:

| Log file | Purpose |
|---|---|
| `/var/log/syslog` | General system messages on Debian-based systems |
| `/var/log/auth.log` | Authentication-related events on Debian-based systems |
| `/var/log/kern.log` | Kernel messages on systems that use this log |
| `/var/log/dmesg` | Boot and kernel-related messages |

Log locations and names can vary between distributions.

Useful commands:

```bash
ls /var/log
cat /var/log/syslog
less /var/log/auth.log
tail -f /var/log/syslog
```

The `tail -f` command follows new log entries as they are written.

## 5.5 Lab: Locating Log Files

The lab focuses on locating and examining Linux log files.

Important skills include:

- Navigating the `/var/log` directory.
- Identifying different log files.
- Viewing log contents.
- Understanding the purpose of system logs.
- Using command-line tools to investigate system activity.

---

# 6. The Linux File System

## 6.1 Linux Directory Structure

Linux uses a hierarchical filesystem structure.

The root directory is represented by:

```text
/
```

All files and directories are organised beneath the root directory.

Common directories include:

| Directory | Purpose |
|---|---|
| `/` | Root of the filesystem |
| `/home` | User home directories |
| `/root` | Root user's home directory |
| `/etc` | System configuration files |
| `/var` | Variable data such as logs |
| `/tmp` | Temporary files |
| `/bin` | Essential user commands on systems using this layout |
| `/sbin` | System administration commands on systems using this layout |
| `/usr` | User applications, utilities and shared resources |
| `/dev` | Device files |
| `/proc` | Virtual filesystem containing process and kernel information |
| `/boot` | Boot-related files |
| `/mnt` | Common mount point for temporarily mounted filesystems |
| `/media` | Common mount point for removable media |

## 6.2 Linux File System Types

A filesystem determines how data is stored and organised on a storage device.

Common Linux filesystem types include:

| Filesystem | Description |
|---|---|
| ext2 | Older Linux filesystem without journaling |
| ext3 | Linux filesystem with journaling |
| ext4 | Modern and widely used Linux filesystem |
| XFS | High-performance journaling filesystem |
| Btrfs | Filesystem with features such as snapshots and checksums |
| FAT32 | Filesystem commonly used on removable storage |
| exFAT | Filesystem commonly used for removable storage |

## 6.3 Linux File Permissions

Linux uses permissions to control access to files and directories.

There are three permission categories:

- User (owner)
- Group
- Others

There are three basic permissions:

| Permission | Symbol | Meaning |
|---|---|---|
| Read | `r` | Allows reading |
| Write | `w` | Allows modifying |
| Execute | `x` | Allows execution |

Example:

```text
-rwxrw-r--
```

This represents:

| Category | Permissions |
|---|---|
| Owner | Read, write, execute |
| Group | Read, write |
| Others | Read only |

## 6.4 Numeric File Permissions

Linux permissions can also be represented using numbers.

| Permission | Value |
|---|---|
| Read (`r`) | 4 |
| Write (`w`) | 2 |
| Execute (`x`) | 1 |

Examples:

| Number | Permissions |
|---|---|
| 7 | Read, write, execute |
| 6 | Read, write |
| 5 | Read, execute |
| 4 | Read only |

Example:

```bash
chmod 754 script.sh
```

This assigns:

- Owner: 7 – Read, write, execute.
- Group: 5 – Read, execute.
- Others: 4 – Read only.

## 6.5 Managing Permissions

The `chmod` command changes file permissions.

Examples:

```bash
chmod 755 script.sh
chmod 644 notes.txt
chmod u+x script.sh
```

The `chown` command changes file ownership.

Example:

```bash
sudo chown user:user notes.txt
```

The `chgrp` command changes the group ownership of a file.

Example:

```bash
sudo chgrp staff notes.txt
```

## 6.6 Hard Links and Symbolic Links

Linux supports two types of links: hard links and symbolic links.

**Hard links**

A hard link is another directory entry that references the same inode as the original file.

Characteristics:

- Shares the same underlying file data.
- Both names reference the same inode.
- Cannot normally cross filesystem boundaries.
- Cannot normally be created for directories by ordinary users.

**Symbolic links**

A symbolic link is a separate file containing a path to another file or directory.

Characteristics:

- Can point to files and directories.
- Can reference targets on different filesystems.
- Stores the target path.
- Can become broken if the target is moved or deleted.

Create a hard link:

```bash
ln original.txt hardlink.txt
```

Create a symbolic link:

```bash
ln -s original.txt symlink.txt
```

Inspect links:

```bash
ls -li
```

The inode number helps identify whether two directory entries reference the same underlying file.

## 6.7 Lab: Navigating the Linux Filesystem and Permission Settings

The lab focuses on:

- Navigating directories.
- Locating files.
- Understanding the Linux directory structure.
- Inspecting file permissions.
- Changing file permissions.
- Understanding file ownership.
- Creating and examining hard links and symbolic links.

---

# 7. Working with the Linux GUI

## 7.1 X Window System

The X Window System, also known as X11, provides a graphical windowing system for Unix-like operating systems.

It allows graphical applications to display windows and receive user input.

## 7.2 Linux Graphical User Interfaces

Linux distributions can use different desktop environments.

Examples include:

- GNOME
- KDE Plasma
- Xfce
- Cinnamon

A desktop environment provides graphical tools such as:

- File managers.
- Application menus.
- System settings.
- Terminal applications.
- Window management.

Linux can be administered through both graphical interfaces and the command line.

---

# 8. Working on a Linux Host

## 8.1 Installing and Running Applications

Linux distributions use package managers to install, update and remove software.

Ubuntu and Debian commonly use APT.

Examples:

```bash
sudo apt update
sudo apt upgrade
sudo apt install package-name
sudo apt remove package-name
```

Important distinction:

- `apt update` refreshes the local package lists.
- `apt upgrade` installs available updates for installed packages.
- `apt install` installs a package.
- `apt remove` removes a package.

The `sudo` command allows an authorised user to execute commands with elevated privileges.

## 8.2 Keeping the System Up to Date

Keeping Linux updated is an important security and maintenance practice.

Updates can include:

- Security patches.
- Bug fixes.
- Software improvements.
- Kernel updates.
- Application updates.

Regular updates help protect systems against known vulnerabilities.

## 8.3 Processes and Forks

A process is an instance of a running program.

Linux assigns each process a Process ID (PID).

Useful commands:

| Command | Purpose |
|---|---|
| `ps` | Displays process information |
| `ps aux` | Displays detailed process information |
| `top` | Displays live process and resource information |
| `htop` | Interactive process monitor, if installed |
| `kill` | Sends a signal to a process |
| `pgrep` | Searches for processes by name |

Example:

```bash
ps aux
top
pgrep firefox
```

### Process Forking

Forking is a mechanism through which a process creates a new process.

The new process is called the child process, while the original is the parent process.

Linux uses process creation mechanisms such as `fork()` and `exec()`.

## 8.4 Malware on a Linux Host

Linux systems can also be affected by malware.

Examples include:

- Trojans.
- Worms.
- Ransomware.
- Spyware.
- Rootkits.

Security practices include:

- Installing software from trusted repositories.
- Keeping the operating system updated.
- Using appropriate permissions.
- Monitoring system activity.
- Avoiding untrusted downloads.
- Investigating unexpected processes and services.

## 8.5 Rootkits

A rootkit is a type of malicious software designed to conceal its presence and maintain unauthorised access to a system.

Rootkits can attempt to hide processes, files or other system activity.

Security tools can help detect suspicious behaviour and possible rootkit infections.

## 8.6 Rootkit Checks

Rootkit detection tools can inspect a system for signs of suspicious modifications.

An example of a Linux rootkit detection utility is:

```bash
sudo rkhunter --check
```

Another example is:

```bash
sudo chkrootkit
```

These tools can produce false positives and cannot guarantee that a system is clean.

## 8.7 Piping Commands

Pipes allow the output of one command to become the input of another command.

The pipe operator is:

```bash
|
```

Example:

```bash
ps aux | grep firefox
```

This displays process information and filters the output for entries containing `firefox`.

Another example:

```bash
ls -l | less
```

This allows directory listings to be viewed page by page.

## 8.8 Practical Lab: Configure Security Features in Windows and Linux

The course includes a practical lab covering security configuration in both Windows and Linux.

The Linux security concepts include:

- Managing user permissions.
- Understanding administrative privileges.
- Keeping software updated.
- Reviewing system security.
- Understanding malware and rootkit detection.

---

# 9. Practical Labs

The Linux module includes several practical activities.

| Lab | Main focus |
|---|---|
| Install a Virtual Machine on a Personal Computer | Virtualisation and VM setup |
| Getting Familiar with the Linux Shell | Command-line navigation and commands |
| Use a Port Scanner to Detect Open Ports | Network service discovery |
| Linux Servers | Client-server communication and services |
| Locating Log Files | Linux system logs |
| Navigating the Linux Filesystem and Permission Settings | Files, directories and permissions |
| Configure Security Features in Windows and Linux | Operating system security |

## 9.1 Practical Skills Developed

Through the lessons and labs, the following areas were covered:

- Using Linux terminal commands.
- Navigating the Linux filesystem.
- Creating and managing files and directories.
- Understanding file permissions.
- Working with hard links and symbolic links.
- Installing and updating software.
- Understanding Linux services.
- Identifying network services and ports.
- Locating and examining system logs.
- Monitoring running processes.
- Understanding Linux security mechanisms.
- Working with virtual machines.

---

# 10. Key Takeaways

The Linux module introduced the fundamentals of Linux operating systems and administration.

Important concepts include:

- Linux is an open-source operating system kernel.
- Linux distributions combine the kernel with utilities and applications.
- Virtualisation allows multiple operating systems to run on one physical computer.
- The shell provides a command-line interface.
- Linux uses a hierarchical filesystem structure.
- File permissions control access for owners, groups and others.
- Hard links reference the same inode, while symbolic links store a target path.
- Linux servers provide network services to clients.
- Ports identify application and service endpoints.
- System logs help administrators monitor and troubleshoot systems.
- APT manages software packages on Debian-based distributions.
- Processes represent running programs.
- Pipes connect the output of one command to another.
- System hardening reduces security risks.
- Rootkits are malware designed to conceal their presence.

---

# 11. Module Completion

| Section | Status |
|---|---|
| Introduction to Linux | Completed |
| Linux Basics | Completed |
| Working in the Linux Shell | Completed |
| Linux Servers and Clients | Completed |
| Basic Server Administration | Completed |
| The Linux File System | Completed |
| Working with the Linux GUI | Completed |
| Working on a Linux Host | Completed |

**Module:** Linux Overview  
**Course:** Cisco Operating Systems Basics  
**Status:** Completed

---

