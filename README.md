# Staff Graded Assignment 1
## Command Line Interfaces and Scripting

### Student Information
- **Name:** Jeshwanth Sai Satthu
- **Course:** Command Line Interfaces and Scripting
- **Platform:** Coursera
- **Operating System:** Ubuntu (WSL2) on Windows 11

---

## Repository Structure

```
Staff-Graded-Assignment-1/
│
├── README.md
│
├── Question_1/
│   ├── Environment_Report.txt
│   ├── Observations.md
│   └── Screenshots/
│
├── Question_2/
│   ├── Project_Workspace_Report.txt
│   ├── Observations.md
│   ├── secure_workspace/
│   └── Screenshots/
│
├── Question_3/
│   ├── Link_Analysis_Report.txt
│   ├── Observations.md
│   ├── original.txt
│   ├── hardlink.txt
│   ├── symlink.txt
│   └── Screenshots/
│
├── Question_4/
│   ├── IO_Investigation_Report.txt
│   ├── Observations.md
│   ├── app.log
│   ├── stdout.txt
│   ├── stderr.txt
│   ├── combined.txt
│   └── Screenshots/
│
└── Question_5/
    ├── Storage_Assessment_Report.txt
    ├── Observations.md
    └── Screenshots/
```

---

## Assignment Summary

### Question 1 – Linux Environment Verification
- Verified username and groups
- Checked current shell
- Verified working directory
- Listed workspace contents
- Tested network connectivity

### Question 2 – Project Workspace and Permissions
- Created secure workspace
- Modified file and directory permissions
- Verified ownership
- Checked default umask
- Documented permission security

### Question 3 – Linux Links
- Created original file
- Created hard link
- Created symbolic link
- Compared inode numbers
- Observed link behavior after deleting the original file

### Question 4 – File Access and I/O Investigation
- Identified open files
- Examined file descriptors
- Performed output redirection
- Performed error redirection
- Verified resource limits

### Question 5 – Storage Health Assessment
- Identified storage devices
- Verified mounted file systems
- Checked disk usage
- Examined inode utilization
- Documented storage health
- Provided storage recommendations

---

## Linux Commands Used

- `whoami`
- `groups`
- `echo $SHELL`
- `pwd`
- `ls -la`
- `ping`
- `mkdir`
- `touch`
- `chmod`
- `ls -ld`
- `umask`
- `ln`
- `ln -s`
- `ls -li`
- `stat`
- `cat`
- `rm`
- `lsof`
- `ulimit`
- `df -h`
- `df -i`
- `lsblk`
- `mount`
- `vi`

---

## Notes

- All tasks were completed using Ubuntu running on Windows Subsystem for Linux (WSL2).
- Each question includes the required report, observations, and screenshots.
- Supporting files generated during the exercises are included where applicable.
- This repository is organized according to the assignment submission requirements.

---

**Submitted for:** Staff Graded Assignment 1  
**Course:** Command Line Interfaces and Scripting
