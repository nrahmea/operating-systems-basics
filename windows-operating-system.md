
# Windows Operating System

**Course:** Cisco Operating Systems Basics  
**Module:** 1 – Windows Overview  

---
## 1. Windows History

This section covers the development and basic characteristics of the Windows operating system.

### 1.1 Disk Operating System (DOS)

DOS (Disk Operating System) is a command-line-based operating system.

Unlike modern Windows versions, DOS primarily relies on text commands rather than a graphical user interface.

### 1.2 Windows Versions

Microsoft Windows has evolved through multiple versions, introducing improvements in usability, security, performance and system management.

Examples include:
- Windows 7
- Windows 8 and 8.1
- Windows 10
- Windows 11

### 1.3 Windows GUI

GUI stands for Graphical User Interface.

Windows provides a graphical environment that allows users to interact with the operating system through visual elements.

Common GUI components include:
- Desktop
- Start Menu
- Taskbar
- File Explorer
- Settings
- Control Panel

### 1.4 Operating System Vulnerabilities

Operating system vulnerabilities are weaknesses that could potentially be exploited to compromise a computer system.

Security updates, strong authentication, firewalls and antivirus protection help reduce security risks.

---

## 2. Windows Architecture and Operations

This section covers the internal architecture of Windows and how the operating system manages hardware and software.

### 2.1 Hardware Abstraction Layers

The Hardware Abstraction Layer (HAL) provides an interface between the Windows operating system and the computer's hardware.

It helps Windows interact with different hardware configurations without requiring every part of the operating system to handle hardware differences directly.

### 2.2 User Mode and Kernel Mode

Windows separates system operations into two execution modes.

**User Mode**
- Used by applications and ordinary processes.
- Applications operate with restricted access to system resources.
- Helps isolate applications from critical operating system components.

**Kernel Mode**
- Used by core operating system components and device drivers.
- Has privileged access to hardware and system memory.
- Responsible for important system operations.

### 2.3 Windows File Systems

A file system determines how data is organised and stored on a storage device.

Common Windows file systems include:

- NTFS (New Technology File System)
- FAT32 (File Allocation Table 32)
- exFAT (Extended File Allocation Table)

NTFS is commonly used for modern Windows system drives and supports features such as file permissions and journaling.

### 2.4 Alternate Data Streams

Alternate Data Streams (ADS) are a feature of the NTFS file system.

They allow additional data to be associated with an existing file without appearing as a separate file in ordinary directory listings.

### 2.5 Windows Boot Process

The Windows boot process describes how a computer starts Windows.

On modern UEFI-based systems, the general process includes:

1. The computer's firmware initialises hardware.
2. The firmware identifies a bootable device.
3. Windows Boot Manager starts.
4. The Windows loader loads the required operating system components.
5. The Windows kernel initialises.
6. Windows starts the required system services and prepares the user environment.

### 2.6 Windows Startup

Windows startup involves loading the operating system, starting services and preparing the user session.

Startup applications and services can affect how quickly a computer becomes ready for use.

### 2.7 Windows Shutdown

Windows shutdown closes applications, stops services and safely powers down the computer.

A proper shutdown helps ensure that system operations are completed before the computer turns off.

### 2.8 Processes, Threads and Services

**Processes**

A process is an instance of a running program. It has its own virtual address space and system resources.

**Threads**

A thread is an execution unit within a process. A process can contain multiple threads.

**Services**

Windows services are background processes that provide functionality to the operating system and applications.

Examples include networking and system update services.

### 2.9 Memory Allocation and Handles

Windows manages memory allocation so that applications and system processes can use available memory.

A handle is a reference used by a process to access a system resource or object, such as a file, process or registry key.

### 2.10 The Windows Registry

The Windows Registry is a hierarchical database that stores configuration settings for Windows, hardware, users and applications.

It is organised into keys, subkeys and values.

Common root keys include:

- HKEY_LOCAL_MACHINE (HKLM)
- HKEY_CURRENT_USER (HKCU)
- HKEY_CLASSES_ROOT (HKCR)
- HKEY_USERS (HKU)
- HKEY_CURRENT_CONFIG (HKCC)

### 2.11 Practical Lab: Exploring Processes, Threads, Handles and Windows Registry

The practical lab focuses on exploring Windows processes, threads, handles and registry information.

Useful tools include:
- Task Manager
- Registry Editor
- Process Explorer (if available)

### 2.12 Knowledge Check: Identify the Windows Registry Hive

The knowledge check covers the identification and purpose of Windows Registry hives.

---

## 3. Windows Configuration and Monitoring

This section covers Windows administration, configuration and monitoring tools.

### 3.1 Run as Administrator

Windows supports elevated permissions through the Run as administrator option.

Administrative privileges are required for certain system configuration and management tasks.

### 3.2 Local Users and Domains

Windows supports local user accounts and domain-based accounts.

**Local accounts**
- Exist on an individual computer.
- Are managed locally.
- Can be used without a domain controller.

**Domain accounts**
- Are managed centrally through a Windows domain.
- Commonly use Active Directory Domain Services.
- Allow organisations to manage users and computers centrally.

### 3.3 Command-Line Interface (CLI) and PowerShell

The Command-Line Interface allows users to interact with Windows through text commands.

PowerShell is a command-line shell and scripting language designed for system administration and automation.

Examples of useful commands:

