# Part 1, Module 2: [User and Group Management](https://learning.oreilly.com/course/linux-foundation-certified/9780138230678/)

- `useradd -m`: Ensures that the user has a home directory.
- `getent`: Retrieves entries from databases configured in `/etc/nsswitch.conf`.
- `chage`: Changes the user password expiry information.
- `man 5 shadow`: Displays the format of the `/etc/shadow` file.
- Pluggable Authentication Modules (PAM): A framework for integrating multiple low-level authentication schemes into a high-level API.
- Storage Area Network (SAN) with Internet Small Computer System Interface (iSCSI) 
#### Important Files and Directories
- `/etc/group`: Contains group information such as group name, group ID, and group members.
- `/etc/login.defs`: Configuration file for the `useradd` command. (`useradd -D` for default settings)
- `/etc/skel`: Directory containing files and directories to be copied to a new user's home directory.

#### Editors for System Files
- `vigr`: Safely edits the `/etc/group` file.
- `vipw`: Safely edits the `/etc/passwd` and `/etc/shadow` files.

#### Systemd Management
- `loginctl`: Manages systemd login sessions.
    - `list-sessions`: Lists current sessions.
    - `list-users`: Lists current users.

#### File Permissions and Masks
- `chmod u+s,+t`: Sets the SUID and sticky bit.
- `umask`: Sets default file creation permissions.

#### Storage and File Systems
- `fdisk`: Manipulates the MBR partition table.
- `gdisk`: Manipulates the GPT partition table.
- `mkfs.xfs`, `mkfs.ext4 /dev/sdb1`: Creates a file system on a partition.
- `lsof`: Lists open files. (Useful for troubleshooting unmounting issues)
- `/etc/fstab`: Configuration file that contains information about disk drives and partitions.(Useful for automounting on boot)
