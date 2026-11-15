# Mission 3 - Understand the operating system

## Task 3.1 - Explore your operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
|---|---|---|
| Operating system / system details | Identifies the OS name, kernel release, and hardware architecture. | macOS (Darwin 27.2.0, arm64, Apple Silicon) |
| Current account identity | Identifies the active user account currently logged into the session. | `[redacted]` |
| Available and used storage | Displays total disk size, used space, available free space, and mount points. | `/dev/disk3s1s1`: 460 GiB total, ~13 GiB used (~4% capacity), ~310 GiB available |
| System activity snapshot | Shows real-time CPU usage, memory utilization, load averages, and count of active/sleeping processes. | 605 total processes (2 running, 603 sleeping), Load Avg ~2.17, CPU ~4.9% user, ~10.1% sys, ~84.9% idle |

## Task 3.2 - Understand processes

- **What is a process?**  
  A process is an active instance of a computer program that is currently being executed by the operating system. It includes the program code, its current activity, and its allocated memory and system resources.

- **What does the PID column represent?**  
  The PID stands for Process Identifier. It is a unique number assigned by the operating system kernel to identify and track each running process during its execution.

- **Two examples of processes running on the computer:**
  1. *Application process:* Google Chrome (`Google Chrome`, PID 16192) or VS Code (`Code`) — an interactive user-facing application.
  2. *Background process:* `launchd` (PID 1) — the primary init/daemon management process on macOS that starts and manages background system services.

## Task 3.3 - Understand paths and permissions

- **Difference between an absolute path and a relative path:**
  - An **absolute path** specifies the complete location of a file or folder starting from the root directory (`/`). It is independent of the current working directory.  
    *Example from assignment folder:* `/Users/[redacted]/Downloads/digital-detective-8443/mission-03-operating-system`
  - A **relative path** specifies the location of a file or folder in relation to the current directory where the user or command is operating.  
    *Example from assignment folder:* From `digital-detective-8443`, navigating to `terminal-practice/original.txt` or using `cd mission-03-operating-system`.

- **File permissions observation:**  
  Inspecting `terminal-practice/original.txt` with `ls -l` showed `-rw-r--r--`.  
  The owner permission triplet is `rw-`:
  - `r` (Read): Yes, the owner can view and read the file's contents.
  - `w` (Write): Yes, the owner can edit, modify, and save changes to the file.
  - `-` (Execute): No, the file cannot be executed as a program or script by the owner.

| Permission | Meaning | Example |
|---|---|---|
| `r` — Read | Allows a file's contents to be read. | Opening a text file to read its contents. |
| `w` — Write | Allows a file to be changed or overwritten. | Editing and saving changes in a text file. |
| `x` — Execute | Allows a file to be run; on a directory, allows access/traversal. | Running an executable script or opening a folder. |

## Task 3.4 - Operating-system responsibilities

| OS responsibility | Your explanation | Example |
|---|---|---|
| Process management | Controls creating, scheduling, running, and terminating processes, distributing CPU time so programs run concurrently without conflicts. | Scheduling CPU time between a web browser and a text editor so both stay responsive. |
| Memory management | Allocates and tracks physical RAM for active programs and frees memory when programs close, keeping program memory spaces isolated. | Allocating RAM when launching VS Code and freeing it when exiting the editor. |
| Device management | Coordinates and controls peripheral hardware devices using device drivers, translating application requests into hardware commands. | Translating keypresses from a keyboard into text and sending display output to a monitor. |
| File management | Manages how files and directories are organized, stored, named, retrieved, and protected on secondary storage drives. | Organizing files into folders like `digital-detective-8443/mission-03-operating-system/README.md` on the SSD. |
| User interface / shell | Provides an interface (graphical GUI or text-based CLI shell) that allows human users to interact with and control the system. | Using macOS Finder / Desktop (GUI) or typing commands in the zsh Terminal (CLI). |
| Security and permissions | Restricts access to data and system resources by verifying user credentials and enforcing read, write, and execute permissions. | Requiring password / Touch ID authentication to modify system settings and enforcing `rw-r--r--` permissions. |

## 1. Task / objective

Explore the operating system, running processes, storage, paths, and file permissions, and describe the core responsibilities of an operating system.

## 2. Work completed

Explored operating system details, checked user identity and disk storage, observed active system processes and PIDs, analyzed absolute vs. relative paths, inspected file owner permissions (`rw-`), and explained the key responsibilities of an operating system with examples.

## 3. Commands / tools used

- `uname -srm`: Displayed the OS kernel name, release version, and hardware architecture.
- `sw_vers`: Showed macOS product name and version details.
- `whoami`: Checked the active user account identity.
- `df -h /`: Inspected storage capacity, used space, and free space on the primary disk.
- `top -l 1 | head -n 12`: Captured a single snapshot of system resource usage, load average, and active/sleeping process counts.
- `ps -A -o pid,comm`: Inspected running processes, PIDs, and identified application and background processes.
- `ls -l`: Examined file permissions, owner details, and file size in `terminal-practice/`.
- `pwd`: Displayed the current absolute working directory.
- `cd`: Navigated between the project folder and subfolders using relative paths.

## 4. My understanding

The operating system acts as the primary layer between hardware and user software. It coordinates the CPU by scheduling processes, manages memory so applications run safely in isolated spaces, organizes storage using a hierarchical file system, and enforces security through user permissions (`r`, `w`, `x`). Every active program receives a unique PID to allow tracking and management.

## 5. Difficulties faced

No major difficulties. Ensured that private machine information and user account names were kept confidential and redacted before documenting evidence.

## 6. How I resolved them

Replaced sensitive usernames and machine identifiers with `[redacted]` to comply with privacy rules for public repository submissions.

## 7. Evidence / files

- `mission-03-operating-system/README.md`
- `terminal-practice/original.txt`

## 8. Commit details

Commit message: `Document operating system and file management`

The completed Mission 3 work was committed and pushed to GitHub on the main branch.
