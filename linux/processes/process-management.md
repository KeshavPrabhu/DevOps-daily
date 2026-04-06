#  Process Management in Linux (Detailed Guide)

---

## What is a Process?

A process is a running instance of a program.
Each process in Linux is uniquely identified by a **PID (Process ID)**.

---

## 🔑 Key Concepts

- **PID (Process ID)** → Unique ID of process  
- **PPID (Parent Process ID)** → ID of parent process  
- **TTY** → Terminal associated with process  
- **Foreground Process** → Runs in terminal  
- **Background Process** → Runs in background (`&`)  
- **Daemon** → Background service (e.g., sshd, nginx)  

---

## Viewing Processes

1. `ps` command

```bash
ps
ps aux
ps -ef

Explanation of ps aux columns:
Column	    Meaning
USER	    Owner of process
PID	    Process ID
%CPU	    CPU usage
%MEM	    Memory usage
VSZ	    Virtual memory
RSS	    Physical memory
TTY	    Terminal
STAT	    Process state
COMMAND	    Command


2. top command (Real-time monitoring)

"top"

--Shows live system stats
--Press q to exit


3. htop (Improved version of top)

"htop"

--Interactive UI
--Easier to kill processes


⚙️  Process States

State	Meaning
R	Running
S	Sleeping
D	Uninterruptible sleep
Z	Zombie
T	Stopped 
