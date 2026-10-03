# File Permissions in Linux

## Project Overview

This project demonstrates my practical experience managing file and directory permissions in Linux. The activity focused on reviewing permissions and modifying access according to specific security requirements.

## Objectives

* Check file and directory permissions, including hidden files.
* Remove unauthorized write permissions.
* Modify permissions for a hidden file.
* Restrict access to a directory to a specific user.

## Linux Commands Used

### Check file and directory permissions

```bash
ls -la
```

Displays files and directories, including hidden files, together with their permissions and ownership.

### Remove write permissions for others

```bash
chmod o-w *
```

Removes write permissions for other users from the files in the current directory.

### Modify hidden file permissions

```bash
chmod u-w,g-w .project_x.txt
chmod u+r,g+r .project_x.txt
```

Removes write permissions from the user and group and ensures that the user and group can read the hidden file.

### Restrict directory access

```bash
chmod go-rwx drafts
```

Removes all permissions for the group and other users, allowing only the owner to access the `drafts` directory.

## Skills Demonstrated

* Linux command line
* File and directory permissions
* `chmod`
* `ls`
* User, group, and other permissions
* Access control and authorization

## Summary

This project demonstrates how Linux permissions can be used to control access to files and directories. I practiced reviewing and modifying permissions to meet security requirements and protect files from unauthorized access.
