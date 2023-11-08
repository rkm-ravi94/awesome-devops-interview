**Question: What is Linux?**<br>
**Explanation:**  Linux is like the engine of a car. It's the core software that makes your computer run. Just like different cars have different features, there are different versions of Linux that look and feel different but still use the same engine underneath. <br>
**Technical Answer:**  Linux is a free and open-source Unix-like operating system kernel. It's the core software that manages hardware resources and provides services for computer programs. Multiple Linux distributions (distros) exist, such as Ubuntu, Fedora, and Debian, providing different user experiences built on top of the Linux kernel.
<br>

**Question: What is the difference between Linux and Unix?**<br>
**Explanation:**  Imagine two cousins who grew up together but chose different paths in life. Unix is the older cousin who went the corporate route, while Linux is the younger one who decided to share his talents with everyone for free. They have a lot in common but also some distinct differences.<br>
**Technical Answer:**  Unix is a proprietary operating system originally developed in the 1960s. It's known for its stability, multi-user capabilities, and security. Linux, on the other hand, is free and open-source, inspired by Unix but not derived from it. Linux provides similar functionality to Unix but with greater flexibility and availability across various hardware platforms.
<br>

**Question: What is a Linux distribution (distro)?**<br>
**Explanation:**  If Linux is the engine, a Linux distribution is the whole car. It's a version of Linux that comes with its own style, features, and additional tools, like a GPS or sunroof, to make your driving experience unique.<br>
**Technical Answer:** A Linux distribution is a complete operating system built around the Linux kernel. It includes the kernel itself, system libraries, user applications, and a package management system. Each distro tailors these components to specific use-cases, user preferences, or system requirements, leading to a wide variety of distributions like Ubuntu, CentOS, and Arch Linux.
<br>

**Question: What is a Stateless Linux Server?**<br>
**Explanation:** A stateless Linux server is like a sketchpad that erases itself after each drawing. It doesn't remember anything from one session to the next.<br>
**Technical Answer:** A stateless Linux server does not store any session information about its clients. Each client interaction is processed independently without relying on information from previous interactions.
<br>

**Question: Explain the features of Stateless Linux Server?**<br>
**Explanation:** Features of a stateless server include not needing to remember past interactions, making it easier to manage, more secure, and better at handling lots of traffic.<br>
**Technical Answer:** Features include reduced complexity as no state is maintained, increased security as no sensitive data is stored, better scalability, and potential for load balancing.
<br>

**Question: Explain Linux Boot Process.**<br>
**Technical Answer:** <br>
1. The machine’s BIOS (Basic Input/Output System) or boot microcode hundreds and runs a boot loader.
2. Boot loader finds the kernel image on the disk and loads it into memory, to start the system.
3. The kernel initializes the devices and their drivers.
4. The kernel mounts the basis filesystem.
5. The kernel starts a program referred to as init with a method ID zero
6. init sets the remainder of the system processes in motion.
7. For some purpose, init starts a method permitting you to log in, typically at the top or close to the top of the boot sequence.
8. system startup BIOS -> MBR Boot Loader -> GRUB -> RUNLEVEL -> INIT
<br>

**Question:  How do you troubleshoot a Linux OS that fails to boot?**<br>
**Explanation:** Troubleshooting a Linux OS that fails to boot is like being a detective trying to figure out why a car won't start. You check the battery, the fuel, the engine, and other parts to find the problem.<br>
**Technical Answer:** Troubleshooting a Linux OS that fails to boot involves checking various components such as the bootloader (GRUB), kernel, initramfs, and system files. Using recovery mode or a live CD to access the system, examining log files like /var/log/syslog or /var/log/dmesg, and checking file system integrity with fsck are part of the process. Resolving issues with bootloaders, repairing broken packages, and ensuring correct kernel parameters are also crucial steps.
<br>

**Question: What is a Boot Loader ?**<br>
**Technical Answer:** Boot Loader is a software program that is responsible for “actually loading” the operating system once the Boot Manager has finished its work. And by loading Operating System we mean “loading the kernel of the Operating System”.  The Boot Loader is typically a part of the Operating System itself. Till the point Boot Loader starts loading the OS, there is nothing in the Main Memory of the machine.
Following are a series of tasks that a typical Boot Loader is expected to perform:
    1. Loading and parsing the Boot Configuration File.
    2. Loading and initializing the OS’s kernel into the main memory.
    3. Loading and initializing the other system components and system drivers.
    4. Finally, finish up the system environment setup and transfer the control to the kernel.
<br>

**Question: What is a kernel ?**<br>
**Explanation:** Consider any school with no teacher in it. How will the situations be in such schools? As you can imagine the consequences with not much effort, the similar output will be found if an Operating system does not include a Kernel in it. Without a kernel, you can't have an Operating System that actually works. All the Operating System's like Windows, Mac OS X, and Linux have different kernels in it. Kernel acts as a central component of any Operating System, similar to nucleus of any cell.<br>
**Technical Answer:** Kernel handles the complicated job of managing the resources efficiently. It should keep checking the availability of memory in your system and place the required applications in the proper memory location. It is also responsible for completing any internal task quickly by optimizing the usage of the processor and preventing the deadlocks. There are three types of kernels, Monolythic, Micro and Hybrid.
<br>

**Question: What are kernel modules ?**<br>
**Technical Answer:** A kernel module is a piece of software whose aim is to extend the Linux kernel with a new feature. A kernel module can be a device driver, in which case it would control and manage a particular hardware device, hence the name device driver. A module can also add a framework support (for example IIO, the Industrial Input Output framework), extend an existing framework, or even a new filesystem or an extension of it. The thing to keep in mind is that kernel modules are not always device drivers, whereas device drivers are always kernel modules.
<br>

**Question: Where are the kernel modules located?**<br>
**Explanation:** Kernel modules are like add-on parts for a car stored in a specific garage. You can add them to the car to give it new features or improve its performance.<br>
**Technical Answer:**  Kernel modules are typically located in /lib/modules/$(uname -r) directory. They are loadable kernel modules that can be loaded or unloaded from the kernel as needed.
<br>

**Question: First process started by the kernel in Linux and its process id ?**<br>
**Explanation:** The first process is like the first employee to arrive and open the office in the morning. Its job is to get everything ready for the other employees. Its ID badge is always number 1.<br>
**Technical Answer:** The first process started by the Linux kernel is init (or systemd in some distributions), and its process ID (PID) is always 1.
<br>

**Question: What are runlevels in Linux?**<br>
**Explanation:** Runlevels in Linux are like different gears in a car. Each gear (or runlevel) tells your computer to run in a different way. Some gears are for troubleshooting, some are for normal use, and others are for shutting down or rebooting.<br>
**Technical Answer:** Runlevels are predefined modes of operation in Unix-based systems. Each runlevel represents a different state of the system and dictates which services or processes should be running. For example, runlevel 3 might be multi-user text mode, while runlevel 5 is multi-user graphical mode. The concept of runlevels is often used in the SysV init system.
<br>

**Question: What is a shell?**<br>
**Explanation:** A shell is like a translator between you and your computer. You tell it what you want in a language you both understand, and the shell makes sure the computer knows what to do.<br>
**Technical Answer:** A shell is a command-line interpreter that provides a user interface for accessing an operating system's services. It interprets user commands and translates them into actions the operating system can perform. There are various shells available in Linux, such as Bash, Zsh, and Tcsh, each with its own features and syntax.
<br>

**Question: How many types of Shells are there in Linux?**<br>
**Explanation:** Just like there are different languages people can speak, there are different types of shells, or "languages," your computer can understand and respond to.<br>
**Technical Answer:**  There are several types of shells in Linux, including the Bourne Shell (sh), the C Shell (csh), the Korn Shell (ksh), the Bourne Again Shell (bash), and the Z Shell (zsh).
<br>

**Question: What is the command line?**<br>
**Explanation:** The command line is like a chat window with your computer. You type in commands, and the computer does what you ask. It's a powerful way to communicate directly with your computer without using a mouse.<br>
**Technical Answer:** The command line, or terminal, is a text-based interface used to interact with the operating system. Users enter commands as text, and the operating system executes them. It's a powerful tool that allows for complex operations, scripting, and direct access to system functions.
<br>

**Question: Explain LILO.**<br>
**Explanation:**  LILO is like a traffic cop at a crossroad, deciding which operating system to boot when you start your computer.<br>
**Technical Answer:**  LILO (Linux Loader) is a boot loader for Linux. It's responsible for loading the Linux kernel into memory and initiating the boot process.
<br>

**Question: What is the init process in Linux?**<br>
**Explanation:** The init process in Linux is like the master switch that turns everything on when you start your computer. It's the first thing that runs and sets up everything else you need.<br>
**Technical Answer:** The init process is the first process started by the Linux kernel and has a process ID (PID) of 1. It is responsible for starting and managing all other processes on the system, either directly or by delegating to other process managers. In modern systems, traditional init has been replaced by systems like systemd or Upstart, providing more features and better handling of dependencies.
<br>

**Question: What do you understand about the standard streams?**<br>
**Explanation:** Standard streams are like pipes in your house. One brings in fresh water (input), one drains away dirty water (output), and one handles unexpected leaks (errors).<br>
**Technical Answer:** Standard streams are pre-established communication channels between a program and its environment: standard input (stdin), standard output (stdout), and standard error (stderr).
<br>

**Question: What is the difference between a process and a thread?**<br>
**Explanation:** A process is like a worker in an office doing a job, while a thread is a specific task the worker performs. Multiple threads mean the worker is multitasking.<br>
**Technical Answer:** A process is an instance of a program in execution. It's an independent unit with its own address space. A thread, however, is the smallest unit of processing and executes within the context of a process. Threads in the same process share resources and address space.
<br>

**Question: What is the difference between a process and a daemon in Linux?**<br>
**Explanation:** A process is like a worker in an office doing a specific task, while a daemon is like the janitor working in the background, keeping everything running smoothly without much interaction.<br>
**Technical Answer:** A process is an instance of a running program that performs a specific task or set of tasks. A daemon is a special type of process that runs in the background, often initiated at system startup, and does not interact with users directly. Daemons provide various services to the system and other processes.
<br>

**Question: Explain Process Management System Calls in Linux?**<br>
**Explanation:** Process management system calls are like the commands a manager gives to start, stop, or manage different tasks and workers in an office.<br>
**Technical Answer:** Process management system calls in Linux include fork() for creating a new process, exit() for terminating a process, wait() for making a process wait until its child processes finish, and exec() for replacing the process memory space with a new program.
<br>

**Question: What do you mean by a Process States in Linux?**<br>
**Explanation:** Process states are like different moods for your computer's tasks. Some tasks are active and running, some are waiting in line, some are sleeping, and others have finished their job or are stopped.<br>
**Technical Answer:** In Linux, a process can be in one of several states, including:
Running: The process is either running or ready to run.
Interruptible Sleep: The process is sleeping, waiting for some condition to be met or event to happen.
Uninterruptible Sleep: The process is sleeping, but cannot be woken up until a specific event occurs.
Stopped: The process has been stopped, usually by a signal.
Zombie: The process has completed, but still has an entry in the process table to report its exit status to its parent process.
<br>

