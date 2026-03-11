# 👤 User Management Commands

A quick reference guide for the most common and useful Linux user management commands.

---

## 1. `useradd` — Create a New User

**Description:** Creates a new user account on the system. Use the `-m` flag to automatically generate a home directory.

```bash
sudo useradd -m john
```

---

## 2. `passwd` — Set or Change a User's Password

**Description:** Sets or updates the password for a specified user account. Running it without a username changes the current user's password.

```bash
sudo passwd john
```

---

## 3. `usermod` — Modify a User Account

**Description:** Modifies an existing user's account properties such as username, home directory, or group memberships. The `-aG` flag appends the user to a supplementary group.

```bash
sudo usermod -aG sudo john
```

---

## 4. `userdel` — Delete a User Account

**Description:** Removes a user account from the system. Use the `-r` flag to also delete the user's home directory and mail spool.

```bash
sudo userdel -r john
```

---

## 5. `id` — Display User Identity Information

**Description:** Prints the user ID (UID), group ID (GID), and all group memberships for a specified user. Useful for verifying permissions and group assignments.

```bash
id john
```

---

> 💡 **Tip:** Always use `sudo` for user management commands, as they require root privileges.

