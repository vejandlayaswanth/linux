# 🔐 Private File System on AWS EC2

This project sets up a secure file system structure on an AWS EC2 instance using Linux commands, users/groups, ACLs, and a simple HTTP server.

## 💡 Features
- Users & groups for controlled access
- Private, Shared, and Backup folders
- File and directory permissions with `chmod`, `chgrp`, and `setfacl`
- Python HTTP server to serve files over port 8080
- Secure Backup folder restricted to root

## 📂 Folder Structure
- `Private/` → Only owner can access
- `Shared/`  → Shared with group `myfam`
- `Backup/`  → Only `root` can access

## 🌐 Access
Start the HTTP server with:
```bash
cd ~/Shared
python3 -m http.server 8080
