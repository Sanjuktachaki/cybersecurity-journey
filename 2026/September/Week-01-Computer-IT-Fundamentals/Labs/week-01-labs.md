**# Week 1 — Practical Labs**



\## Objective



**To reinforce the computer and IT fundamentals studied during Week 1 through practical work.**



\## Lab 1 — Computer Boot Process



\### What I did?

I entered my computer’s **BIOS/UEFI settings** by pressing the **F2 key** during startup. I checked the available system information, including the BIOS mode, operating system, processor, system type, and physical memory.



\### What I observed?

I observed that the BIOS/UEFI provides important information about the **hardware and system configuration** before the operating system starts. I was able to identify my system’s **UEFI mode, OS details, processor, and installed memory**.



\### What I learnt?

I learned how to access the BIOS/UEFI settings and where to find basic information about my computer’s **hardware and operating system configuration.**



\### Security Relevance

Understanding the **normal system environment and configuration** is important in blue-team/defensive security. It helps establish a baseline, which can later be used to notice **unusual system changes, malware activity, resource abuse, or possible security exposure**.





\## Lab 2 — Programs, Processes, and Services



\### What I did?

I opened **Notepad** and checked it in **Task Manager → Processes**. I noted its process information and then closed Notepad to see what happened. I also checked its **PID** and recorded the CPU and memory usage. I opened applications such as **Chrome and File Explorer** to observe their resource usage. Finally, I went to **Task Manager → Services** and compared a service with a running process.



\### What I observed?

I observed that when I open a program, it appears as a **running process**, and when I close it, the process disappears. I also noticed that the **PID changes** when I close and reopen the same application, showing that it identifies a particular running instance. CPU, memory, disk and network usage also **change depending on what the applications are doing**. In Services, I saw the service name, status and description, which is different from the resource information shown for processes.



\### What I learnt?

I learned the difference between a **program, process and service**. A program is stored on the computer, while a process is created when that program is running. A **PID identifies a specific running process**, rather than permanently identifying the program. I also learned that services are mainly designed to **run in the background** and that resource usage naturally changes while using different applications.



\### Security Relevance

Understanding normal **processes, PIDs, resource usage and services** helps in monitoring a system and spotting unusual behavior. In security investigations, this knowledge can help identify **suspicious processes, unexpected resource usage or unusual services**, and can provide useful information when tracking and investigating potentially malicious activity.



\## Lab 3 — File Systems \& Folders \& File permissions



\### What I did?

I opened **File Explorer → This PC → Local Disk (C:)** and explored the main folders and directories. I then created my own folder structure for my **Cybersecurity Journey**, including folders for the year, September, Week 1 and Notes, and created a **Week 01 Notes.md** file. I also checked the file properties to view its type, location, size, and created/modified details. Finally, I opened the file's **Properties → Security** section to check the users/groups and their permissions.



\### What I observed?

I observed that the **C: drive contains important system and user directories**, such as Windows, Users and Program Files. I also saw that files have their own information, including **location, size, type and timestamps**. In the Security section, I found different users/groups with permissions such as **Full Control, Modify, Read \& Execute, Read and Write**.



\### What I learnt?

I learned how files and folders are **organized within the Windows file system** and how to create and manage my own directory structure. I also learned that file permissions control **what different users or groups are allowed to do** with a file.



\### Security Relevance

Understanding the **file system, file properties and permissions** is important for security investigations. It can help in **detecting unauthorized changes, identifying suspicious files or activity, and investigating incidents through file locations, timestamps and access permissions**.



\## Overall Lab Reflection



After doing the practicals, the theory became much clearer to me. I could actually see **how the system starts, how programs run as processes, how resources and services behave, and how files and permissions are organized**. It helped me connect the concepts I studied with what actually happens on a real computer.

