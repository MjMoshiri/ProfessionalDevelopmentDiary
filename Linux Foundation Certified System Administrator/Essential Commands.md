# Part 1, Module 1: [Essential Commands](https://learning.oreilly.com/course/linux-foundation-certified/9780138230678/)

- **Man Page Utilities**:
  - `man -k keyword`: Search the short descriptions and manual page names for the keyword.
  - `apropos keyword`: Equivalent to `man -k`.
  - `mandb`: Rebuilds the manual page database; this is essential after installing new man pages.
- #### Man Pages Group
    - **1**: User commands that may be started by anyone.
    - **5**: File formats and conventions, e.g., `/etc/passwd`.
    - **8**: System administration commands that are typically only for root.

- `pinfo`: An info viewer with a menu-driven interface, alternative to traditional man pages.
- `tldr`: TD;LR guides for common commands (limited availability).

#### File Management
- `find -exec cmd {} \;`: Execute `cmd` on each file found by `find`. Replace `{}` with the file name.
- `locate`: Searches a pre-built database of files and directories. Run `updatedb` to update the database.
- `tar`: A versatile archiving utility capable of creating and manipulating archive files. `v` for verbose output, `f` for file.
  - `tar cvf archive.tar files`: Creates an archive.
  - `tar xvf archive.tar`: Extracts an archive.
  - `tar tvf archive.tar`: Lists the contents of an archive.
  - Options:
    - `-C`: Changes to a directory before performing an operation.(Useful for extracting to a specific directory.)
    - `-z`: Uses gzip compression.
    - `-j`: Uses bzip2 compression.
    - `-J`: Uses xz compression.
- `ln`: Creates a link to a file or directory.
  - `-s`: Creates a symbolic link.
  - `-f`: Removes existing destination files.
- `findmnt`: Displays target mount point for all currently mounted file systems.
- `df -h`: Displays disk space usage in a human-readable format.
- `lsblk`: Lists information about all available block devices.

#### Text Processing
- `grep`:
  - `-i`: Ignore case distinctions in both the pattern and the input files.
  - `-v`: Invert the match, showing only lines that do not match.
  - `-A 2`, `-B 2`, `-C 2`: Context control; shows 2 lines after, before, or around the matched line.
  - `-E`: Interpret pattern as an extended regular expression (ERE).
- `cut -d ':' -f 3 /etc/passwd`: Extracts the third field from lines in `/etc/passwd` using `:` as the delimiter.
- `awk`: A versatile text processing tool that can be used to manipulate text files.
  - `awk -F ':' '{print $3}' /etc/passwd`: Prints the third field of each line in `/etc/passwd`.
#### System Configuration
- `visudo`: Edits the sudoers file in a safe manner, preventing configuration errors.
  - Example: Set `timestamp_timeout` to 240 minutes to extend sudo timeout.
- `tee filename`: Reads from standard input and writes to standard output and files, useful for logging.

#### System Components
- `glibc`: The GNU C Library; this is a core part of the Linux operating system, providing essential system functions.
- `systemd`: A system and service manager for Linux, providing aggressive parallelization capabilities and the use of socket and D-Bus activation for starting services.

#### File System Hierarchy
- [File System Hierarchy Standard](https://refspecs.linuxfoundation.org/FHS_3.0/fhs/index.html): The standard file system structure used by Linux.
- `man hier`

#### Profile and Shell Scripts
- `/etc/profile`: System-wide.
- `.bash_profile`: User-specific.
- `.bashrc`: User-specific, executed for non-login shells.