**Question: what is a Zombie Process ?**<br>
**Explanation:** A zombie process is like a finished task that's still hanging around on your to-do list. It's done its job, but it's still there taking up space until you cross it off the list.<br>
**Technical Answer:** A zombie process is a process that has completed execution but still has an entry in the process table. It occurs when a parent process fails to call wait() to retrieve its child's exit status, leaving the terminated child process in a "defunct" state.
<br>

**Question: What is an Orphan Process ?**<br>
**Technical Answer**: Orphan processes are those processes that are still running even though their parent process has terminated or finished. A process can be orphaned intentionally or unintentionally.
An intentionally orphaned process runs in the background without any manual support. This is usually done to start an indefinitely running service or to complete a long-running job without user attention.
An unintentionally orphaned process is created when its parent process crashes or terminates. Unintentional orphan processes can be avoided using the process group mechanism.
<br>

**Question: Describe how a parent and child process communicates with each other?**<br>
**Explanation:** It's like a parent and child talking through a walkie-talkie. They can send messages back and forth to each other.<br>
**Technical Answer:** A parent and child process can communicate with each other through various forms of inter-process communication (IPC), such as pipes, signals, message queues, shared memory, or semaphores.
<br>

**Question: What do you understand about process scheduling in Linux?**<br>
**Explanation:** Process scheduling in Linux is like a juggler keeping several balls in the air. The system has to manage multiple tasks at once, deciding which ones get attention and in what order to keep everything running smoothly.<br>
**Technical Answer:** Process scheduling in Linux is handled by the kernel, which uses scheduling algorithms to determine the order and amount of CPU time allocated to each process. Common scheduling algorithms include Completely Fair Scheduler (CFS) for general-purpose tasks, and Real-Time Scheduling for time-critical tasks. The scheduler ensures efficient CPU utilization and responsive multitasking.
<br>

**Question: How do you list all the processes running in Linux?**<br>
**Explanation:** Listing all processes is like taking a roll call to see who's currently doing something on your computer.<br>
**Technical Answer:** The `ps` command lists currently running processes. Using options like ps aux provides more detailed information.
<br>

**Question: How do you find the process ID (PID) of a running process?**<br>
**Explanation:** Finding the PID of a running process is like looking up a person's ID number. It's a unique number that identifies what's running on your computer.<br>
**Technical Answer:** The ps command can display the PID alongside other process information. Additionally, pidof can be used to find the PID of a specific process by name.
<br>

**Question: What is the /proc file system?**<br>
**Explanation:** The /proc filesystem is like a real-time bulletin board that displays information about your computer's current state, like what's running and how resources are being used.<br>
**Technical Answer:** The /proc filesystem is a pseudo-filesystem that provides an interface to kernel data structures. It's used to access information about the system and running processes.
These answers should provide a comprehensive understanding of these Linux concepts and **Questions in both simple and technical language.
<br>

**Question: How do you kill the program using one port in Linux?**<br>
**Explanation:** Imagine you have a pipe, and water is flowing through it. But you want to use this pipe for something else. First, you need to stop the water (or program) that's currently using it. In the computer world, you can find out which program is using the pipe (or port) and ask it nicely to stop, so you can use the port for something else.<br>
**Technical Answer:** In Linux, every network service listens on a port. If you want to stop a service (or kill a process) that's using a specific port, you first need to find the process ID (PID) that's associated with that port. This can be done using the netstat or lsof command. Once you have the PID, you can use the kill command to terminate the process.
Example: `sudo kill $(sudo lsof -t -i:<port_number>)`
<br>

**Question: How do you schedule recurring tasks in Linux?**<br>
**Explanation:** Scheduling recurring tasks in Linux is like setting up automatic reminders or alarms. You tell the computer when and what you want to be done regularly, and it takes care of it for you.<br>
**Technical Answer:** Recurring tasks in Linux can be scheduled using cron jobs. Cron is a time-based job scheduler that runs commands at specified intervals. Users can add entries to their crontab file using the crontab -e command, specifying the schedule and command to run.
<br>

**Question: Difference between cron and anacron**<br>
**Explanation:** Cron is like setting a regular alarm clock that rings at the same time every day, even if you're not home. Anacron is more like a reminder system that'll make sure to remind you about something even if you missed the initial reminder.<br>
**Technical Answer:** Cron is a time-based job scheduler that runs tasks at specified intervals. Anacron is similar but is used primarily for tasks that don't necessarily need to run at an exact time. Anacron can run missed tasks once the system is up.
<br>

**Question: What are some common Linux commands?**<br>
**Explanation:** Think of Linux commands as basic instructions you can give to your computer, like "show me what's inside this folder" or "make a copy of this file." They're simple phrases that help you navigate and manage your files.<br>
**Technical Answer:** Some common Linux commands include:
ls: Lists directory contents.
cd: Changes the current directory.
cp: Copies files or directories.
mv: Moves or renames files or directories.
rm: Removes files or directories.
pwd: Prints the current working directory.
grep: Searches for patterns within files.
chmod: Changes file permissions.
sudo: Executes a command with superuser privileges.
<br>

**Question: How do you check the status of a service or daemon in Linux?**<br>
**Explanation:** Checking the status of a service or daemon in Linux is like checking if a store is open or closed. You use a specific command to see if the service is running, stopped, or experiencing problems.<br>
**Technical Answer:** You can check the status of a service or daemon in Linux using the systemctl status <service_name> command if the system uses systemd, or the /etc/init.d/<service_name> status command for systems using the init system. This will provide information on whether the service is active, inactive, or has failed.
<br>

**Question: INODE and Process Id**<br>
**Explanation:** An INODE is like a detailed index card in a library that contains all the information about a book except its name. A Process ID is like a unique ID badge for every employee in a large office, so everyone knows who's who.<br>
**Technical Answer:** An INODE is a data structure on a filesystem that stores all the information about a file except its name and actual data. 
<br>

**Question: What is a root user?**<br>
**Explanation:** The root user is like the master key to your computer. It has the power to open every door and change anything. Because it's so powerful, you should use it carefully to avoid any accidental damage.<br>
**Technical Answer:** The root user is the administrative user in a Linux environment with full access to all files and commands. The root user has the highest level of access, allowing them to perform any administrative tasks, modify system settings, and manage other user accounts. Due to its elevated privileges, it's recommended to use the root user sparingly and with caution.
<br>

**Question: How do you create a user account?**<br>
**Explanation:** Creating a user account is like setting up a new mailbox for someone. It gives them their own space to receive messages and store their things.<br>
**Technical Answer:** A user account is created using the useradd command, followed by the username. Additional options can set a password, create a home directory, and more.
<br>

**Question: What is the difference between /etc/passwd and /etc/shadow files?**<br>
**Explanation:** The /etc/passwd and /etc/shadow files are like membership lists for a club. The /etc/passwd file is the public list that shows who's a member, while the /etc/shadow file is the private list that contains sensitive information like members' passwords.<br>
**Technical Answer:** The /etc/passwd file contains user account information, including usernames, user IDs, group IDs, home directories, and default shells. The /etc/shadow file contains the password information for the user accounts in a secure and encrypted format, along with password aging information.
<br>

**Question: What is the purpose of the sudoers file in Linux, and how do you configure sudo access for users?**<br>
**Explanation:** The sudoers file is like a VIP list at a club. It decides who gets special permissions to do things that regular users can't. You can add people to the list and specify exactly what they're allowed to do.<br>
**Technical Answer:** The sudoers file is a configuration file for the sudo command, which allows users to run programs with the security privileges of another user. By editing this file, you can specify which users or groups have permission to use sudo, and the commands for which they have privileges.
<br>

**Question:  Explain chown, chmod, chage commands**<br>
**Explanation:** These commands are like tools for managing who can access your files and what they can do with them. chown changes who owns the file, chmod changes what they can do with it (like read or write), and chage sets rules for how long a user's password will last.<br>
**Technical Answer:**
chown: Changes the owner of a file or directory.
chmod: Changes the file mode bits of a file or directory (permissions).
chage: Changes user password expiry information, managing the aging of passwords.
<br>

**Question: How to lock a user account in Linux?**<br>
**Explanation:** Locking a user account is like taking away someone's keycard so they can't enter a building.<br>
**Technical Answer:** A user account can be locked using the passwd -l command, which disables the password by prefixing it with a special character.
<br>

**Question: What is umask?**<br>
**Explanation:** umask is like setting default privacy settings for your files. When you create a new file, umask decides who can read, write, or execute that file by default.<br>
**Technical Answer:** umask, or user file-creation mode mask, is a default value that determines the permissions that are set for newly created files and directories. It's a way of setting default access rights so that when a user creates a file, it doesn't have more permissions than intended.
<br>

**Question: Elaborate all the file permissions in Linux.**<br>
**Explanation:** File permissions in Linux are like rules at a private club. They decide who can come in (read), who can change things (write), and who can run activities or programs (execute).<br>
**Technical Answer:** Linux file permissions are based on three types: read (r), write (w), and execute (x). These permissions can be set for three categories of users: the file owner, the group to which the file belongs, and others. Using the chmod command, you can modify these permissions.
<br>

**Question: What is the chmod command in Linux, and how do you use it?**<br>
**Explanation:** The chmod command is like changing the locks on your doors. It controls who can come in (read), rearrange furniture (write), or throw a party (execute).<br>
**Technical Answer:** The chmod command changes the file's mode (permissions). It can be used in numerical form (e.g., chmod 755 filename) or symbolic form (e.g., chmod u+x filename) to modify the file permissions.
<br>

**Question: How to check the default route and routing table?**<br>
**Explanation:** Checking the default route and routing table is like looking at a map to see which highways your car will take by default to get out of your town, and seeing all the other possible routes it can take.<br>
**Technical Answer:** The route or ip route command can be used to check the default route and routing table. It shows the IP routing table which is a set of rules that determines where network traffic will be directed.
<br>

**Question: How do you troubleshoot network connectivity issues in Linux?**<br>
**Explanation:** Troubleshooting network issues is like solving a mystery of why your letter didn't reach its destination. You check each step of the journey to find where it got lost.<br>
**Technical Answer:** Troubleshooting involves checking the network configuration, using commands like ping, traceroute, ifconfig/ip, and examining firewall settings to isolate the connectivity problem.
<br>

**Question: What is SMTP?**<br>
**Explanation:** SMTP is like the postal service for emails. It's the set of rules that allows your email to be sent from your computer to someone else's, wherever they are in the world.<br>
**Technical Answer:** Simple Mail Transfer Protocol (SMTP) is an Internet standard communication protocol for electronic mail transmission. Mail servers and other message transfer agents use SMTP to send and receive mail messages. Client email software typically uses SMTP only for sending messages to a mail server for relaying.
<br>

