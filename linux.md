# Linux Command-Line Cheatsheet (Compact)

| **File Operations**           | **Directory Operations**      | **Permissions**               |
|--------------------------------|-------------------------------|--------------------------------|
| `ls` List files               | `pwd` Show current directory  | `chmod [mode] file` Change permissions |
| `cp src dest` Copy file       | `cd dir` Change directory     | `chown user:group file` Change ownership |
| `mv src dest` Move/Rename file| `mkdir dir` Create directory  | `umask` Show default permissions |
| `rm file` Delete file         | `rmdir dir` Remove empty dir  | `sudo` Run as superuser        |
| `touch file` Create empty file| `tree` Display dir structure  |                                |

---

| **Process Management**        | **Search and Filters**         | **Compression**               |
|--------------------------------|-------------------------------|--------------------------------|
| `ps aux` List processes       | `grep pattern file` Search text | `tar -cvf file.tar files` Archive |
| `top` Monitor system          | `find dir -name name` Find file | `tar -xvf file.tar` Extract archive |
| `kill PID` Kill process       | `locate name` Locate file      | `gzip file` Compress with gzip |
| `pkill name` Kill by name     | `cat file` View file contents  | `gunzip file.gz` Decompress gzip |
| `jobs` Background processes   | `head/tail file` File start/end| `zip -r file.zip dir` Zip a dir |

---

| **Networking**                | **Disk Usage**                | **System Information**         |
|--------------------------------|-------------------------------|---------------------------------|
| `ping host` Test connectivity | `df -h` Disk usage summary    | `uname -a` System info         |
| `curl URL` Download content   | `du -sh dir` Size of directory| `uptime` System uptime         |
| `wget URL` Download file      | `mount` Mount a drive         | `who` Active users             |
| `ifconfig` Show IP address    | `umount` Unmount drive        | `whoami` Current user          |
| `netstat -tuln` Open ports    | `lsblk` List block devices    | `dmesg` Kernel log             |

---

| **User Management**           | **Package Management**        | **Miscellaneous**              |
|--------------------------------|-------------------------------|---------------------------------|
| `whoami` Show current user     | `apt-get install pkg` Install package | `alias name='command'` Create alias |
| `id` Show user/group info      | `yum update pkg` Update package | `history` Command history      |
| `passwd` Change password       | `pacman -S pkg` Install (Arch)| `echo text` Print to console    |
| `adduser user` Add new user    | `dpkg -i pkg.deb` Install DEB | `date` Show current date/time  |
| `deluser user` Remove user     | `rpm -i pkg.rpm` Install RPM  | `cal` Display calendar         |

---

| **File Viewing/Editing**      | **Archive & Backup**          | **Shell Basics**               |
|--------------------------------|-------------------------------|---------------------------------|
| `cat file` View file contents | `tar -czf file.tgz files` Create tarball | `exit` Exit shell            |
| `less file` Paginate view     | `tar -xzf file.tgz` Extract tarball | `clear` Clear terminal        |
| `nano file` Edit file         | `rsync src dest` Sync files    | `!!` Repeat last command       |
| `vim file` Edit with Vim      | `scp src user@host:dest` Secure copy | `&` Run command in background |
| `head/tail file` Start/End    | `crontab -e` Edit cron jobs    | `|` Pipe output                |

---

### Notes:
- `Ctrl+C` to cancel a running process.
- `Ctrl+Z` to suspend a process.
- Use `man [command]` for detailed help.
- Replace `apt-get`, `yum`, or `pacman` based on your Linux distro.

This layout keeps everything concise for quick reference in a single window. Let me know if you'd like specific additions!
