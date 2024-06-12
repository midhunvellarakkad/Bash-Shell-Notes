# Bash Cheatsheet: Control Structures

## 1. If Statement
Check conditions with `if`:
```bash
age=18
if [ $age -ge 18 ]; then
  echo "You are an adult."
else
  echo "You are a minor."
fi
```

## 2. Comparison Operators
Use these in `[ ]`:
- `-eq` : Equal
- `-ne` : Not equal
- `-gt` : Greater than
- `-lt` : Less than
- `-ge` : Greater or equal
- `-le` : Less or equal

Example:
```bash
if [ 5 -gt 3 ]; then
  echo "5 is greater than 3"
fi
```

## 3. String Comparison
Compare strings with `=` or `!=`:
```bash
name="Bob"
if [ "$name" = "Bob" ]; then
  echo "Hello, Bob!"
fi
```

## 4. For Loop
Iterate over a list:
```bash
for i in 1 2 3; do
  echo "Number: $i"
done
```

## 5. While Loop
Loop while a condition is true:
```bash
count=1
while [ $count -le 5 ]; do
  echo "Count: $count"
  ((count++))
done
```

**Tip**: Always quote variables in `[ ]` to avoid errors if they’re unset.