**Question: What is the difference between UDP and TCP?**<br>
Answer: UDP and TCP are like two different ways of sending mail. UDP is like sending a postcard: it's fast, but there's no guarantee it'll arrive, and there's no way to know if it gets lost. TCP is like sending a registered letter: it's a bit slower because you get a receipt and confirmation of delivery.
<br>

**Question: What is network bonding in Linux?**<br>
**Explanation:** Network bonding is like combining multiple internet cables into one. By doing this, you can increase the speed and reliability of your internet connection.<br>
**Technical Answer:** Network bonding, also known as NIC teaming, involves combining multiple network interfaces into a single logical interface. This can provide increased bandwidth, load balancing, or fault tolerance by allowing traffic to be distributed or rerouted in case of a failure.
<br>

**Question: How do you set up a static IP address in Linux using the command-line interface?**<br>
**Explanation:** Setting up a static IP address is like picking a permanent parking spot for your car. Instead of moving around, your computer always 'parks' at the same address on the network.<br>
**Technical Answer:** To set up a static IP address, you need to edit the network configuration files or use network management commands like ifconfig or ip addr and specify the desired IP address, subnet mask, gateway, and DNS servers.
<br>

**Question: Different network bonding modes used in Linux**<br>
**Explanation:** Different bonding modes are like different strategies for a team of relay racers. Some modes are about speed, some are about reliability, and some are a mix of both.<br>
**Technical Answer:** Network bonding modes include balance-rr (round-robin), active-backup, balance-xor, broadcast, 802.3ad (LACP), balance-tlb (adaptive transmit load balancing), and balance-alb (adaptive load balancing).
<br>

**Questions: what are advantages of using NIC teaming**<br>
**Explanation:** NIC teaming is like having multiple internet connections to your home. If one goes out, you still have internet, and when they're all working, you have a faster connection.<br>
**Technical Answer:** NIC teaming provides redundancy and load balancing for network interfaces. If one NIC fails, another can take over, ensuring network availability. It can also aggregate bandwidth, increasing the overall network throughput.
<br>

**Question: What is Port number of Ping**<br>
**Explanation:** Ping doesn't have a specific port number; it's like knocking on the door to see if anyone's home, rather than sending a letter to a specific mailbox.<br>
**Technical Answer:** Ping uses ICMP (Internet Control Message Protocol), which does not operate on a port level. It's part of the IP layer and is used to send error messages and operational information.
<br>

**Question: What is the iptables command, and how to use it for network filtering?**<br>
**Explanation:** The iptables command is like a security guard for your computer's network, deciding who gets in and who doesn't. You can set rules to allow or block traffic to keep your network secure.<br>
**Technical Answer:** iptables is a user-space utility program that allows a system administrator to configure the IP packet filter rules of the Linux kernel firewall. Rules can be set to filter traffic based on protocols, ports, source and destination IP addresses, and other criteria. iptables is often used to create complex network traffic filtering arrangements for security and network management.
<br>

**Question: What is pipe?**<br>
**Explanation:** A pipe is like a conveyor belt in a factory that takes the output of one machine and feeds it directly into the next machine.<br>
**Technical Answer:** A pipe is a form of redirection that is used in Linux and other Unix-like operating systems to send the output of one program to another program for further processing.
<br>

**Question: What is Swap Space?**<br>
**Explanation:** Swap space is like an overflow parking lot. When your computer's memory is full, it uses swap space to store extra information temporarily.<br>
**Technical Answer:** Swap space is a form of virtual memory. When the physical RAM is full, the operating system can move inactive pages to swap space to free up RAM for active processes.
<br>

**Question:  What is the difference between hard links and soft links?**<br>
**Explanation:** Imagine two shortcuts to your house. A hard link is a direct shortcut, while a soft link is like a note telling you where to go. If your house moves, the direct shortcut won't work, but the note still tells you where to find it.<br>
**Technical Answer:** A hard link is a direct reference to the data on the disk, sharing the same inode as the original file. A soft link (symbolic link) is a separate file that points to the target file's path. If the original file is moved or deleted, the hard link remains valid, but the soft link breaks.
<br>

**Question: How do users create a symbolic link in Linux?**<br>
**Explanation:** Creating a symbolic link is like making a signpost that points to a specific place. You tell your computer where the sign should point, and it creates a shortcut for you.<br>
**Technical Answer:** Users create a symbolic link using the ln -s command, specifying the target file and the symbolic link name.
<br>

**Question: What is the ulimit command, and how do you use it?**<br>
**Explanation:** The ulimit command sets boundaries for how much of certain resources (like memory or file size) a process can use. It's like giving a child an allowance to control their spending.<br>
**Technical Answer:** ulimit sets user limits for system resources. It can limit file sizes, number of open files, and more. Usage includes ulimit [options] [limit].
<br>

**Question: How do you mount and unmount filesystems in Linux?**<br>
**Explanation:** Mounting a filesystem is like opening a book to read it. Unmounting is like closing the book when you're done.<br>
**Technical Answer:** Mounting a filesystem attaches it to a directory structure, making its contents accessible. The mount command is used for this purpose. Unmounting with the umount command detaches it, ensuring no further access.
<br>

**Question: How do you format a disk in Linux?**<br>
**Explanation:** Formatting a disk is like clearing out and rearranging a room to make it ready for a new purpose.<br>
**Technical Answer:** Formatting a disk involves creating a new filesystem on the disk. The mkfs command, followed by the type of filesystem and the device name, is used for this purpose.
<br>

**Question: How do you check the contents of a file without opening it in Linux?**<br>
**Explanation:** Checking the contents of a file without opening it is like peeking through a window to see what's inside a room. You can use special commands that let you quickly look at the beginning or end of a file without going through the whole thing.<br>
**Technical Answer:** You can use commands like cat, less, more, head, and tail to view the contents of a file in Linux. cat prints the entire file, less and more allow for scrollable viewing, while head and tail show the beginning and end of the file, respectively.
<br>

**Question:  What is RAID in Linux?**<br>
**Explanation:** RAID is like a team of hard drives working together to either improve performance or ensure your data is safe even if one drive fails.<br>
**Technical Answer:** RAID (Redundant Array of Independent Disks) is a way of storing data on multiple hard disks for redundancy or performance improvement. Linux supports various RAID levels, like RAID 0 (striping), RAID 1 (mirroring), and RAID 5 (parity).
<br>

**Question: Explain different types of Raids.**<br>
**Technical Answer:**
RAID 0, also known as a striped set or a striped volume, requires a minimum of two disks. The disks are merged into a single large volume where data is stored evenly across the number of disks in the array.
This process is called disk striping and involves splitting data into blocks and writing it simultaneously/sequentially on multiple disks. Configuring the striped disks as a single partition increases performance since multiple disks do reading and writing operations simultaneously. Therefore, RAID 0 is generally implemented to improve speed and efficiency.
RAID 1: is an array consisting of at least two disks where the same data is stored on each to ensure redundancy. The most common use of RAID 1 is setting up a mirrored pair consisting of two disks in which the contents of the first disk is mirrored in the second. This is why such a configuration is also called mirroring.
Unlike with RAID 0, where the focus is solely on speed and performance, the primary goal of RAID 1 is to provide redundancy. It eliminates the possibility of data loss and downtime by replacing a failed drive with its replica.
RAID 2: is rarely used in practice today. It combines bit-level striping with error checking and information correction. This RAID implementation requires two groups of disks – one for writing the data and another for writing error correction codes. RAID 2 also requires a special controller for the synchronized spinning of all disks.
Instead of data blocks, RAID 2 stripes data at the bit level across multiple disks. Additionally, it uses the Humming error ode correction (ECC) and stores this information on the redundancy disk.
RAID 3: is rarely used in practice. This RAID implementation utilizes bit-level striping and a dedicated parity disk. Because of this, it requires at least three drives, where two are used for storing data strips, and one is used for parity.
To allow synchronized spinning, RAID 3 also needs a special controller. Due to its configuration and synchronized disk spinning, it achieves better performance rates with sequential operations than random read/write operations.
RAID 4: is another unpopular standard RAID level. It consists of block-level data striping across two or more independent diss and a dedicated parity disk.
The implementation requires at least three disks – two for storing data strips and one dedicated for storing parity and providing redundancy. As each disk is independent and there is no synchronized spinning, there is no need for a controller.
RAID 5: is considered the most secure and most common RAID implementation. It combines striping and parity to provide a fast and reliable setup. Such a configuration gives the user storage usability as with RAID 1 and the performance efficiency of RAID 0.
This RAID level consists of at least three hard drives (and at most, 16). Data is divided into data strips and distributed across different disks in the array. This allows for high performance rates due to fast read data transactions which can be done simultaneously by different drives in the array.
RAID 6: is an array similar to RAID 5 with an addition of its double parity feature. For this reason, it is also referred to as the double-parity RAID.
This setup requires a minimum of four drives. The setup resembles RAID 5 but includes two additional parity blocks distributed across the disk. Therefore, it uses block-level striping to distribute the data across the array and stores two parity blocks for each data block.
RAID 10: is part of a group called nested or hybrid RAID, which means it is a combination of two different RAID levels. In the case of RAID 10, the array combines level 1 mirroring and level 0 striping. This RAID array is also known as RAID 1+0.
RAID 10 uses logical mirroring to write the same data on two or more drives to provide redundancy. If one disk fails, there is a mirrored image of the data stored on another disk. Additionally, the array uses block-level striping to distribute chunks of data across different drives. This improves performance and read and write speed as the data is simultaneously accessed from multiple disks.
<br>

**Question: What is LVM in Linux?**<br>
**Explanation:** LVM in Linux is like having a flexible closet organizer. It lets you resize your storage spaces, move them around, or add new ones without having to throw everything out and start over.<br>
**Technical Answer:** Logical Volume Manager (LVM) is a device mapper framework that provides logical volume management for the Linux kernel. It allows for flexible disk space management by abstracting the physical storage into logical volumes, making it easier to resize and manage disk space without downtime.
<br>

**Question: How do you check disk space usage?**<br>
**Explanation**s: Checking disk space usage is like checking how full your storage unit is. It helps you decide if you need to clear out old things or get more space.<br>
**Technical Answer:** The df command reports file system disk space usage, and du provides the disk usage of files and directories.
<br>

**Question:  What is the rsync command, and how do you use this command for synchronization?**<br>
**Explanation:** The rsync command is like a moving truck that carefully packs and moves your stuff from one place to another, making sure nothing gets left behind.<br>
**Technical Answer:** rsync is used for fast and versatile file copying and synchronization. It can synchronize files between local directories, different hosts, or between a local machine and a remote host. Usage includes rsync options source destination.
<br>

