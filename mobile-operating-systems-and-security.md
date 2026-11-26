
# Mobile Operating Systems and Security

**Course:** Cisco Operating Systems Basics  
**Module:** 4 – Mobile Operating Systems and Security Overview  


## Overview

Mobile devices such as smartphones and tablets use operating systems to manage hardware, run applications, provide a user interface, and manage security.

The module covered:

- Android and iOS
- Open-source and closed-source software
- Mobile touch interfaces
- Android and iOS home screens
- Common mobile device features
- Mobile operating system security
- App permissions and sandboxing
- Malware and antivirus protection
- Operating system updates and patches
- Rooting and jailbreaking
- Mobile device firewalls

---

# 1. Android Versus iOS

Mobile devices use operating systems in the same way desktops and laptops do.

The two major mobile operating systems covered in this module are:

| Operating System | Developer |
|---|---|
| Android | Google / Open Handset Alliance |
| iOS | Apple |

Both operating systems manage hardware, run applications, provide a graphical user interface, and implement security features.

## Android

Android is a Linux-based mobile operating system.

Characteristics:

- Open-source components
- Highly customizable
- Used by many manufacturers
- Available on smartphones and tablets
- Can be adapted for other devices
- Supports applications from different developers and sources, depending on device configuration

Android is used on many different types of devices, including smartphones, tablets, smart TVs, and other electronics.

## iOS

iOS is Apple's mobile operating system for iPhone devices.

Characteristics:

- Developed and controlled by Apple
- Closed-source operating system
- Integrated with Apple's hardware and services
- Applications are distributed primarily through Apple's App Store
- Strong restrictions on application execution and system access

---

# 2. Open Source Versus Closed Source

## Source Code

Source code is a set of human-readable instructions written by software developers.

Before software is executed by a computer, the instructions are processed into a form that the computer can execute.

## Open-Source Software

Open-source software makes its source code available for inspection and, depending on its license, modification and redistribution.

Advantages can include:

- Transparency
- Community development
- Customization
- Ability to inspect the code
- Contributions from multiple developers

Android contains open-source components that allow manufacturers and developers to customize the operating system.

## Closed-Source Software

Closed-source software does not publicly provide its source code.

Users generally cannot freely inspect or modify the source code.

Apple's iOS is a closed-source operating system.

## Comparison

| Feature | Open Source | Closed Source |
|---|---|---|
| Source code availability | Available | Generally unavailable |
| Code inspection | Possible | Restricted |
| Modification | May be permitted by license | Usually restricted |
| Customization | Often extensive | Usually more limited |
| Development | Community and/or organization | Controlled by developer |

---

# 3. Android Applications

Android applications are software programs designed to run on Android devices.

Applications can provide functions such as:

- Messaging
- Navigation
- Web browsing
- Games
- Productivity
- Media playback
- Banking
- Communication

Android applications may be installed through supported application stores or other installation methods, depending on the device's configuration and security settings.

Because applications may request access to device resources, users should carefully review permissions before installing applications.

---

# 4. iOS Applications

iOS applications are designed to run on Apple's mobile operating system.

Applications are primarily distributed through the Apple App Store.

Apple uses an application review process before apps are released through its official store.

Developers can create iOS applications using Apple's development tools and software development frameworks.

The official App Store distribution and review process helps reduce the distribution of malicious applications, although it does not guarantee that every application is completely safe.

---

# 5. Mobile Touch Interfaces

Mobile operating systems use graphical interfaces designed for touchscreen interaction.

Users interact with applications and system functions using touch gestures.

## Common Touch Gestures

| Gesture | Function |
|---|---|
| Tap | Select or open an item |
| Long press | Display additional options or activate a contextual action |
| Swipe | Move between screens or scroll |
| Drag | Move an item |
| Pinch | Zoom in or out |
| Double tap | Perform an additional action, depending on the application |

The exact behavior of gestures can vary depending on the operating system and application.

---

# 6. Android Home Screen

The Android home screen is the main interface used to access applications and system functions.

Android home screens may contain:

- Application icons
- Widgets
- Navigation icons
- Notification icons
- System status icons
- Screen indicators

Users can access additional home screens by swiping left or right.

## Android Home Screen Components

### Application Icons

Application icons provide access to installed applications.

### Widgets

Widgets display information or provide functionality directly on the home screen.

Examples include:

- Weather information
- Calendar events
- Clock
- Music controls

### Notification Icons

Notification icons indicate that an application or system service has information for the user.

### System Icons

System icons may indicate:

- Battery status
- Wi-Fi connection
- Cellular signal
- Bluetooth
- Time

### Screen Indicator

The screen indicator shows which home screen is currently active.

---

# 7. iOS Home Screen

The iOS home screen provides access to installed applications and system functions.

The interface differs from Android in several ways.

According to the course material:

- iOS does not use the same navigation icons as Android.
- Older iPhones use a physical Home button for navigation.
- Newer iPhones use gestures for navigation.
- The iOS home screen primarily contains application icons and other content.
- iOS does not use Android-style application shortcuts and widgets in the same way described in the course material.

## Home Button

