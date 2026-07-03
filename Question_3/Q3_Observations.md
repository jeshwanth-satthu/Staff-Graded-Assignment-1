```
=========================================================
OBSERVATIONS
Question 3 – Linux Links
```

```
=========================================================
```

## `1. Command:` 

```
echo "This is the original file." > original.txt
```

```
Observation:
```

```
The command created a new file named original.txt and stored the text "This is
the original file." in it. This file was used as the source for creating both
the hard link and the symbolic link.
```

```
---------------------------------------------------------
```

## `2. Command:` 

```
cat original.txt
```

```
Observation:
```

```
The command displayed the contents of original.txt, confirming that the file was
created successfully and contained the expected text.
```

```
---------------------------------------------------------
```

## `3. Command:` 

```
ln original.txt hardlink.txt
```

```
Observation:
```

```
The command created a hard link named hardlink.txt. This hard link shares the
same inode number and points to the same file data as the original file.
```

```
---------------------------------------------------------
```

## `4. Command:` 

```
ln -s original.txt symlink.txt
```

```
Observation:
```

```
The command created a symbolic link named symlink.txt. The symbolic link stores
the path to the original file and has its own inode number.
```

```
---------------------------------------------------------
```

## `5. Command:` 

```
ls -li
```

```
Observation:
```

```
The command displayed inode numbers for all files. It showed that original.txt
and hardlink.txt shared inode number 44953, while symlink.txt had a different
inode number (44954).
```

```
---------------------------------------------------------
```

## `6. Command:` 

```
stat original.txt hardlink.txt symlink.txt
```

```
Observation:
```

```
The command displayed detailed metadata including inode number, file type,
permissions, ownership, file size, and timestamps. The original file and hard
link shared the same inode and metadata, while the symbolic link had different
metadata.
```

```
---------------------------------------------------------
```

## `7. Command:` 

```
cat hardlink.txt
```

```
Observation:
```

```
The command displayed the same contents as the original file, confirming that
the hard link accesses the same file data.
```

```
---------------------------------------------------------
```

## `8. Command:` 

```
cat symlink.txt
```

```
Observation:
```

```
The command successfully displayed the contents of the original file through the
symbolic link, confirming that the link was working correctly.
```

```
---------------------------------------------------------
```

## `9. Command:` 

```
rm original.txt
```

```
Observation:
```

```
The command deleted the original file name from the directory. However, the
actual file data still existed because the hard link continued to reference the
same inode.
```

```
---------------------------------------------------------
```

## `10. Command:` 

```
ls -li
```

```
Observation:
```

```
The command showed that original.txt was removed. The hard link still existed
with inode number 44953, while the symbolic link pointed to a missing target
(original.txt).
```

```
---------------------------------------------------------
```

## `11. Command:` 

```
cat hardlink.txt
```

```
Observation:
```

```
The command displayed "This is the original file.", proving that the hard link
```

```
remained functional even after the original file was deleted.
```

```
---------------------------------------------------------
```

```
12. Command:
```

```
cat symlink.txt
```

```
Observation:
```

```
The command returned the error "No such file or directory" because the symbolic
link pointed to the deleted original file. This confirmed that symbolic links
depend on the existence of the target file.
```

```
=========================================================
End of Observations
```

```
=========================================================
```

