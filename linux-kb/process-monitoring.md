# 🖥️ Process Monitoring Commands

A quick reference guide for the most common and useful Linux process monitoring commands.

---

## 1. `top` — Real-Time Process Viewer

**Description:** Displays a live, dynamic view of running processes including CPU and memory usage. Refreshes every few seconds automatically.

```bash
top
```

---

## 2. `ps` — Snapshot of Current Processes

**Description:** Prints a static snapshot of currently running processes. The `aux` flags show all processes for all users with detailed info.

```bash
ps aux
```

---

## 3. `kill` — Terminate a Process by PID

**Description:** Sends a signal to a process to stop it. The `-9` flag forces an immediate kill, useful when a process is unresponsive.

```bash
kill -9 1234
```

---

## 4. `htop` — Interactive Process Monitor

**Description:** An enhanced, user-friendly alternative to `top` with color-coded output, mouse support, and easier process management.

```bash
htop
```

---

## 5. `lsof` — List Open Files and Processes

**Description:** Lists all open files and the processes using them. Useful for finding which process is using a specific port or file.

```bash
lsof -i :8080
```

---

> 💡 **Tip:** Use `q` to quit `top` and `htop`. Run `sudo` before commands if you need to inspect or kill processes owned by other users.