**Question:  What is the difference between absolute and relative paths in Linux?**<br>
**Explanation:** Absolute and relative paths are like giving directions to your house. An absolute path is like giving someone your full address, while a relative path is like giving directions from where they are now (like saying "turn left at the next corner").<br>
**Technical Answer:** An absolute path is a complete path from the root of the file system to a specific file or directory, starting with a /. A relative path, on the other hand, is a path that is relative to the current directory, not starting with a /, and can use . for the current directory and .. for the parent directory.
<br>

**Question: How to copy a file to multiple directories in Linux?**<br>
**Explanation:** Copying a file to multiple directories is like handing out copies of a flyer to several different stores. You can use a special command that makes copies for each location all at once.<br>
**Technical Answer:** You can use a loop in conjunction with the cp command to copy a file to multiple directories. Alternatively, tools like rsync or shell features like brace expansion can be used to distribute a file across multiple destinations.
<br>

**Question: Purpose of /etc/resolv.conf and /etc/hosts files.**<br>
**Explanation:** The /etc/resolv.conf file is like an address book for your computer, telling it where to find websites by their names. The /etc/hosts file is like a list of shortcuts for your computer, letting it know where to find certain websites without having to look them up.<br>
**Technical Answer:** The /etc/resolv.conf file contains nameserver information used by the system for DNS resolution. The /etc/hosts file maps hostnames to IP addresses for small-scale or local hostname resolution.
<br>

**Question:  How do you limit memory usage for commands?**<br>
**Explanation:** Think of a command as a small robot that does a job for you on the computer. Sometimes, this robot can get greedy and use too much memory, causing problems for other robots. To prevent this, you can give the robot a rule when you start it, telling it to use only a certain amount of memory. This way, it won't be greedy and will leave enough memory for other robots to work properly.<br>
**Technical Answer:** In Linux, you can limit the memory usage of a command using the ulimit shell builtin or the cgroups (control groups) feature. ulimit provides control over the resources available to the shell and processes it creates, allowing you to limit memory usage. cgroups allow for more granular control and are used for limiting resources like CPU, memory, and disk I/O for a group of processes.
Example Command: `ulimit -v 1000000 # This limits virtual memory for all processes to approximately 1GB`
<br>

**Question: How do you get the full path of a file in Linux?**<br>
**Explanation:** Imagine you're trying to tell a friend how to get to your house. Instead of just saying "My house," you give them your full address with the street name, city, and everything else they need to find it. Similarly, on a computer, if you want to know exactly where a file is, you can ask for its full address, which is called the "full path." This tells you exactly where the file is located on your computer.<br>
**Technical Answer:** In Linux, the full path of a file refers to its absolute path, which starts from the root directory. To obtain the full path, you can use the realpath command or the pwd command if you're in the same directory as the file.
Example Command: `realpath filename.txt`
<br>

**Question: How to administer Linux servers?**<br>
**Explanation:** Administering Linux servers is like taking care of a fleet of cars. You need to regularly check their oil, tire pressure, and make sure they're running smoothly. Occasionally, you'll need to fix problems or add new parts.<br>
**Technical Answer:** Linux server administration involves installing and configuring software, managing user accounts and permissions, monitoring system performance, setting up and maintaining network configurations, applying updates and patches, backing up data, and troubleshooting issues as they arise. Tools like SSH for remote access, cron for scheduling tasks, and system monitoring tools are essential in a sysadmin's toolkit.
<br>

**Question: How do you optimize Linux system performance?**<br>
**Explanation:** Optimizing Linux system performance is like tuning a car to make it run faster and smoother. You clean up unnecessary files, adjust settings to match how you use your computer, and ensure everything is up-to-date.<br>
**Technical Answer:** Linux system performance can be optimized by monitoring resource usage with tools like top, htop, or nmon, and identifying bottlenecks. Kernel parameters can be tuned via the /proc filesystem or sysctl. Unnecessary services and startup programs should be disabled. Filesystem performance can be improved using appropriate mount options, and regular system updates, along with judicious use of resources, contribute to overall system optimization.
<br>

**Question: What is a Linux virtual memory system?**<br>
**Explanation:** A Linux virtual memory system is like having an extra storage unit when your house gets too full. When your computer runs out of actual memory, it uses a section of the hard drive to temporarily store data.<br>
**Technical Answer:** The Linux virtual memory system uses both RAM and a portion of the hard disk, called swap space, to manage the system's memory resources. It provides an abstraction layer that allows processes to have more memory available than physically present, handles memory protection, and facilitates efficient memory allocation and paging.
<br>

**Question: What is Load Average in Linux ?**<br>
**Explanation:** Load average is like measuring how busy a cashier is at a store. If there are more customers than cashiers, the load is high. It's a way to see how much work is waiting to be done.<br>
**Technical Answer:** Load average represents the average system load over a period of time. It gives the number of processes that are either in a runnable or uninterruptible state. A process in a runnable state is either using the CPU or waiting to use the CPU, while a process in an uninterruptible state is waiting for some I/O access, like disk access.
<br>

**Question: What is a Shell Script ?**<br>
**Explanation:** A shell script is like a cooking recipe for your computer. It tells your computer a series of steps to follow, one after another, to complete a task.<br>
**Technical Answer:** A shell script is a text file containing a sequence of commands for a UNIX-based operating system. It's a script written for the shell, or command line interpreter, of an operating system.
<br>

**Question: What is the find command, and how do you use it?**<br>
**Explanation:** The find command is like playing hide and seek with files. You tell your computer what to look for, and it finds files that match your description.<br>
**Technical Answer:** find searches for files in a directory hierarchy. You can specify criteria like name, type, size, or modification time. An example is find / -name filename.
<br>

**Question: What is strace command? Its alternatives?**<br>
**Explanation:** Think of strace as a detective tool that follows a program around, noting everything it does. This helps you understand what's happening behind the scenes. If strace is not available, you can use other detective tools like ltrace or dtrace.<br>
**Technical Answer:** strace is a diagnostic, debugging, and instructional userspace utility for Linux used to monitor the system calls made by a program and the signals it receives. Its alternatives include ltrace for library call tracing and dtrace for dynamic tracing, which provide similar functionality for different use cases or system architectures.
<br>

**Question: How does env command work?**<br>
**Explanation** The env command is like taking a snapshot of all the settings and preferences you have on your computer at a moment in time.<br>
**Technical Answer:** The env command in UNIX/Linux prints out the current environment variables or runs a program in a modified environment.
<br>

**Question: Command to check the memory status.**<br>
**Explanation:** It's like checking the fuel gauge in your car to see how much gas you have left. In this case, you're checking how much memory your computer is using.<br>
**Technical Answer:** The free command is commonly used to display the amount of free and used memory in the system.
<br>

**Question: Linux directory commands.**<br>
**Explanation:** Directory commands are like the basic commands you give to a filing cabinet — open this drawer, create a new folder, find this file, etc.<br>
**Technical Answer:** Linux directory commands include ls (list directory contents), cd (change directory), mkdir (make directory), rmdir (remove directory), and pwd (print working directory).
<br>

**Question: what is the command used to review boot messages.**<br>
**Explanation:** It's like reading the logbook of a ship to see everything that happened from the moment it left port.<br>
**Technical Answer:** The dmesg command is used to examine or control the kernel ring buffer. It can display boot-up messages among other kernel messages.
<br>

**Question: What is the File system used to access remote systems ?**<br>
**Explanation:** It's like having a special phone line that lets you access files stored in a friend's computer.<br>
**Technical Answer:** Network File System (NFS) and Server Message Block (SMB) are commonly used protocols to access files on remote systems.
<br>

**Question: Command commonly used to record sessions in Linux.**<br>
**Explanation:** It's like having a tape recorder that records everything you say and do on your computer.<br>
**Technical Answer:** The script command is commonly used to make a typescript of everything displayed on your terminal. It records all the input and output of a terminal session.
<br>

**Question: How do you secure a Linux server?**<br>
**Explanation:** Securing a Linux server is like securing your house. You change the locks (passwords), install an alarm system (firewall), and make sure your windows and doors (ports and services) are properly closed and locked unless you need them open.<br>
**Technical Answer:** Securing a Linux server involves setting strong passwords, configuring a firewall like iptables or UFW, keeping the system updated, disabling root login via SSH, using key-based authentication, closing unnecessary ports, setting proper permissions, and using tools like Fail2Ban to prevent brute-force attacks. Regular security audits, kernel hardening, and employing SELinux/AppArmor for mandatory access control also contribute to a server's security.
<br>

**Question: What is SELinux?**<br>
**Explanation:** SELinux is like a VIP bodyguard for your computer. It has strict rules about who can do what, providing an extra layer of security by keeping a close eye on software and users, making sure they only do what they're supposed to.<br>
**Technical Answer:** SELinux (Security-Enhanced Linux) is a security architecture integrated into the Linux kernel. It uses mandatory access controls (MAC) to enforce the security decisions of a central policy, limiting programs and system services to the minimum level of permissions they require to work.
<br>

**Question: What is the purpose of the SSH protocol in Linux, and how do you securely connect to a remote server using SSH?**<br>
**Explanation:** SSH is like a secure phone line for computers. When you want to talk to another computer, SSH encrypts your conversation, so nobody else can listen in. To connect securely, you need the right password or a special key that proves who you are.<br>
**Technical Answer:** SSH (Secure Shell) is a protocol used for secure communication over an unsecured network. It provides strong authentication and encrypted data communications between two computers connecting over an open network such as the internet. To connect using SSH, you can use a password or cryptographic keys for authentication.
<br>

**Question: How would you recover a root password that you have forgotten on a critical server?**<br>
**Technical Answer:**
Reboot the server and access the GRUB menu.
Edit the boot parameters to enter single-user mode or init=/bin/bash.
Reset the root password and reboot.
<br>

**Question:  A critical service fails to start at boot. How would you troubleshoot and fix it?**<br>
**Technical Answer:**
Check the service logs and system journal for error messages.
Verify the configuration files for any recent changes or errors.
Ensure all dependencies for the service are installed and running.
Test starting the service manually to isolate the issue.
<br>

**Question: How would you ensure that your servers are compliant with company security policies?**
<br>
**Technical Answer:**
Regularly audit servers with tools like Lynis or OpenSCAP.
Implement automated compliance checking with Ansible or Puppet.
Continuously monitor the system logs and set up alerts for suspicious activities.
<br>

**Question: How do you handle a server that is running out of disk space frequently?**
<br>
**Technical Answer:**
Identify the directories/files consuming the most space using tools like du or ncdu.
Set up log rotation and archiving to manage log file sizes.
Implement monitoring and alerts for disk usage thresholds.
Consider adding more storage or migrating data to a larger disk.
<br>

**Question: How do you manage and monitor multiple Linux servers efficiently?**
<br>
**Technical Answer:**
Use centralized configuration management tools like Ansible, Puppet, or Chef.
Set up monitoring solutions like Nagios, Prometheus, or Zabbix for health and performance monitoring.
Implement centralized logging with ELK Stack or Graylog.
<br>

