```
=========================================================
TECHNICAL OBSERVATIONS
=========================================================
```

```
1. Command:
echo "sample log line" > app.log
```

```
Observation:
```

```
A log file named app.log was created successfully.
```

```
---------------------------------------------------------
```

```
2. Command:
lsof | head -20
```

```
Observation:
The command displayed the first 20 open files and their associated processes.
```

```
---------------------------------------------------------
```

```
3. Command:
exec 3<app.log
```

```
Observation:
The log file was opened using file descriptor 3.
```

```
---------------------------------------------------------
```

```
4. Command:
lsof -p $$ | grep app.log
```

```
Observation:
The output confirmed that app.log was open through file descriptor 3.
```

```
---------------------------------------------------------
```

```
5. Command:
ls -l /proc/$$/fd
```

```
Observation:
The command displayed all file descriptors currently used by the shell,
including descriptors 0, 1, 2, and 3.
```

```
---------------------------------------------------------
```

```
6. Command:
ls -l > stdout.txt
```

```
Observation:
The standard output was redirected and stored in stdout.txt.
```

```
---------------------------------------------------------
```

```
7. Command:
ls /not_a_real_path 2> stderr.txt
```

```
Observation:
The error message was redirected to stderr.txt instead of appearing on the
terminal.
```

```
---------------------------------------------------------
```

```
8. Command:
(ls -l && ls /not_a_real_path) > combined.txt 2>&1
```

```
Observation:
```

```
Both standard output and standard error were redirected into combined.txt.
```

```
---------------------------------------------------------
```

```
9. Command:
ulimit -a
```

```
Observation:
```

```
The command displayed the current resource limits for the shell, including open
files, stack size, and CPU time.
```

```
---------------------------------------------------------
```

```
10. Command:
exec 3<&-
```

```
Observation:
```

```
The file descriptor 3 was closed successfully, releasing the open file.
```

```
=========================================================
End of Observations
```

```
=========================================================
```

