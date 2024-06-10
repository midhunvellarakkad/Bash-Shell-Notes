# Bash Cheatsheet: Basics and Variables

## 1. Shebang
Start your script with a shebang to specify the interpreter:
```bash
#!/bin/bash
```

## 2. Comments
Add comments to explain your code:
```bash
# This is a single-line comment
```

## 3. Echo Command
Print text to the terminal:
```bash
echo "Hello, World!"
```

## 4. Variables
Define and use variables (no spaces around `=`):
```bash
name="Alice"          # Define a variable
echo "Hello, $name!"  # Use variable with $
```

## 5. Environment Variables
Access system variables:
```bash
echo $USER    # Prints current username
echo $PWD     # Prints current directory
```

## 6. Arithmetic
Perform basic math using `$(( ))`:
```bash
a=5
b=3
echo $((a + b))  # Outputs 8
echo $((a * b))  # Outputs 15
```

## 7. Read Input
Prompt user for input:
```bash
echo "Enter your name:"
read name
echo "Hi, $name!"
```

**Tip**: Variables are case-sensitive. Use `export` to make variables available to child processes.