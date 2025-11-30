# Experiment 11: Shell Programming – Advanced String & File Operations
### Name: Arjun
### Roll No.: 590029204
### Date: 2025-11-05
---
## Aim
To write and execute shell scripts for advanced string manipulation, file processing, menu-driven
systems, and dictionary-based word validation.
---
## Requirements
- Linux system with Bash shell
- Commands: `grep`, `cut`, `awk`, `rev`, `tr`, `df`, `free`, `cal`, `date`
- Dictionary file at `/usr/share/dict/words` (for dictionary check task)
---
# Exercise 1: Split Sentence into Words
### Task Statement
Write a shell script to split a sentence into individual words and print them one per line.
### Script
```bash
#!/bin/bash
echo "Enter a sentence:"
read sentence
for word in $sentence; do
echo "$word"
done
```
### Explanation
- When `$sentence` is **unquoted**, Bash performs word splitting automatically based on the **IFS
(Internal Field Separator)**.
- By default, it splits on spaces, tabs, and newlines.
- Each word becomes a separate iteration of the loop.

### Output
<img width="1147" height="635" alt="image" src="https://github.com/user-attachments/assets/d55d61e9-52c1-4002-a3a0-e383ef699839" />


---
# Exercise 2: Palindrome Check
### Task Statement
Write a script that checks whether a given string is a palindrome.
### Script
```bash
#!/bin/bash
echo "Enter string:"
read str
rev=$(echo "$str" | rev)
if [ "$str" = "$rev" ]; then
echo "Palindrome"
else
echo "Not palindrome"
fi
```
### Explanation
- The `rev` command reverses a string character by character.
- Comparison checks if the original string equals the reversed one.
- This comparison is **case-sensitive** and includes spaces.
### Output
<img width="978" height="562" alt="image" src="https://github.com/user-attachments/assets/6cc1b0a1-1a59-46e6-a288-34955f5cd75b" />



---
# Exercise 3: Interactive Menu System
### Task Statement
Create a menu-driven script that allows users to display system information.
### Script
```bash
#!/bin/bash
show_date() {
echo "Current date and time: $(date)"
}
show_calendar() {
echo "Current month calendar:"
cal
}
show_disk_usage() {
echo "Disk usage:"
df -h
}
show_memory_info() {
echo "Memory information:"
free -h
}
while true; do
echo ""
echo "=== SYSTEM INFORMATION MENU ==="
echo "1. Show current date and time"
echo "2. Show calendar"
echo "3. Show disk usage"
echo "4. Show memory information"
echo "5. Exit"
echo ""
read -p "Please select an option (1-5): " choice
case $choice in
1) show_date ;;
2) show_calendar ;;
3) show_disk_usage ;;
4) show_memory_info ;;
5) echo "Goodbye!"; break ;;
*) echo "Invalid option! Please enter a number between 1-5." ;;
esac
read -p "Press Enter to continue..."
clear
done
```

### Output
<img width="845" height="695" alt="image" src="https://github.com/user-attachments/assets/c2a9ff7f-210a-4950-a7f2-6ec09a2b289a" />

---
# Result
Successfully implemented shell scripts for sentence splitting, palindrome checking, CSV processing,
interactive menus, and dictionary-based word verification.
---
# Conclusion
This experiment strengthened understanding of **string handling, user interaction, text processing, and
file manipulation** in Bash scripting.
