# Bash Cheatsheet: File Operations and Text Processing

## 1. Check File Existence
Test if a file or directory exists:
```bash
if [ -f "file.txt" ]; then
  echo "File exists"
fi
if [ -d "mydir" ]; then
  echo "Directory exists"
fi
```

## 2. File Tests
Common test operators:
- `-f` : File exists
- `-d` : Directory exists
- `-r` : Readable
- `-w` : Writable
- `-x` : Executable

## 3. Create/Delete Files
Manage files:
```bash
touch newfile.txt      # Create empty file
rm file.txt            # Delete file
mkdir mydir            # Create directory
rm -r mydir            # Delete directory
```

## 4. Grep
Search text in files:
```bash
grep "error" log.txt   # Find lines with "error"
grep -i "error" log.txt  # Case-insensitive
```

## 5. Awk and Sed
Process text:
```bash
awk '{print $1}' file.txt  # Print first column
sed 's/old/new/g' file.txt # Replace "old" with "new"
```

**Tip**: Use `man grep` or `man awk` for detailed options.