**Question: How would you handle a corrupted filesystem?**<br>
**Technical Answer:**
Run filesystem checks using fsck on unmounted filesystems.
Attempt to repair the filesystem, if possible.
If irreparable, restore from a backup.
Check hardware for potential issues if corruption is recurring.
<br>

**Question: How do you manage kernel updates, especially on critical systems?**<br>
**Technical Answer:**
Schedule updates during maintenance windows.
Test updates in a staging environment before applying to production.
Use tools like ksplice for live kernel patching without rebooting.
<br>

**Question: How would you set up a highly available web service in Linux?**<br>
**Technical Answer:**
Use load balancers like HAProxy or Nginx to distribute traffic.
Implement a failover mechanism using keepalived or a similar tool.
Utilize clustering with solutions like Pacemaker and Corosync.
<br>

**Question: Describe a situation where you had to recover data from a failed hard drive.**<br>
**Technical Answer:**
Use tools like ddrescue to clone the drive and attempt data recovery.
Employ file carving tools like TestDisk or PhotoRec if the filesystem is damaged.
Send the drive to professional data recovery services if in-house recovery fails.
<br>

**Question: How do you optimize network performance on a Linux server?**<br>
**Technical Answer:**
Adjust network parameters using sysctl (e.g., TCP window size, buffers).
Use traffic shaping tools like tc to prioritize traffic.
Implement Quality of Service (QoS) on the network.
<br>

**Question: How would you deal with a rogue process consuming all CPU resources?**<br>
**Technical Answer:**
Identify the process using top or htop.
Use nice and renice to adjust the process priority.
Kill the process if necessary and investigate the cause.
<br>

**Question: How do you secure SSH access on your servers?**<br>
**Technical Answer:**
Disable root login and use SSH keys instead of passwords.
Implement two-factor authentication.
Restrict access with AllowUsers/AllowGroups and IP whitelisting.
Use fail2ban to block repeated failed login attempts.
<br>

**Question: How would you handle a suspected memory leak in an application?**<br>
**Technical Answer:**
Monitor the application’s memory usage over time.
Use tools like valgrind or memleax to trace memory leaks.
Collaborate with developers to fix the leak in the application code.
<br>

**Question: How do you prepare for and handle a server migration with zero downtime?**<br>
**Technical Answer:**
Use a blue-green deployment strategy.
Synchronize data between old and new servers.
Test thoroughly before switching over.
Employ a load balancer or DNS changes for a seamless transition.
<br>

**Question: How do you handle backups for a large number of Linux servers?**<br>
**Technical Answer:**
Implement centralized backup solutions like Bacula or Amanda.
Ensure regular backups with cron jobs.
Test restore processes periodically for reliability.
<br>

**Question: Describe a situation where you had to troubleshoot a complex network issue in Linux.**<br>
**Technical Answer:**
Use network diagnostic tools like ping, traceroute, netstat, ss, and tcpdump.
Analyze network traffic and logs to isolate the issue.
Collaborate with the networking team for a holistic approach.
These Questions probe deeper into the skills and experiences of a Linux System Administrator, focusing on problem-solving, critical thinking, and practical application of knowledge in real-world scenarios. The answers should reflect a candidate’s ability to handle complex issues and maintain the stability and security of Linux systems.
<br>

**Question: A server is running slow, but CPU, memory, and disk IO all look normal. What could be wrong?**<br>
**Technical Answer:**
Network issues could be causing the slowness.
Misconfiguration in server settings.
Could be an issue with a slow-running process, requiring a deeper look using tools like top, htop, or iotop.
Kernel issues or need for updates/patches.
<br>

**Question: How would you troubleshoot a service failure after a package update?**<br>
**Technical Answer:**
Check service logs using journalctl or in /var/log/.
Verify if the configuration files were overwritten during the update.
Check for dependency issues with the new package.
Rollback to a previous version if necessary.
<br>

**Question: How would you handle a full /boot partition?**<br>
**Technical Answer:**
Remove old kernels using package managers like apt or yum.
Clean up unused files in /boot.
Resize the partition if it's consistently getting full.
<br>

**Question: Describe a situation where you had to optimize a server for better performance.**<br>
**Technical Answer:**
Implemented caching, adjusted kernel parameters, configured a load balancer, or optimized databases.
Monitored using tools like Nagios, Prometheus, or Grafana and made data-driven optimizations.
<br>

**Question: How do you secure a new Linux server?**<br>
**Technical Answer:**
Configure firewall rules with iptables or ufw.
Set up SSH key-based authentication and disable root login.
Keep the system updated with the latest patches.
Use SELinux/AppArmor for additional security.
Regularly audit the server with tools like Lynis.
<br>

**Question: You accidentally deleted an important configuration file. How do you recover it?**<br>
**Technical Answer:**
Restore from backup.
Use the extundelete tool if the file system is ext3/ext4.
Check if the package manager kept a backup (e.g., .rpmnew or .dpkg-old files).
<br>

**Question: How would you automate repetitive tasks in Linux?**<br>
**Technical Answer:**
Use cron jobs for scheduled tasks.
Write shell scripts for complex tasks.
Use configuration management tools like Ansible, Puppet, or Chef.
<br>

**Question: How do you handle kernel panic?**<br>
**Technical Answer:**
* Analyze the panic message and logs to understand the cause.
* Boot from a live CD/USB to repair the system if necessary.
* Check for hardware issues if the panic is recurring.
* Update/rollback the kernel if the issue is software-related.
<br>

**Question: How do you handle a DDoS attack?**<br>
**Technical Answer:**
Implement IP filtering and rate limiting.
Use tools like fail2ban to block offending IPs.
Deploy a reverse proxy or load balancer to distribute traffic.
Collaborate with the ISP or hosting provider for additional mitigation.
<br>

**Question: How would you migrate a service from one server to another with minimal downtime?**<br>
**Technical Answer:**
Plan the migration and inform stakeholders.
Sync the data between old and new servers using tools like rsync.
Test the service on the new server.
Update DNS records or use a load balancer to switch traffic to the new server.
Monitor the service closely after migration.
<br>

**Question: How do you manage package versions across multiple servers to ensure consistency?**<br>
**Technical Answer:**
Use configuration management tools like Ansible, Puppet, or Chef.
Set up a local repository mirror to control package versions.
Implement infrastructure as code practices for consistency.
<br>

**Question: How do you handle a situation where a server has been compromised?**<br>
**Technical Answer:**
Isolate the server from the network.
Conduct a forensic analysis to understand the breach.
Restore from a known good backup.
Harden the server and patch the vulnerability before bringing it back online.
Review and improve security measures.
<br>

**Question: How would you reduce the boot time for a server?**<br>
**Technical Answer:**
Disable unnecessary services and startup scripts.
Use a more efficient init system like systemd.
Optimize kernel parameters.
Consider using a lighter version of the Linux OS.
<br>

**Question: How do you handle a situation where you accidentally executed a command that could harm the system?**<br>
**Technical Answer:**
Immediately stop the process if it’s still running.
Assess the impact and start damage control.
Restore affected files from backup.
Document the incident and implement safeguards to prevent future occurrences.
These **Questions delve into various aspects of a Linux System Administrator's role, from troubleshooting and performance optimization to security and disaster recovery. The answers should demonstrate a deep understanding of Linux systems and problem-solving skills.
<br>

**Question: what is the difference between init 6 and reboot ?**<br>
**Technical Answer:** reboot uses the shutdown command (with the -r switch). The shutdown command used to kill all the running processes, unmount all the file systems and finally tells the kernel to issue the ACPI power command. In older distros the reboot command was forcing the processes to exit by issuing the SIGKILL signal (still found in sources, can be invoked with -f option), in most recent distros it defaults to the more graceful and init friendly init 1 -> shutdown -r. This ensures that daemons clean up themselves before shutdown.
init 6 tells the init process to shutdown all of the spawned processes/daemons as written in the init files (in the inverse order they started) and lastly invoke the shutdown -r now command to reboot the machine.
<br>

**Question: Explain SAR.**<br>
**Technical Answer:** sar (System Activity Report) It can be used to monitor Linux system’s resources like CPU usage, Memory utilization, I/O devices consumption, Network monitoring, Disk usage, process and thread allocation, battery performance, Plug and play devices, Processor performance, file system and more. Linux system Monitoring and analyzing aids in understanding system resource usage which can help to improve system performance to handle more requests. In order to run sar, one need to install `systat`.
<br>

**Question: How to do kernel upgrade ?**<br>
**Technical Answer:** Kernel Upgrade is a fairly simple process. In involves below mentioned commands.

(Centos, RHEL)
1. Run the uname -a command to query the current kernel version.
```uname -a```
2. Run the yum update kernel command to upgrade the kernel.
```yum update kernel``` 
3. Run the cat /boot/grub2/grub.cfg |grep menuentry command to check the kernel information of the OS after the upgrade.
```cat /boot/grub2/grub.cfg |grep menuentry```

(Ubuntu, Debian)
1. Run the uname -sr command to query the current kernel version.
```uname -sr```
2. Goto `http://kernel.ubuntu.com/~kernel-ppa/mainline/` and choose the desired version (Kernel 5.0 is the latest at the time of writing) from the list by clicking on it.
3. download the `.deb` files for your system architecture using `wget` command.
4. Once you’ve downloaded all the above kernel files, now install them as follows:
```sudo dpkg -i *.deb```
<br>

**Question: How to rollback kernel upgrade incase applications starts failing due to upgraded kernel version.**<br>
**Technical Answer:** 
(Ubuntu, Debian)
1.  make a backup copy of /etc/default/grub. In case something goes wrong, you can easily revert to the known-good copy:
```sudo cp /etc/default/grub /etc/default/grub.bak```
2. Then edit the file using vim or the text editor of your choice:
```sudo vim /etc/default/grub```
3. Find the line that contains `GRUB_DEFAULT=0` and set it to `GRUB_DEFAULT=x`, where x is the index of grub menu item to which you would like to boot to by default. Note that the menu items are zero-indexed. That means that the first item in the list is 0 and that the sixth item is actually 5. So to boot to the sixth item in the list, the line would read: 
`GRUB_DEFAULT=5`
4. Then build the updated grub menu: 
```sudo update-grub```

(Centos, RHEL)
1. Run the following commands to set the original kernel version as the default startup kernel and verify the modification result
```yum list kernel --show-duplicates```
2. Lets say, kernel of interest is `kernel-3.10.0-862.el7`, then run the following command to set it to the same.
```yum downgrade kernel-3.10.0-862.el7 ```
<br>

**Question: What are sticky bits ?**<br>
**Technical Answer:** A Sticky bit is a permission bit that is set on a file or a directory that lets only the owner of the file/directory or the root user to delete or rename the file. No other user is given privileges to delete the file created by some other user.
1. Creating a directory
```mkdir allaccess```
2. Creating a sticky bit for folder allaccess 
```chmod +t allAccess/```
3. Lets check the permission of folder
```ls -ld allAccess/
    drwxrwxrwt 2 ravi ravi 4096 Oct 24 16:19 allAccess/
```
<br>

