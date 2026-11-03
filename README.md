# 🚀 WorkspaceOps – Linux User Workspace Management System

**WorkspaceOps** is a Bash-based Linux administration tool designed to simplify user workspace management, storage monitoring, file searching, and automated archiving.

It provides a menu-driven interface that allows administrators to create organized user workspaces, monitor disk usage, locate files across multiple directories, and archive inactive workspaces.

## ✨ Features

### 1. 👤 User Workspace Creation
- Create dedicated workspaces for individual users.
- Automatically generate three subdirectories:
  - `docs/` – Document storage.
  - `code/` – Source code and development files.
  - `shared/` – Shared workspace files.
- Apply restricted directory permissions using `chmod 700`.

### 2. 💾 Disk Usage Monitoring
- Monitor workspace storage using the Linux `du` command.
- Display current storage consumption in MB.
- Generate a warning when workspace usage exceeds 100 MB.
- Help administrators keep track of workspace storage.

### 3. 🔍 File Search System
- Search files across all user workspaces.
- Search using filenames or file extensions.
- Display useful file information:
  - File path
  - File size
  - Last modification date and time

### 4. 📦 Automated Workspace Archiving
- Identify workspaces whose directories have not been modified for 60 days.
- Compress inactive workspaces into `.tar.gz` archives.
- Store archived workspaces in `/archives`.
- Provide an option to delete the original workspace after archiving.

## 🛠️ Technologies & Linux Commands

| Technology / Command | Purpose |
|---|---|
| Bash Scripting | Automation and menu-driven interface |
| `mkdir
