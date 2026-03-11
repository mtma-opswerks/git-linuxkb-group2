# 🖥️ Process Monitoring Commands

A quick reference guide for the most common and useful Linux process monitoring commands.

---

## 1. `ps` — Snapshot of Current Processes

**Description:** Prints a static snapshot of currently running processes. The `aux` flags show all processes for all users with detailed info.

```bash
ps aux
```

---

## 2. `vmstat` — System Performance Overview

**Description:** Reports information about system processes, memory, paging, block I/O, and CPU activity. Great for spotting overall system bottlenecks.

```bash
vmstat 2 5
```

---

## 3. `pidstat` — Per-Process Resource Statistics

**Description:** Reports statistics for individual tasks managed by the Linux kernel, including CPU, memory, and I/O usage per process.

```bash
pidstat -u 2
```

---

## 4. `kill` — Terminate a Process by PID

**Description:** Sends a signal to a process to stop it. The `-9` flag forces an immediate kill, useful when a process is unresponsive.

```bash
kill -9 1234
```

---

## 5. `strace` — Trace System Calls of a Process

**Description:** Tracks and displays all system calls made by a process in real time. Invaluable for debugging misbehaving or hanging processes.

```bash
strace -p 1234
```

---

> 💡 **Tip:** `vmstat` and `pidstat` are part of the `sysstat` package. Install with `sudo apt install sysstat` if not available.