Older iPhones use a physical Home button for functions such as:

- Waking the device
- Returning to the home screen
- Activating Siri or voice control

Newer iPhone models without a physical Home button use gestures and other hardware controls.

---

# 8. Common Mobile Device Features

Mobile devices provide many features beyond basic communication.

Common features include:

- Camera
- GPS and location services
- Navigation
- Wireless communication
- Bluetooth
- Wi-Fi
- Cellular connectivity
- Voice assistants
- Multimedia
- Mobile applications
- Touchscreen interaction

## Automobile Applications

Modern vehicles may integrate smartphones with in-vehicle entertainment and information systems.

Examples include:

- Android Auto
- Apple CarPlay

A smartphone can connect to a vehicle using USB or Bluetooth, depending on the vehicle and device.

Common functions include:

- Navigation
- Music playback
- Hands-free calling
- Talk-to-text
- Voice assistants
- Calendar information

These features allow users to access certain smartphone functions through the vehicle's interface.

---

# 9. Mobile Device Security

Mobile devices are computers and are vulnerable to malicious software.

Security measures are used to protect:

- The operating system
- Applications
- Personal data
- Network connections
- User accounts

Mobile operating systems use multiple security mechanisms to reduce the risk of malware and unauthorized access.

---

# 10. Application Sandboxing

A sandbox is an isolated environment in which an application runs.

Sandboxing prevents applications from freely accessing other applications and system resources.

## Purpose of Sandboxing

Sandboxing helps:

- Isolate applications from each other
- Restrict access to system resources
- Reduce the impact of malicious applications
- Prevent applications from interfering with other applications
- Improve operating system security

Mobile applications generally run within their own isolated environments.

If an application becomes malicious, sandboxing can limit its ability to affect the entire operating system or other applications.

However, sandboxing does not make an application completely harmless.

---

# 11. Application Permissions

Applications may request permission to access specific device resources.

Examples include:

- Camera
- Microphone
- Location
- Contacts
- Files
- Photos
- Bluetooth

Permissions determine which resources an application is allowed to access.

## Android Permissions

Android applications request permissions for resources they need.

If a user grants permission, the application may be able to access the corresponding resource.

A malicious application could misuse permissions that were granted to it.

Therefore, users should:

- Review application permissions
- Avoid granting unnecessary permissions
- Install applications from trusted sources
- Remove permissions that are no longer needed

---

# 12. Trusted Application Sources

Applications should be installed from trusted sources.

A trusted application source can authenticate developers and verify applications through mechanisms such as developer certificates and application signing.

Application signing helps identify the developer and establish that an application is associated with a particular signing identity.

Installing applications from untrusted sources increases the risk of malware.

## Important Security Practices

- Use official application stores when possible.
- Verify the application developer.
- Avoid suspicious downloads.
- Review permissions.
- Keep applications updated.
- Be cautious with applications requesting unnecessary access.

---

# 13. Malware on Mobile Devices

Malware is malicious software designed to perform unauthorized or harmful actions.

Mobile devices can be affected by malware just like computers.

Possible malware risks include:

- Theft of information
- Unauthorized access
- Misuse of device resources
- Malicious network communication
- Transfer of malware to other devices

## Mobile Malware and Other Devices

Mobile devices may also transfer malicious software to connected computers.

For example, a malicious file stored on a mobile device could potentially be transferred to a laptop or desktop computer when the devices connect.

Mobile devices should therefore be treated as potential sources of malware when connecting them to other systems.

---

# 14. Antivirus Software

Antivirus applications are available for Android and iOS.

However, mobile operating systems impose restrictions that affect how antivirus applications operate.

## Android Antivirus

Depending on permissions and operating system restrictions, antivirus applications may not be able to automatically scan every file or perform scheduled scans.

Manual scans may be necessary.

## iOS Antivirus

iOS uses strict application isolation and security restrictions.

Traditional antivirus applications cannot freely scan the entire device or perform unrestricted automatic scanning.

This is part of the operating system's security design.

## Additional Security Features

Some security applications may provide:

- Device location
- Remote locking
- Remote wiping
- Security notifications
- Manual file scanning

---

# 15. Mobile Device Firewalls

A firewall monitors and controls network traffic.

Mobile firewall applications may be used to monitor application activity and restrict network connections.

Depending on the firewall, it may allow users to control connections involving:

- Specific applications
- IP addresses
- Ports

## Firewall Permissions

Firewalls may require elevated permissions because they need to monitor or control network activity.

Some mobile firewall applications without root access use a VPN interface to control network traffic.

This does not necessarily mean that the user is connected to a commercial VPN service.

Instead, the application may use the operating system's VPN functionality to inspect or control connections.

---

# 16. Operating System Updates and Patches

Operating system updates and patches are important for both functionality and security.

Updates can:

- Add new features
- Improve performance
- Fix bugs
- Improve compatibility
- Fix security vulnerabilities
- Improve hardware and software support

## Android Updates

Android updates can vary between devices because Android is used by many manufacturers.

Updates may depend on:

- Device manufacturer
- Device model
- Hardware requirements
- Carrier
- Android version