**Quesiton: What are ACLs ?**<br>
**Explanation:** Think of a scenario in which a particular user is not a member of group created by you but still you want to give some read or write access, how can you do it without making user a member of group, here comes in picture Access Control Lists, ACL helps us to do this trick.
Basically, ACLs are used to make a flexible permission mechanism in Linux.
From Linux man pages, ACLs are used to define more fine-grained discretionary access rights for files and directories.<br>
**Technical Answer:** Access control list (ACL) provides an additional, more flexible permission mechanism for file systems. It is designed to assist with UNIX file permissions. ACL allows you to give permissions for any user or group to any disc resource.
setfacl and getfacl are used for setting up ACL and showing ACL respectively.
<br>

**Question: What is the difference between SUID vs UID vs ACL ?**<br>
**Technical Answer:**
SUID (Set User ID) is a permission that can be set on an executable file so that it is run with the privileges of the file's owner, not with the privileges of the user invoking the command. It is done via the command chmod u+s myfile.
ACL (Access Control Lists) is the way to give more fine-grained permissions to files, compared to the Discretionary Access Control (rwx permissions to user, group, and other) used as a default in Linux systems. They are set using the setfacl command.
UID stands for User Identifier. It is a unique numerical value assigned to each user account. The UID is used by the system to identify and differentiate between different users.
<br>

**Question: What is PAM?**<br>
**Technical Answer:** PAM separates the standard and specialized tasks of authentication from applications. Programs such as login, gdm, sshd, ftpd, and many more all want to know that a user is who they say they are, yet there are many ways to do that. A user can provide a user name and password credential which can be stored locally or remotely with LDAP or Kerberos. A user can also provide a fingerprint or a certificate as a credential. It would be painful to ask each application developer to rewrite the authentication checks for each new method. A call to PAM libraries leaves the checks to authentication experts. PAM is pluggable in that we can have different applications run different tests and modular in that we can add new methods with new libraries.
If you make a change to authentication using a program such as authconfig or authselect and want to see what changed, here are some of the places to look:
`/usr/lib64/security`
A collection of PAM libraries that perform various checks. Most of these modules have man pages to explain the use case and options available.
`/etc/pam.d`
A collection of configuration files for applications that call libpam. These files define which modules are checked, with what options, in which order, and how to handle the result. These files may be added to the system when an application is installed and are frequently edited by other utilities.
Since there are several checks done by all applications, these files may also have include statements to call other configuration files in this directory. Most shared modules are found in the system-auth file for local authentication and the password-auth file for applications listening for remote connections.
`/etc/security`
A collection of additional configuration files for specific modules. Some modules, such as pam_access and pam_time, allow additional granularity for checks. When an application configuration file calls these modules, the checks are completed using the additional information from its corresponding supplemental configuration files. Other modules, like pam_pwquality, make it easier for other utilities to modify the configuration by placing all the options in a separate file instead of on the module line in the application configuration file.
`/var/log/secure`
Most security and authentication errors are reported to this log file. Permissions are configured on this file to restrict access.
<br>

**Question: Difference between FirewallD and Iptables ?**<br>
**Technical Answer:** In the context of Linux (not just RHEL) a firewall is a collection of rules that operate on network packets that traverse the Linux kernel's network stack. Mostly, those rules live in the kernel module called Netfilter.
In order to load, unload and inspect those rules there exists a userspace tool called iptables. Iptables is just a translator that takes the notation used to describe the specific rules and formats them into the data structures needed by the kernel, and then sends them to the kernel.
There are numerous software packages that put a prettier face in front of the iptables rule notation, as well as providing collections of rules that are commonly used to perform certain tasks. These packages are often described as firewalls, but I consider that a misnomer. They are tools used to create and manage firewalls, but the actual firewall is always in the Linux kernel.
<br>

**Question: Difference between initrd and initrmfs ? **Explanation** also.**<br>
**Explanation:** initrd gives us the ability to load a RAM disk by the bootloader. The loaded RAM disk is mounted as the root file system, and different programs are run from it. We can also mount a new root file system from a different device, making the bootloader move the former initrd root to a different directory, and we can unmount it. The primary design of initrd was to allow our system startup to occur in two preceding phases:
The kernel allocates a minimum set of compiled-in drivers
Loading of additional modules from initrd
initrd usually functions as a block device, and compiling it into the kernel requires a file system driver such as ext2, ext3, or ext4.
initramfs is a cpio archive file of the initial file system that is loaded to memory. This loading happens after the kernel finishes starting the system, and before the user-space begins the init procedure.
The contents of initramfs are loaded as the initial root file system by the kernel before the main root is loaded. The initial root contains the files that are required to mount the “real” root file system and initialize our system. The files mostly contain kernel modules.<br>
**Technical Answer:** We can use initrd for Linux kernels 2.4 and lower. Conversely, initramfs is for kernels 2.6 and above.Compiling initrd into the kernel requires at least one filesystem driver, which increases boot-time flexibility, simplicity, and memory efficiency.
With initramfs, we can create an archive with the files that the kernel will extract to a tmpfs, which makes file access extremely fast.
<br>

**Question: what are SUID, GUID in linux ?**<br>
**Technical Answer:** SUID or Set Owner User ID is a permission bit flag that applies to executables. SUID allows an alternate user to run an executable with the same permissions as the owner of the file instead of the permissions of the alternate user.When the SUID bit is set on an executable file, this means that the file will be executed with the same permissions as the owner of the executable file.
GUID is similar to SUID. In the SUID, the executable in **Question runs with the privileges of the owner of the file. In the GUID, if it’s an executable, then it runs with the permissions of the group. If it’s a directory, it results in all new files and directories created to belong to the group.It’s benefit is in handling the directory. When GUID permission is applied to a directory, all sub directories and files created inside this directory will get the same group ownership as main directory (not the group ownership of the user that created the files and directories).
<br>

**Question: what is difference between anacron vs cron ?**<br>
**Technical Answer:** Cron is a time-based job scheduler in Unix-like operating systems. It enables users to schedule jobs to run periodically at fixed times, dates, or intervals. With Cron, you can automate tasks like backups, system updates, maintenance, data synchronization, and many others. Assumes that the machine is running all the time. If a scheduled task is missed, it won't be executed.  Can be used by any user, offering higher flexibility. Offers granular control over the scheduling, down to the minute.
Anacron is a job scheduler in Unix-like operating systems. It is similar to Cron but has a different purpose. It is used for scenarios where your machine might not be running all the time. Unlike Cron, it doesn't expect the system to be continuously running. In this, your jobs are mostly executed periodically, as it provides you with time flexibility.  Will execute missed tasks as soon as the machine is up and running. Usually restricted to the system administrator, which limits its use for regular users. Focuses on a broader time scale such as daily, weekly, or monthly. 
<br>

**Question: How do you check for processess on particular cpu or core ?**<br>
**Technical Answer:** You can use ps command to find out which process is currently assigned to which CPU core. Lookout for the PSR field in ps command output.
Example:
```$ ps -o pid,psr,comm -p 24868```
```taskset -c -p <PID>```
<br>

**Question: What are namespaces in Linux ?**<br>
**Technical Answer:** Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The key feature of namespaces is that they isolate processes from each other. On a server where you are running many different services, isolating each service and its associated processes from other services means that there is a smaller blast radius for changes, as well as a smaller footprint for security‑related concerns. The list of namespaces comprises of User, IPC, UTC, Network, Process, UTS, Mount.
<br>

**Question: What are Cgroups in Linux ?**<br>
**Technical Answer:** A control group (cgroup) is a Linux kernel feature that limits, accounts for, and isolates the resource usage (CPU, memory, disk I/O, network, and so on) of a collection of processes.
Cgroups provide the following features:
Resource limits – You can configure a cgroup to limit how much of a particular resource (memory or CPU, for example) a process can use.
Prioritization – You can control how much of a resource (CPU, disk, or network) a process can use compared to processes in another cgroup when there is resource contention.
Accounting – Resource limits are monitored and reported at the cgroup level.
Control – You can change the status (frozen, stopped, or restarted) of all processes in a cgroup with a single command.
<br>

**Question: How do you streamline load across all cores ? What is irq balance ?**<br>
**Technical Answer:** irqbalance is a command line tool that distributes load, generated by different interrupt sources, across CPUs in order to achieve better system performance. It can be run in a oneshot mode where it distributes interrupts once and then stops. However by default it runs as a daemon and periodically performs interrupt load balancing at intervals of a fixed time period (default 10 sec, but configurable as well). At a very high level irqbalance periodically gathers interrupt and softirq related load by reading relevant entries in /proc/interrupts and /proc/stat and changes the affinity of one or more interrupts so that this load is more evenly distributed between NUMA nodes, processor packages and/or CPUs. 
<br>

**Question: How is interrupts distribution done ?**<br>
**Technical Answer:** Interrupt requests coming from external hardware devices can be distributed among the available CPUs in two ways:
***Static distribution***
The IRQ signal is delivered to the local APICs listed in the corresponding Redirection Table entry. The interrupt is delivered to one specific CPU, to a subset of CPUs, or to all CPUs at once (broadcast mode).
***Dynamic distribution***
The IRQ signal is delivered to the local APIC of the processor that is executing the process with the lowest priority.
Every local APIC has a programmable task priority register (TPR), which is used to compute the priority of the currently running process. Intel expects this register to be modified in an operating system kernel by each process switch.
If two or more CPUs share the lowest priority, the load is distributed between them using a technique called arbitration . Each CPU is assigned a different arbitration priority ranging from 0 (lowest) to 15 (highest) in the arbitration priority register of the local APIC.
Every time an interrupt is delivered to a CPU, its corresponding arbitration priority is automatically set to 0, while the arbitration priority of any other CPU is increased. When the arbitration priority register becomes greater than 15, it is set to the previous arbitration priority of the winning CPU increased by 1. Therefore, interrupts are distributed in a round-robin fashion among CPUs with the same task priority.
<br>

**Question: How do you ensure nic card name consistency ?**<br>
**Technical Answer:** The udev device manager implements consistent device naming in most of the Linux distros. The device manager supports different naming schemes and, by default, assigns fixed names based on firmware, topology, and location information. To implement a consistent naming scheme for network interfaces, the udev device manager processes the following rule files in the listed order:
1. /usr/lib/udev/rules.d/60-net.rules
2. /usr/lib/udev/rules.d/71-biosdevname.rules ( for DELL systems )
3. /usr/lib/udev/rules.d/75-net-description.rules
4. /usr/lib/udev/rules.d/80-net-setup-link.rules
<br>

