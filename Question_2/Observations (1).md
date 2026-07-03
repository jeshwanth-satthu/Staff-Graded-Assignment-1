```
=========================================================
OBSERVATIONS
Question 2 – Project Workspace Configuration
=========================================================
```

## `1. Command: mkdir` 

```
Observation:
```

```
The 'mkdir' command was used to create the project workspace and its
subdirectories (docs, src, and logs). This helped organize the project files
into separate folders for better management.
```

```
---------------------------------------------------------
```

## `2. Command: touch` 

```
Observation:
```

```
The 'touch' command created sample files inside each directory. These files
represent project documents, source code, and log files, confirming that the
workspace was created successfully.
```

```
---------------------------------------------------------
```

## `3. Command: ls -ld and ls -l` 

```
Observation:
```

```
The 'ls -ld' command displayed the permissions and ownership of the directories,
while 'ls -l' showed the permissions of the files. These commands were used to
verify the workspace before and after changing permissions.
```

```
---------------------------------------------------------
```

## `4. Command: chmod` 

```
Observation:
```

```
The 'chmod' command changed the directory permissions to 750 and the file
permissions to 640. This allows the owner full access, the group limited access,
and prevents unauthorized users from accessing the project files.
```

```
---------------------------------------------------------
```

## `5. Command: umask` 

```
Observation:
```

```
The 'umask' command displayed the default permission mask of the system. The
value 0022 indicates that newly created files and directories do not provide
write permission to the group or others by default.
```

```
---------------------------------------------------------
```

## `6. Overall Observation` 

```
Observation:
```

```
The project workspace was successfully created with secure permissions. Proper
ownership, restricted access, and the default umask settings help protect
project files while allowing controlled access to authorized users.
```

```
=========================================================
```

```
End of Observations
```

```
=========================================================
```

