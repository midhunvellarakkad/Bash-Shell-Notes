# Bash Cheatsheet: Common Commands and Tips

## 1. Navigation
Move around the filesystem:
```bash
pwd               # Print current directory
ls                # List files
cd /path/to/dir   # Change directory
cd ..             # Go up one directory
```

## 2. File Viewing
View file contents:
```bash
cat file.txt      # Print entire file
less file.txt     # View file interactively
head -n 5 file.txt  # First 5 lines
tail -n 5 file.txt  # Last 5 lines
```

## 3. Permissions
Manage file permissions:
```bash
chmod +x script.sh  # Make script executable
chmod 644 file.txt  # Set read/write for owner, read for others
```

## 4. Exit Codes
Check command success:
```bash
ls /nonexistent
echo $?  # Prints non-zero (error)
```

## 5. Debugging Scripts
Run with debugging:
```bash
bash -x script.sh  # Trace execution
```

**Tip**: Combine commands with `&&` (run if previous succeeds) or `||` (run if previous fails).