**Question: What is chroot ? Explain its impact ?**<br>
**Technical Answer:** The chroot Linux utility can modify the working root directory for a process, limiting access to the rest of the file system. This is usually done for security, containerization, or testing, and is often called a "chroot jail". Chroot does one thing---run a command with a different root directory. The command being run has no idea that anything outside of its jail exists, as it doesn't have any links to it, and as far as it's aware, is running on the root filesystem anyway. There's nothing above root, so the command can't access anything else.
Chroot doesn't make any modifications to your disk, but it can make it appear that way from the point of view of the processes running under it. Chrooting a process accomplishes the same thing as changing the mount namespace for a process, but does so at a higher level than namespace modification.
A process that needs to access and interact with user-level resources would not work well inside a chroot jail, or would require extra configuration that may make the whole setup more insecure. But, even complicated apps like Apache and MySQL can be run inside a chrooted environment with all dependencies accounted for.
<br>

**Question: Explain difference between SNAT and DNAT ?**<br>
**Technical Answer:** SNAT, as name suggests, is a technique that translates source IP address generally when connecting from private IP address to public IP address. It maps source client IP address in a request to a translation defined on BIG-IP device. It is most common form of NAT that is used when internal host needs to initiate session to an external host or public host. It is generally used to change private address or port into a public address or port for packets leaving network. It generally allows multiple hosts on inside to get any host on outside. Client inside LAN and behind Firewall needs to browse Internet. 
DNAT, as name suggests, is a technique that translates destination IP address generally when connecting from public IP address to private IP address. It is generally used to redirect packets destined for specific IP address or specific port on IP address, on one host simply to a different address mostly on different host. It is generally used to redirect incoming packets with destination of public address or port to private IP address or port inside network. It generally allows multiple hosts on outside to get single host on inside. Website hosted inside data center behind Firewall and needs to be accessible to users over Internet.
<br>

**Question: What is conntrack/connection track ? How do you track connections in IPtables ?**<br>
**Technical Answer:** It is the ability to maintain connection information in memory. This is new feature added in 2.4.xx Linux kernel. Eariler only commercial firewall has this feature but now it is part of Linux. It can remember connection states such as established & new connections along with protocol types, source and destination ip address. You can allow or deny access based upon state. Following are the states:
NEW â€“ A Client requesting new connection via firewall host
ESTABLISHED â€“ A connection that is part of already established connection
RELATED – A connection that is requesting a new request but is part of an existing connection.
INVALID – If none of the above three states can be referred or used then it is an INVAID state.