```powershell
Get-Process
Get-Service
Get-ComputerInfo
Get-Help
```

### 3.4 Windows Management Instrumentation (WMI)

Windows Management Instrumentation (WMI) provides an interface for accessing management information about Windows systems.

It can be used to retrieve information about hardware, software and system configuration.

### 3.5 The net Command

The `net` command is a Windows command-line utility used for managing network-related resources and accounts.

Examples:

```cmd
net user
net user username
net use
net share
```

### 3.6 Task Manager and Resource Monitor

**Task Manager**

Task Manager provides an overview of running applications, processes and system resource usage.

It can monitor:
- CPU usage
- Memory usage
- Disk activity
- Network activity
- Running processes

**Resource Monitor**

Resource Monitor provides more detailed information about system resource usage.

It helps investigate CPU, memory, disk and network activity.

### 3.7 Networking

Windows includes networking tools and configuration options that allow computers to communicate across local networks and the internet.

Examples of useful commands:

```cmd
ipconfig
ipconfig /all
ping
tracert
nslookup
```

### 3.8 Accessing Network Resources

Windows allows users to access shared network resources, including files, folders and printers.

Network resources can be accessed through File Explorer or command-line tools.

### 3.9 Windows Server

Windows Server is Microsoft's operating system designed for server environments.

It provides services and features for managing network infrastructure and organisational resources.

Examples include:
- Active Directory Domain Services
- DNS Server
- DHCP Server
- File and Storage Services

### 3.10 Practical Lab: Create User Accounts

This lab focuses on creating and managing Windows user accounts.

User accounts allow different people to access a computer with their own permissions and settings.

### 3.11 Practical Lab: Using Windows PowerShell

This lab introduces PowerShell for interacting with and managing Windows.

PowerShell commands are known as cmdlets and commonly follow a Verb-Noun naming structure.

### 3.12 Practical Lab: Windows Task Manager

This lab focuses on using Task Manager to inspect running processes and applications.

It helps users understand how Windows manages running programs and system resources.

### 3.13 Practical Lab: Monitor and Manage System Resources

This lab covers monitoring system performance and managing resource usage.

Task Manager and Resource Monitor can help identify processes consuming excessive CPU, memory, disk or network resources.

---

## 4. Windows Security

This section covers Windows security and system monitoring tools.

### 4.1 The netstat Command

The `netstat` command displays network connection information and network statistics.

Example:

```cmd
netstat -an
```

This displays active connections and listening ports using numerical addresses.

### 4.2 Event Viewer

Event Viewer is a Windows management tool used to view system, application and security event logs.

It helps administrators investigate errors, warnings and system events.

Common log categories include:
- Application
- Security
- System

### 4.3 Windows Update Management

Windows Update provides operating system updates, security patches and bug fixes.

Keeping Windows updated helps maintain system security, stability and compatibility.

### 4.4 Local Security Policy

Local Security Policy allows administrators to configure security settings on an individual Windows computer.

Examples include:
- Password policies
- Account lockout policies
- User rights assignments
- Security options

### 4.5 Windows Defender

Microsoft Defender Antivirus provides built-in protection against malware and other security threats.

It can scan files, monitor system activity and detect potentially harmful software.

### 4.6 Windows Defender Firewall

Windows Defender Firewall controls network traffic entering and leaving a computer.

It uses firewall rules to allow or block network connections based on configured conditions.

---

## 5. Practical Knowledge and Assessment

The Windows Operating System module also includes practical activities and knowledge checks.

Completed practical activities include:

- Exploring processes, threads, handles and the Windows Registry.
- Creating Windows user accounts.
- Using Windows PowerShell.
- Managing applications and processes with Task Manager.
- Monitoring and managing system resources.

The module also includes knowledge checks covering:
- Windows Registry hives.
- Windows administration and security tools.

---

## 6. Key Takeaways

After completing this module, the main concepts covered include:

- Windows history and graphical user interfaces.
- Hardware abstraction and Windows architecture.
- Differences between user mode and kernel mode.
- Windows file systems and the boot process.
- Processes, threads, services and memory management.
- The Windows Registry and its structure.
- Local users, domains and administrative privileges.
- Command Prompt and PowerShell.
- Windows management and monitoring tools.
- Network configuration and resource sharing.
- Windows Server fundamentals.
- Windows security, firewall and event monitoring.

---

## 7. Completion Status

| Section | Status |
|---|---|
| Windows History | Completed |
| Windows Architecture and Operations | Completed |
| Windows Configuration and Monitoring | Completed |
| Windows Security | Completed |
| Windows Operating System Summary | Completed |

**Course:** Cisco Operating Systems Basics  


## 8. Practical Experience

I completed the practical labs included in the Windows Operating System module.

The practical work included:

| Practical Lab | Status |
|---|---|
| Exploring Processes, Threads, Handles and Windows Registry | Completed |
| Creating Windows User Accounts | Completed |
| Using Windows PowerShell | Completed |
| Windows Task Manager | Completed |
| Monitoring and Managing System Resources | Completed |

### Skills Practised

- Exploring running processes and system resources.
- Understanding Windows Registry structure.
- Creating and managing local user accounts.
- Executing commands using Windows PowerShell.
- Monitoring CPU, memory, disk and network usage.
- Using Windows administration and monitoring tools.


**Module:** Windows Operating System  
**Status:** Completed


