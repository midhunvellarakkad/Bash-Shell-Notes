# Bash Cheatsheet: Functions and Input/Output

## 1. Defining Functions
Create reusable code blocks:
```bash
greet() {
  echo "Hello, $1!"
}
greet "Alice"  # Calls function with argument
```

## 2. Function with Return
Use `return` for status codes:
```bash
check_number() {
  if [ $1 -gt 0 ]; then
    return 0  # Success
  else
    return 1  # Failure
  fi
}
check_number 5
echo $?  # Prints 0 (last command’s exit status)
```

## 3. Redirect Output
Save output to a file:
```bash
echo "Hello" > output.txt   # Overwrite
echo "World" >> output.txt  # Append
```

## 4. Pipe Output
Pass output to another command:
```bash
echo "Hello World" | grep "Hello"
```

## 5. Read from File
Read file content:
```bash
while read line; do
  echo "Line: $line"
done < input.txt
```

**Tip**: `$1`, `$2`, etc., represent function arguments. Use `$#` to get the number of arguments.