Connection tracking is already recording things about the tracked connections, like whether one connection is related to another (such as a new FTP DATA connection being related to an existing FTP session, even though it's on a different port).The conntrack iptables extension provides additional criteria you can use in iptables rules to match the tracked state, for instance by allowing these related connections through.
If you don't use the conntrack extension then the connections are still tracked by the kernel (if the appropriate kernel modules are loaded) but that tracking information then goes unused as it won't be examined by any iptables rules.
Basically the whole connection tracking system is split in two - the bit in the kernel that does the actual tracking, and the bit in iptables that examines the tracking information from the kernel and decides whether to allow a given packet through or not.
<br>

**Question: How do you set priorities for processess in linux ?**<br>
**Technical Answer:** Priority is a value that you can assign to each process, and the kernel uses this value to schedule the execution of the process. 0-99 is the priority value used for real-time priority assignments. 100-139 is the priority value that the users assign. 
When you start any program or process without any defined priority, nice set a default priority of 10. A niceness of 19 is the lowest priority, while -20 is the highest priority.The nice command is very useful when several processes demand more resources than the CPU. Renice is very similar to nice and is used to change the priority of an already running process. 
Example:
```renice -n -15 -p <PID>```
or
```renice -n 10 -u root```
or
```nice -n 19 <Command>```
<br>

**Question: What is htaccess file ?**<br>
**Technical Answer:** Htaccess is short for Hypertext Access. It is a configuration file used by Apache-based web servers.
Configuration files configure the initial settings of a program or, in this case, the server. This means that the .htaccess file can be used to make the server behave in a certain way. <br>

**Question: How do you recover a lvm if any lvm partition fails ?**<br>
**Technical Answer:** To rebuild the mirrored volume, you replace the broken drive and recreate the physical volume. If you use the same disk rather than replacing it with a new one, you will see "inconsistent" warnings when you run the `pvcreate` command. You can prevent that warning from appearing by executing the vgreduce --removemissing command.
```pvcreate /dev/sdi[12]```
```pvscan```
```vgextend vg /dev/sdi[12]```
```pvscan```
```lvconvert -m 1 /dev/vg/groupfs /dev/sdi1 /dev/sdb1 /dev/sdc1```
```lvs -a -o +devices```
<br>

**Question: How can you recover root password ?**<br>
**Technical Answer:** 
* First, you need console access: Either at a keyboard and monitor locally, or via Virtual Machine remote console, you will need to see and interact with the bootloader.
* Reboot the machine: As soon as the bootloader comes up with the selection screen, quickly tap the up and down arrows up and down to pause the countdown.
* Select the kernel you want to boot into, and hit 'e': This will take you into a screen where you can edit the grub bootloader script.
* Find the line that refers to the kernel: There will be a series of 'boot parameters' here: these are instructions passed during the loading of the kernel.
* For RHEL/CentOS 7, the line starts with 'linux16'.
* For RHEL/Centos 8x, and Fedora the line starts with 'linux'.
* Add 'rd.break' at the end of that line (There are other things you can do here, but for now, this is all you need) [ Note: This change is temporary ].
* Now hit Ctrl-x to run the edited bootloader script.
* You’ll boot to a 'rescue' prompt that looks like this: switch_root:/#.
* Remount the root partition in read-write mode so that you can run commands. Enter the following: mount -o remount rw /sysroot and then hit ENTER.
* Now type chroot /sysroot and hit enter. This will change you into the sysroot (/) directory, and make that your path for executing commands. 
* Now you can simply change the password for root using the passwd command.
* Next, before you reboot, you will need to make sure that SELinux allows the file changes. At the prompt ,enter: touch /.autorelabel. This will signal SELinux on the next reboot that the filesystem has changed (the changed password) and allow the change to be loaded. This will cause the whole filesystem to be 'relabeled' which might take a while, depending on the size of the filesystem and the speed of the machine, so be aware of this possibility.
* Type `exit` to leave the chroot environment and enter reboot.
<br>

**Question: What is steal time in CPU ?**<br>
**Technical Answer:** Steal time is the amount of CPU time needed by a guest virtual machine that is not provided by the host. Steal time occurs when the host allocates these resources elsewhere: for example, to another guest.
Steal time is reported in the CPU time fields in /proc/stat. It is automatically reported by utilities such as top and vmstat. It is displayed as "%st", or in the "st" column. Note that it cannot be switched off. Large amounts of steal time indicate CPU contention, which can reduce guest performance. To relieve CPU contention, increase the guest's CPU priority or CPU quota, or run fewer guests on the host.
<br>

**Question: What is iSCSI ?**<br>
**Technical Answer:** ISCSI is a transport layer protocol that describes how Small Computer System Interface (SCSI) packets should be transported over a TCP/IP network. ISCSI makes it possible to set up a shared-storage network where multiple servers and clients can access central storage resources as if the storage was a locally connected device. SCSI -- without the "i" prefix -- is a data access protocol that's been around since the early 1980s. ISCSI works by transporting block-level data between an iSCSI initiator on a server and an iSCSI target on a storage device. The iSCSI protocol encapsulates SCSI commands and assembles the data in packets for the TCP/IP layer. Packets are sent over the network using a point-to-point connection. Upon arrival, the iSCSI protocol disassembles the packets, separating the SCSI commands so the operating system (OS) will see the storage as if it was a locally connected SCSI device that can be formatted as usual. 
<br>

**Question: What is difference between GPT and MBR ?**<br>
**Technical Answer:** MBR stands for Master Boot Record, and is a bit of reserved space at the beginning of the drive that contains the information about how the partitions are organized. The MBR also contains code to launch the operating system, and it's sometimes called the Boot Loader. GPT is an abbreviation of GUID Partition Table, and is a newer standard that's slowly replacing MBR. Unlike an MBR partition table, GPT stores the data about how all the partitions are organized and how to boot the OS throughout the drive. That way if one partition is erased or corrupted, it's still possible to boot and recover some of the data.
the maximum capacity of MBR partition tables is only about 2 terabytes. You can use a drive that's larger than 2 terabytes with MBR, but only the first 2 terabytes of the drive will be used. The rest of the storage on the drive will be wasted.GPT partition tables offer a maximum capacity of 9.7 zetabytes. 1 zetabyte is about 1 billion terabytes, so you're unlikely to run out of space anytime soon. GPT partition tables allow for up to 128 separate partitions, which is more than enough for most real world applications. As MBR is older, it's usually paired with older Legacy BIOS systems, while GPT is found on newer UEFI systems. This means that MBR partitions have better software and hardware compatibility, though GPT is starting to catch up.
<br>

**Question: What is the difference between Legacy and UEFI ?**<br>
**Technical Answer:** Legacy Boot refers to the boot process used by the BIOS firmware to initialize hardware devices. The Legacy boot contains a selection of installed devices that get initialized as the computer performs the POST test during the boot process. The legacy boot will check for all connected devices for the Master Boot Record (MBR), usually in the first sector of a disk.When it can’t find a bootloader in the devices, Legacy switches to the next device in the list and keeps repeating this process until it finds a bootloader, or if not, returns an error. It is slower compared to UEFI. Legacy runs in 16-bit mode that only supports keyboard navigation. It does not provide a secure boot method, which allows for the loading of unauthorized applications, making dual-booting possible.
UEFI or Unified Extensible Firmware Interface is a modern way of handling the boot process. UEFI is similar to Legacy, however, it stores the boot data in a .efi file rather than the firmware. You will often find UEFI boot mode in modern motherboards with very intuitive and user-friendly Interfaces. UEFI boot mode contains a special EFI partition that is used to store the .efi file and is used in the boot process and the bootloader. UEFI provides faster boot time. UEFI runs in 32-bit and 64-bit, allowing support for mouse and touch navigation. It allows a secure boot that prevents the loading of unauthorized applications. It may also hinder dual boot because it treats operating systems (OS) as applications.
<br>

**Question: How to add modules in kernel ?**<br>
**Technical Answer:** Linux provides a utility known as “insmod”. This is the utility which can be used to load the kernel module at the running kernel. Let us take an example of hello-world.ko , a module which is the classic example and just prints the hello world message. To load the hello-world kernel module, below is the command which can be used ```insmod hello-world.ko```. 
The “lsmod” command can be used to list all the kernel modules.
To remove or unload the kernel module, we can use the Linux command “rmmod”.
<br>

**Quesiton: What is SELinux ?**<br>
**Technical Answer:** Security-Enhanced Linux (SELinux) is a security architecture for Linux® systems that allows administrators to have more control over who can access the system. SELinux defines access controls for the applications, processes, and files on a system. It uses security policies, which are a set of rules that tell SELinux what can or can’t be accessed, to enforce the access allowed by a policy. 
When an application or process, known as a subject, makes a request to access an object, like a file, SELinux checks with an access vector cache (AVC), where permissions are cached for subjects and objects. If SELinux is unable to make a decision about access based on the cached permissions, it sends the request to the security server. The security server checks for the security context of the app or process and the file. Security context is applied from the SELinux policy database. Permission is then granted or denied. 
If permission is denied, an "avc: denied" message will be available in /var/log.messages. You can tell what your system is supposed to be running at by looking at the /etc/sysconfig/selinux file. SELinux can have permissive mode, enforcing mode, or disabled mode.
<br>

**Question: What do you understand by Context Switching ?**<br>
**Technical Answer:** The Context switching is a technique or method used by the operating system to switch a process from one state to another to execute its function using CPUs in the system. When switching perform in the system, it stores the old running process's status in the form of registers and assigns the CPU to a new process to execute its tasks. While a new process is running in the system, the previous process must wait in a ready queue. The execution of the old process starts at that point where another process stopped it. It defines the characteristics of a multitasking operating system in which multiple processes shared the same CPU to perform multiple tasks without the need for additional processors in the system.
<br>

**Question: If a kernel crashes, what will you do ?**<br>
**Technical Answer:** `Use Safe Mode`: In some cases, you may be able to boot the system in safe mode, which loads a minimal set of drivers and services. This can help you troubleshoot and isolate the cause of the crash.
`Kernel Debugging`: If you have the technical expertise, you can perform kernel debugging to analyze the crash dump or core dump files generated by the kernel. This is a more advanced technique and typically requires knowledge of debugging tools and kernel internals.
`Consider System Restore`: If you're using a Windows operating system, you can try using the System Restore feature to revert your system to a previous state when it was working correctly.
Reinstall the Operating System: As a last resort, if all else fails and you suspect a deep-seated software issue that cannot be resolved, you may need to reinstall the operating system. Be sure to back up your data before taking this step.
<br>

**Question: What is PXE and iPXE, when will you use each ?**<br>
**Technical Answer:** PXE (Preboot eXecution Environment) and iPXE (Internet Preboot eXecution Environment) are network boot protocols used in computer systems to boot from a network server rather than a local storage device, such as a hard drive or a USB drive. They serve similar purposes, but iPXE is an extended version of PXE with additional features and capabilities.
PXE is a widely used network boot protocol that allows a computer to boot over a network using the Ethernet interface. It is commonly used in enterprise environments for tasks such as network-based OS deployment, system recovery, and remote management. Here's when you might use PXE:
- `Network-Based OS Deployment`
- `Diskless Boot`
- `Network Diagnostics and Recovery`
iPXE is an open-source and more advanced version of PXE. It extends the capabilities of PXE and includes support for additional network protocols, scripting, and various features. You might choose to use iPXE over traditional PXE in the following scenarios:
- `Improved Compatibility`
- `Scripting and Customization`
- `Boot from Additional Sources`
    - HTTP
    - iSCSI
    - PXE Servers
- `Security Features:`
- `Advanced Network Protocols`
<br>

**Question: What is kernel panic ?**<br>
**Technical Answer:** A kernel panic is one of several Linux boot issues. In basic terms, it is a situation when the kernel can't load properly and therefore the system fails to boot. During the boot process, the kernel doesn't load directly. Instead, initramfs loads in RAM, then it points to the kernel (vmlinuz), and then the operating system boots. If initramfs gets corrupted or deleted at this stage because of recent OS patching, updates, or other causes, then we face a kernel panic.
Step 1: Reboot your machine again and select the rescue prompt.
Step 2: Go to /boot and list all files. Here you will see there is no initramfs file for your kernel, but there is an initramfs file for rescue by which you have booted your system, and another is for kdump.
Step 3: You will need to create a new initramfs file that corresponds to your kernel version.
Step 3.1: First check your kernel version using `#uname -r`.
Step 3.2: Next, run the dracut command: `#dracut -f <initrd-image> <kernal-version>`
Step 3.3: List the /boot directory contents again. The initramfs file for the kernel is now created.
Step 4: Now, when you boot normally, your machine starts without a kernel panic error.
Step 5: There might be a situation that occurs when you boot your system with a rescue image with creating a new initramfs file where you couldn't make a new file because it was already present.
Step 5.1: Run the mkinitrd command with the --force option and your kernel specification: `#mkinitrd --force <initrd-Image> <Kernel-Version>`
Step 6: you can now start your OS without any errors
<br>

**Question: Explain SSH connection.**<br>
**Technical Answer:** The Secure Shell (SSH) protocol is a method for securely sending commands to a computer over an unsecured network. SSH uses cryptography to authenticate and encrypt connections between devices. SSH also allows for tunneling, or port forwarding, which is when data packets are able to cross networks that they would not otherwise be able to cross. SSH is often used for controlling servers remotely, for managing infrastructure, and for transferring files. SSH runs on top of the TCP/IP protocol suite — which much of the Internet relies upon. TCP stands for Transmission Control Protocol and IP stands for Internet Protocol. TCP/IP pairs those two protocols in order to format, route, and deliver packets. IP indicates, among other information, which IP address a packet should go to (think of a mailing address), while TCP indicates which port a packet should go to at each IP address (think of the floor of a building or an apartment number).
TCP is a transport layer protocol: it is concerned with the transportation and delivery of data packets. Usually, additional protocols are used on top of TCP/IP in order to put the transmitted data in a form that applications can use. SSH is one such protocol. (Other examples include HTTP, FTP, and SMTP.)
<br>

**Question: Explain SSH Tunneling.**<br>
**Technical Answer:** SSH tunneling, or SSH port forwarding, is a method of transporting arbitrary data over an encrypted SSH connection. SSH tunnels allow connections made to a local port (that is, to a port on your own desktop) to be forwarded to a remote machine via a secure channel. When you connect to a server using SSH, you get a server's shell. This is the default behavior of an SSH connection. Under the hood, your SSH client creates an encrypted session between your SSH client and the SSH server. But the data transported within the SSH session can be of any type. For example, during shell access, the data transmitted are binary streams detailing dimensions of pseudo-terminal and ASCII characters to run commands on the remote shell. However, during SSH port forwarding, the data transmitted can be a binary stream of protocol tunneled over SSH. So SSH tunneling is just a way to transport arbitrary data with a dedicated data stream (tunnel) inside an existing SSH session. This can be achieved with either local port forwarding, remote port forwarding, dynamic port forwarding, or by creating a TUN/TAP tunnel.
<br>

**Question: Explain SSL handshake.**<br>
**Technical Answer:** TLS handshakes are a series of datagrams, or messages, exchanged by a client and a server. A TLS handshake involves multiple steps, as the client and server exchange the information necessary for completing the handshake and making further conversation possible.
The exact steps within a TLS handshake will vary depending upon the kind of key exchange algorithm used and the cipher suites supported by both sides. The RSA key exchange algorithm, while now considered not secure, was used in versions of TLS before 1.3. It goes roughly as follows:
* The 'client hello' message: The client initiates the handshake by sending a "hello" message to the server. The message will include which TLS version the client supports, the cipher suites supported, and a string of random bytes known as the "client random."
* The 'server hello' message: In reply to the client hello message, the server sends a message containing the server's SSL certificate, the server's chosen cipher suite, and the "server random," another random string of bytes that's generated by the server.
* Authentication: The client verifies the server's SSL certificate with the certificate authority that issued it. This confirms that the server is who it says it is, and that the client is interacting with the actual owner of the domain.
* The premaster secret: The client sends one more random string of bytes, the "premaster secret." The premaster secret is encrypted with the public key and can only be decrypted with the private key by the server. (The client gets the public key from the server's SSL certificate.)
* Private key used: The server decrypts the premaster secret.
* Session keys created: Both client and server generate session keys from the client random, the server random, and the premaster secret. They should arrive at the same results.
* Client is ready: The client sends a "finished" message that is encrypted with a session key.
* Server is ready: The server sends a "finished" message encrypted with a session key.
* Secure symmetric encryption achieved: The handshake is completed, and communication continues using the session keys.
<br>

**Question: Explain RTO and RPO in context of DR.**<br>
**Technical Answer:** RTO: Recovery Time Objective
A standard definition of RTO is the duration of time in which a business process must be restored after a disaster in order to avoid unacceptable consequences associated with a break in business continuity.
RPO: Recovery Point Objective
RPO is often defined as the maximum targeted period in which data might be lost from a disaster.
<br>

**Question: What are caches in CPU ?**<br>
**Technical Answer:** Cache is the amount of memory that is within the CPU itself, either integrated into individual cores or shared between some or all cores. It’s a small bit of dedicated memory that lives directly on the processor so that your CPU doesn’t need to fetch information from your system RAM every time you want to do something on your PC. Every processor has a small amount of cache, with smaller CPUs getting perhaps just a few kilobytes while large CPUs can have many megabytes worth of cache. Cache has its own hierarchy, or cache levels, which are split into L1, L2, and L3 cache. These are all kinds of cache, but they perform slightly different functions.
<br>

**Question: What are file descriptors ?**<br>
**Technical Answer:** In simple words, when you open a file, the operating system creates an entry to represent that file and store the information about that opened file. So if there are 100 files opened in your OS then there will be 100 entries in OS (somewhere in kernel). These entries are represented by integers like (...100, 101, 102....). This entry number is the file descriptor. So it is just an integer number that uniquely represents an opened file for the process. If your process opens 10 files then your Process table will have 10 entries for file descriptors.
Similarly, when you open a network socket, it is also represented by an integer and it is called Socket Descriptor.
<br>

**Question: How is Load Average of CPU calculated ?**<br>
**Technical Answer:** Load average reflect "system" load, that consider CPU load and I/O waiting. And this is most common parameter from which you need to start you performance issues troubleshooting. Use different metrics (disk load) and tools (e.g. iostat from sysstat package) to analyze system performance. To calculate CPU utilization use
```grep 'cpu ' /proc/stat | awk '{usage=100-($5*100)/($2+$3+$4+$5+$6+$7+$8)} END {print usage}'```
<br>

**Question: Explain difference between PID VS JOBID.**<br>
**Technical Answer:** The job identifier is given inside the square brackets. In this case, it's 1. That's the ID you'll use to bring it to the foreground and perform other administrative tasks. It's what identifies this job in the shell. UNIX/Linux shells make use of process groups: a process group is a set of processes that are somehow related (often by a linear pipeline, but as mentioned before, not necessarily the case). At any moment, you can have 0 or more background process groups, and at most one foreground process group (the shell controls which groups are in the background and which is in the foreground with tcsetpgrp(3)).
A group of processes is identified by a process group ID, which is the ID of the process group leader. The process group leader is the process that first created and joined the group by calling setpgid(2). The exact process that does this depends on how the shell is implemented, but in bash, IIRC, it is the last process in the pipeline.
<br>

**Question: What algorithm works while creating rsa ssh key ?**<br>
**Technical Answer:** Server is usually providing more different host key types, so you are targeting for compatibility. The order of priority in the client config is from the stronger to more compatible ones. RSA is still recommended as a gold standard (strong, wide compatible). 
<br>