Older devices may not be able to install newer operating system versions because they do not meet the required hardware specifications.

Some older devices may continue receiving security patches without receiving major operating system upgrades.

## iOS Updates

iOS updates are delivered through Apple's update system.

Devices that do not meet the required hardware specifications may not support newer versions of iOS.

Users can check for updates through the device's settings.

Typical iPhone update path:

`Settings → General → Software Update`

---

# 17. Baseband Updates

Mobile devices also use radio firmware for cellular communication.

The course covered two important baseband-related configuration items:

| Component | Purpose |
|---|---|
| PRL | Preferred Roaming List |
| PRI | Primary Rate ISDN |

## Preferred Roaming List (PRL)

The PRL contains information that helps a mobile device identify and communicate with supported networks, particularly when roaming outside its primary carrier network.

## Primary Rate ISDN (PRI)

PRI configuration information relates to cellular communication parameters and data rates between the device and cellular network infrastructure.

Baseband-related updates can help a device maintain proper cellular communication.

---

# 18. Rooting and Jailbreaking

Rooting and jailbreaking are methods of removing restrictions imposed by a mobile operating system.

They allow users to gain additional privileged access to the device.

## Rooting

Rooting is commonly associated with Android devices.

It allows the user to obtain root-level privileges.

Root access can allow:

- Greater customization
- Modification of system files
- Installation of software normally restricted
- Access to protected system areas

## Jailbreaking

Jailbreaking is commonly associated with iOS devices.

It removes or bypasses certain restrictions imposed by Apple.

It may allow users to:

- Install software from alternative sources
- Modify system behavior
- Access restricted parts of the filesystem
- Run software that would normally be restricted

## Risks of Rooting and Jailbreaking

Rooting or jailbreaking can:

- Reduce built-in security protections
- Increase exposure to malware
- Allow applications greater access
- Cause stability problems
- Affect system updates
- Potentially void the manufacturer's warranty

Removing operating system restrictions can increase flexibility, but it also reduces some of the protections designed to keep the device secure.

---

# 19. Mobile Device Security Best Practices

Important security practices include:

- Keep the operating system updated.
- Install applications from trusted sources.
- Review application permissions.
- Use a secure screen lock.
- Avoid suspicious links and downloads.
- Be cautious when connecting mobile devices to computers.
- Use trusted Wi-Fi networks.
- Avoid unnecessary rooting or jailbreaking.
- Use security features such as remote lock and remote wipe when available.
- Remove applications that are no longer needed.
- Do not grant applications unnecessary access to sensitive resources.

---

# 20. Important Concepts

| Concept | Description |
|---|---|
| Android | Linux-based mobile operating system |
| iOS | Apple's mobile operating system |
| Open source | Source code is available for inspection and potentially modification |
| Closed source | Source code is not publicly available |
| GUI | Graphical user interface |
| Sandbox | Isolated environment in which applications run |
| Permissions | Controls access to device resources |
| Application signing | Helps identify and authenticate an application developer |
| Malware | Malicious software |
| Antivirus | Software used to detect or help protect against malicious software |
| Firewall | Controls or monitors network traffic |
| Patch | Update that fixes problems, including security vulnerabilities |
| Rooting | Obtaining privileged root access on Android |
| Jailbreaking | Removing or bypassing restrictions on iOS |
| PRL | Preferred Roaming List |
| PRI | Primary Rate ISDN |
| Android Auto | Android smartphone integration with supported vehicles |
| Apple CarPlay | iPhone integration with supported vehicles |

---

# Key Takeaways

- Android is a Linux-based mobile operating system.
- Android contains open-source components and is highly customizable.
- iOS is Apple's closed-source mobile operating system.
- Mobile operating systems use touchscreen interfaces.
- Android and iOS have different home screen and navigation designs.
- Mobile devices include features such as navigation, cameras, wireless connectivity, and voice assistants.
- Applications run in sandboxes to isolate them from other applications.
- Application permissions control access to sensitive resources.
- Applications should be installed from trusted sources.
- Mobile devices can be vulnerable to malware and can potentially transfer malicious files to other devices.
- Mobile antivirus capabilities are limited by operating system security restrictions.
- Mobile firewalls can monitor and control network connections.
- Updates and patches improve functionality, compatibility, and security.
- Rooting and jailbreaking remove operating system restrictions and can reduce security.
- Mobile device security depends on both operating system protections and responsible user behavior.

---

## Module Completion

**Course:** Cisco Networking Academy – Operating Systems Basics  
**Module:** 4 – Mobile Operating Systems and Security  
**Status:** Completed

This module improved my understanding of Android and iOS, mobile interfaces, common mobile features, application security, permissions, sandboxing, updates, malware protection, and mobile operating system security.

## Operating Systems Basics – Course Completion

With the completion of this module, I have completed all modules of Cisco Networking Academy's **Operating Systems Basics** course.

Topics covered throughout the course included:

- Windows operating systems
- Linux operating systems
- Operating system architecture
- System administration
- Processes and services
- Filesystems
- Command-line interfaces
- Mobile operating systems
- Mobile connectivity
- Mobile device security
- Application security
- System updates and troubleshooting
