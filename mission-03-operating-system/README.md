# MISSION 3 — Understand the operating system
## 1. Task / objective
Mission objective: Explore the operating system, running processes, storage, paths and file permissions, and describe
the OS responsibilities.
What you must produce: Notes covering system information, process observations, paths, permissions and OS
responsibilities.
An operating system (OS) manages the computer's hardware and provides services to applications. macOS, Windows
and Linux are examples


## WORK COMPLETED
# task 3.1
 
 nformation	Command	What it tells you	What to write (privacy-safe)
OS / system details	
uname -a	Kernel name, version and hardware type	

Darwin VIDUSHIs-MacBook-Pro.local 25.3.0 Darwin Kernel Version 25.3.0: Wed Jan 28 20:54:05 PST 2026; root:xnu-12377.81.4~5/RELEASE_ARM64_T8142 arm64

Current account	 whoami	 The user account that is logged in and running commands	“It printed my username"


Storage. 	df -h	
Total, used and free disk space	
“The main disk showed about X GB total, Y used, Z available” 

/dev/disk5s1     100Mi    73Mi    27Mi    73%    574  4.3G    0%   /Volumes/Autodesk Fusion Installer 1


System activity; top -l 1 | head -15	
One snapshot of CPU use, memory use and running processes	
“It showed the number of processes, CPU usage and memory use”


# task 3.2 Processes

what is a process?
A program that is currently running. Each running program such as a browser or a terminal , i one or more processes

what does PID represent?
the process ID, a unique number the OS gives each process so it can track and manage it.

examples- 
* Google chrome - has its own PID and browsers often show several processes at once.
* VS Code - an application process that runs while the editor is open.

# task 3.3 paths and permissions 

absolute path - the full addres strating fro the root/
 /Users/[redacted]/Desktop/the-digital-detective-8553

relative path - address where you ar e currently 
mission-03-operating-system

In the ls -l output, find a line like -rw-r--r--. The first character is the file type, and the next three (rw-) are the owner’s permissions: read yes, write yes, execute no (-). Write what you actually see.

r (Read)	The file’s contents can be read	Opening a text file
w (Write)	The file can be changed	Editing a text file
x (Execute)	The file can be run, or a folder can be entered running a scipt

| OS responsibility | Your explanation | Example |

| Process management | Decides which programs run, when, and for how long on the CPU | Running Chrome and VS Code at the same time |
| Memory management | Gives each program its share of RAM and takes it back when the program closes | Closing an app frees its RAM |
| Device management | Controls hardware through drivers so programs can use it | Sending a document to a printer |
| File management | Organises how files and folders are stored, named, found and accessed | Saving a file in a folder on the SSD |
| User interface / shell | Lets the user interact with the computer, through a graphical interface or the terminal | Finder windows, or typing `ls` in the terminal |
| Security and permissions | Controls who can access files and resources | Needing a password to change system settings |

## 3. Commands / tools used
- uname -a: shows the operating system name, kernel version and hardware type.
- whoami: shows which user account is currently logged in.
- df -h: shows total, used and available disk space in readable sizes.
- top -l 1 | head -15: gives a one-time snapshot of CPU use, memory use and
  running processes. The pipe keeps only the first lines.
- ps aux | head -10: lists running processes with their PIDs.
- pwd: shows the full path of my current folder.
- cd: moves between my assignment folder and its subfolders.
- ls -l: shows a detailed listing, including permission letters.
- Activity Monitor: a graphical view of processes and their PIDs.
- VS Code: used to write this README.
- Git (status, add, commit, push): saved and uploaded this mission's work.

## 4. My understanding
- Operating system: it manages the hardware and gives services to programs.
  My computer runs macOS. uname showed [Darwin / arm64 or x86_64], and my
  username and device name are redacted.
- Storage: df -h showed that about [X GB] of [Y GB] is used, so I can see how
  much space is left before it runs out.
- Process: a program that is currently running. The PID is a unique number the
  OS gives each process so it can track and manage it. I saw Google Chrome (an
  application I opened) and launchd (a background process that macOS starts
  automatically). [Change these to what you really saw.]
- Absolute vs relative path: an absolute path starts from the root /, for
  example /Users/[redacted]/.../the-digital-detective-8553/mission-03-operating-system.
  A relative path starts from where I am, for example
  mission-03-operating-system/README.md.
- Permissions: in a line like -rw-r--r--, the first group after the file type
  belongs to the owner. rw- means the owner can read and write but not execute.
  I did not change any permissions.
- OS responsibilities: the OS handles processes, memory, devices, files, the
  user interface and security, so programs and users don't have to deal with
  the hardware directly.

## 5. Difficulties faced
No major difficulties.


## 6. How I resolved them
Not applicable.


## 7. Evidence / files
- mission-03-operating-system/README.md (system information table, process
  notes, paths and permissions, OS responsibilities table)
- All outputs have usernames and device names replaced with [redacted].

## 8. Commit details
- Commit message: Document operating system and file management
- Pushed to GitHub: YES