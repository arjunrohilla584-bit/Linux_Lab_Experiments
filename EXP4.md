## Experiment [4]: [Bash Scripting]
### Name arjun, Roll No.: 590029204, Date: 2025-09-04
### AIM: 
* [To Learn Basics of Bash Scripting.]

### Requirements:
* [Any Linux Distro, any kind of text editor (vs code, vim, notepad, nano, etc)]

### Theory: 
* [Learning the basics of bash scripting.]

## Procedure & Observations

## Exercise 1: [Hello World Script]

## Task Statement: 
* [Basic Usage of Shell Scripts]

## Explanation: 
* [Writing Begginer level Shell Scripts]

## Command(s):
```
#!/bin/bash
echo "Hello, World!"

```

#### Output:
<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/a10789a4-c5f7-44ad-83f0-5ffed42b29a8" />


## Exercise 2: [Personalized Greeting Script]

## Task Statement: 
* [Basic Shell Script to callout user defined function.]

## Explanation: 
* [This Shell script will take input from user and store it in a variable and then call the variable which will output the stored value.]

## Command(s):
```
#!/bin/bash
echo "What is your name?"
read name
echo "Hello, $name! Welcome to Shell Scripting."

``` 

## Output:
<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/d8f1bcca-5c17-489e-bf0d-4d37da363117" />


## Exercise 3: [Arithmetic Operations in Shell Scripting]

## Task Statement:
* [Using Basic Arithmetic Operations in Shell Scripts]

## Command(s):
```

#!/bin/bash
echo "Enter first number: "
read num1
echo "Enter second number: "
read num2

echo "Addition: $((num1 + num2))"
echo "Subtraction: $((num1 - num2))"
echo "Multiplication: $((num1 * num2))"
echo "Division: $((num1 / num2))"

```

## Output:
<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/80dfcb84-6610-408a-9301-0990a5817fb5" />


## Exercise 4:
* [Voting Eligibility]

## Task Statement:
* [Using Conditionals in Shell script ]

## Command(s):
```
#!/bin/bash
echo "What is your age?"
read age
if [ $age -ge 18 ]; then
    
    echo "You are eligible to vote!"
    
else 
    echo "You are not eligible to vote!"

fi

```

## Output:
<img width="1483" height="601" alt="image" src="https://github.com/user-attachments/assets/2ead419a-abb8-4a60-9b12-26bed62e7278" />


## Result

* The Exercises were successfully completed for Basic Shell Scripting
