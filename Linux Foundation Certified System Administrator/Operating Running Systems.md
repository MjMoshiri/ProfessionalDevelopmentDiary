# Part 1, Module 3: [Operating Running Systems](https://learning.oreilly.com/course/linux-foundation-certified/9780138230678/)

#### Networking Tools
- `nmcli`: Command-line interface for NetworkManager.
- `nmtui`: Text-based UI for NetworkManager.
- `hostnamectl`: Controls the system hostname and related settings.

#### DNS and Network Diagnostics
- `dig`: DNS lookup utility.
- `ss`: Utility to investigate sockets.
- `nmap -sn`: Network scanning tool to discover hosts on a network.

#### Systemctl Commands
- `systemctl`: Controls the systemd system and service manager.
  - `status`: Shows the status of a systemd unit (e.g., `status http`).
  - `start`: Starts a systemd unit.
  - `stop`: Stops a systemd unit.
  - `enable`: Enables a systemd unit to start at boot.
  - `isolate`: Changes the system state to a specific target.
  - `list-dependencies`: Lists a unit's dependencies.
  - `list-units`: Lists all units.

#### Package Management
- `ldd`: Lists dynamic dependencies of an executable.
- `dnf provide */command or package`: Shows which package provides a command.
- `rpm`: RPM package manager.
  - `rpm -qf /path/to/file`: Shows which package owns a file.
  - `rpm -ql package`: Lists files in a package.
  - `rpm -qpi package`: Shows package information (not necessarily installed).
  - `rpm -e package`: Removes a package.

#### Security and Configuration
- `ufw`: Uncomplicated Firewall, a front-end for `iptables`.
- `semanage`: SELinux policy management tool.
- `/etc/sysconfig/selinux`: Contains SELinux configuration.
- `/etc/ssh/sshd_config`: SSH daemon configuration file.
- `ssh-copy-id`: Installs SSH keys on a server.

#### Time Management
- `timedatectl`: Controls the system time and date.
- `hwclock`: Manages the hardware clock.
- `date +%d-%m`: Displays the date in a specific format.

#### Signal Handling
- `SIGTERM 15`: Graceful termination signal.
- `SIGKILL 9`: Immediate termination signal.
- `man 7 signal`: Displays signal information.

#### Monitoring Tools
- `top`: Task manager.
  - `f`: Change settings.
  - `k`: Kill a process.
  - `r`: Renice a process.
  - `w`: Save current settings.
  - `q`: Quit.

#### Process Priority and Management
- `nice`: Runs a program with modified scheduling priority.
- `killall`: Kills processes by name.

#### Task Scheduling
- `cron`: Schedules tasks to run at intervals.
- `at`: Schedules tasks to run at a specific time.
- `systemd timers`: Systemd-based task scheduling.

#### Logging and Journaling
- `rsyslogd`: System logging daemon. `/etc/rsyslog.conf` is the configuration file.
- `systemd-journald`: Systemd journaling service. `/var/log/journal` is the journal directory and `/etc/systemd/journald.conf` is the configuration file.

**Tags**: Linux
