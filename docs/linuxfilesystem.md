# Linux Filesystem
------------------------------------------------
The Linux file system is place in a computer, in which all files and programs are neatly stored. It's like a tree, where the tree trunk is called "root" and the leaves are all the other files and programs.

### **Here's a picture of it to understand it better:**

![ ](../images/linux_filesystem.jpg)

## Filesystem Explained:

### /bin:
- Contains fundamental user commands
- These commands provide the basic functionality to interact with the filesystem
- Examples: ls, cat, cp, etc.

### /boot:
- Stores files needed to start the system
- Contains the Linux kernel and bootloader settings

### /dev:
- Represents hardware devices as files
- Lets programs interact with hardware like hard drives or keyboards

### /etc:
- Keeps system and application settings
- Contains configuration files that control how the system works

### /home:
- Contains personal directories for users (each user has one)
- Stores user-specific files, documents, and settings
- Provides separation for user data and ensures security

### /lib:
- Contains shared library images needed to boot the system and run the commands in the root filesystem

### /media & /mnt:
- Used for mounting external and temporary filesystems
- /media: typically for removable media like USB drives
- /mnt: for temporary filesystems, such as network shares, etc.

### /opt:
- Designed for optional, third-party software installations
- Examples: Google Chrome, Webex, etc.

### /sbin:
- Holds system tools for administrators
- Used for managing disks, networks, and system settings

### /usr:
- Stores programs and files for users
- Includes applications, libraries, etc.
- Example: programming languages like python, etc.

### /var:
- Holds variable data that grows over time
- Includes logs, temporary files, etc.

### /tmp:
- For temporary files
- Files are typically deleted after a reboot or after certain period