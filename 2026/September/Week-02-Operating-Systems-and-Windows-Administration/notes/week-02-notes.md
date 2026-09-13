# Week 2 — Operating Systems and Windows Administration

**Learning period:** September 2026  
**Focus:** Operating systems, Linux commands, macOS, Windows administration, Windows services, Event Viewer, and troubleshooting



## 1\. Operating System Overview

I revised the operating system fundamentals covered previously and connected them with the practical administration work completed during Week 2.

### Operating System

An operating system is the main system software that manages computer hardware and provides services and an environment for applications to run.

The operating system manages resources such as:

* CPU
* Memory
* Storage
* Files and directories
* Processes
* Users
* Permissions
* Devices
* System services



### Kernel

The kernel is the core component of an operating system.

It operates between hardware and higher-level software and is responsible for important system functions such as resource management, process management, memory management, and communication with hardware.



### User Space

User space is the area in which normal applications and user-level processes operate.

Applications generally do not directly control hardware. They request operating-system services through appropriate system interfaces.



### Kernel Space and User Space

The separation between kernel space and user space helps protect the core operating system from ordinary application processes.

This separation is important for system stability and security because a problem in a normal application should not automatically give that application unrestricted control over the operating system.



## 2\. Linux

I completed the Linux portion of the operating-system learning and practiced Linux commands.

For convenience, I divided the commands into two parts:

* Linux Commands — Part 1
* Linux Commands — Part 2

The practical work helped me become more comfortable working with the Linux command line and understanding how commands can be used to inspect and interact with the operating system.

The Linux command practice is documented separately in my study material and is part of my progression toward using Linux for cybersecurity and security-analysis work.



## 3\. Windows

I had already studied the Windows operating system previously, so Week 2 was not a first introduction to Windows.

During this week, I revised and applied Windows administration concepts, with particular focus on services, administrative tools, and troubleshooting.



## 4\. macOS

I studied the macOS operating system as part of the operating-system comparison and administration learning.

This helped broaden my understanding beyond Windows and Linux and reinforced the idea that operating systems provide similar fundamental functions while differing in their architecture, administration tools, interfaces, and system-management approaches.



## 5\. Windows Services

A major focus of Week 2 was Windows services.

Windows services are background processes that provide system or application functionality and can operate without requiring a user to interact with them directly.



### Service Control Manager (SCM)

I learned about the Service Control Manager (SCM), which is responsible for managing Windows services.

The Service Control Manager handles important service-management operations such as starting, stopping, and controlling services.

### Service Startup

I studied how Windows services can be configured to start and how their startup behavior affects the operating system.

I also learned how service configuration can be inspected through the Windows service-management interface.

### Services Console

I worked with the Windows Services console to understand how services can be viewed and managed.

The Services console allows an administrator to inspect information about services and perform management actions such as starting, stopping, restarting, and examining service configuration.



## 6\. Windows Event Viewer

I learned about Windows Event Viewer and its role in system administration and troubleshooting.

Event Viewer provides access to Windows event logs that record information about activities and events occurring within the operating system.

These logs can be useful when investigating:

* System problems
* Application problems
* Service-related issues
* Warnings
* Errors
* Other recorded system events

From a cybersecurity perspective, event logs are also important because system activity can provide information that helps an analyst understand what happened on a Windows system.



## 7\. Windows Administrative Tools and Troubleshooting

I learned that Windows administrative tools can be used together rather than treating each tool as an isolated utility.

During the practical troubleshooting work, I used:

* Task Manager
* Services
* Event Viewer

These tools provide different types of information.

### Task Manager

Task Manager can be used to inspect running processes and system activity.

### Services

The Services interface can be used to inspect and manage Windows services.

### Event Viewer

Event Viewer can be used to inspect recorded Windows events and investigate errors, warnings, and other system activity.

Using these tools together provides a more structured approach to troubleshooting.



## 8\. Week 2 Practical Work

I completed two Windows administration labs during Week 2.

### Lab 1 — Understanding How Windows Services Are Viewed and Managed

The purpose of this lab was to understand how Windows services are viewed and managed.

I used the Windows Services interface to inspect services and worked through the service-management tasks required by the lab.

The lab helped connect the theoretical concepts of Windows services and the Service Control Manager with actual Windows administration.

### Lab 2 — Using Windows Administrative Tools Together During Troubleshooting

The purpose of this lab was to learn how Windows administrative tools can be used together during troubleshooting.

The tools used were:

* Task Manager
* Services
* Event Viewer

I completed the practical troubleshooting activities and recorded the observations and results in my lab documentation.

This lab demonstrated how information from different Windows administrative tools can be combined to investigate a system problem rather than relying on a single source of information.



## 9\. Cybersecurity Relevance

Understanding operating systems is important for cybersecurity because security analysts investigate activity that occurs inside operating-system environments.

Knowledge of processes, services, users, permissions, system events, and administrative tools provides a foundation for later security work involving:

* Windows event logs
* SIEM investigation
* Incident response
* Endpoint security
* Detection and analysis
* Threat hunting
* System troubleshooting

The Windows administration labs were particularly relevant because they introduced practical use of tools that can later support security investigations.



## 10\. What I Completed in Week 2

During Week 2, I completed:

* Operating-system revision
* Kernel and user-space concepts
* Linux learning and command practice
* Linux Commands Part 1
* Linux Commands Part 2
* Windows revision
* macOS learning
* Windows services
* Service Control Manager (SCM)
* Windows service startup concepts
* Windows Services console
* Windows Event Viewer
* Windows administrative tools
* Task Manager
* Services
* Event Viewer
* Windows services management lab
* Windows administrative-tools troubleshooting lab



## 11\. Week 2 Takeaway

This week strengthened my understanding of operating systems from both a conceptual and practical perspective.

I moved beyond simply understanding what an operating system does and worked with Windows administrative tools to inspect services, events, processes, and system activity.

The practical work also showed how different administrative tools can be combined during troubleshooting. This provides useful groundwork for later cybersecurity topics involving Windows logs, endpoint activity, SIEM analysis, and incident investigation.

