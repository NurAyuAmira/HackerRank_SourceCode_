# Let's Echo
## **Task**

Write a bash script that prints the string `"HELLO"`.

### **Input Format**

There is no input file required for this problem.

### **Output Format**
`HELLO` 

----------

## **Approach**

1.  **Bash Scripting Basics**
    
    -   We need to write a simple bash script that prints `"HELLO"`.
    -   The `echo` command in bash is used to display text on the terminal.
2.  **Execution Steps**
    
    -   Create a bash script file (e.g., `hello.sh`).
    -   Write the necessary code to print `"HELLO"`.
    -   Make the script executable using `chmod +x hello.sh`.
    -   Run the script using `./hello.sh`.

----------

## **Code Solution**

    #!/bin/bash
    
    echo "HELLO" 

----------

## **Explanation**

1.  **Shebang (`#!/bin/bash`)**
    
    -   This ensures that the script runs using the bash shell.
2.  **`echo "HELLO"`**
    
    -   The `echo` command prints `"HELLO"` to the terminal.
3.  **Running the Script**
    
    -   Save the script in a file, e.g., `hello.sh`.
    -   Run the following commands in the terminal
        
        `chmod +x hello.sh  # Make the script executable
        ./hello.sh         # Execute the script` 
        
    -   Output:
        
        `HELLO`


# Looping and Skipping
## **Task**

Your task is to use **for loops** to display only **odd natural numbers** from **1 to 99**.

----------

### **Approach**

1.  **Use a loop** to iterate from `1` to `99`.
2.  **Increment by 2** in each iteration to get only **odd numbers**.
3.  **Print each odd number** on a new line.

----------

### **Code Solution (Bash Script)**



    #!/bin/bash
    
    for ((i=1; i<=99; i+=2))
    do
        echo $i
    done

----------

### **Explanation**

1.  **Shebang (`#!/bin/bash`)**
    
    -   This ensures the script runs using the **Bash shell**.
2.  **For Loop (`for ((i=1; i<=99; i+=2))`)**
    
    -   Initializes `i = 1` (starting value).
    -   Runs the loop while `i ≤ 99`.
    -   Increments `i` by `2` in each iteration, ensuring only **odd numbers** are selected.
3.  **Printing Each Odd Number (`echo $i`)**
    
    -   `echo $i` prints the current **odd number** on a new line.


# A Personalized Echo
## **Task**

Write a **Bash script** that accepts **name** as input and displays the greeting:

`Welcome (name)` 

----------

## **Approach**

1.  **Read input** from the user using `read`.
2.  **Store the input** in a variable (`name`).
3.  **Use `echo` to print** the greeting message with the inputted name.

----------

## **Code Solution**



    `#!/bin/bash
    
    # Read input from the user
    read name
    
    # Print the greeting message
    echo "Welcome $name"` 

----------

## **Explanation**

1.  **Shebang (`#!/bin/bash`)**
    
    -   Ensures that the script runs in the **Bash shell**.
2.  **Reading Input (`read name`)**
    
    -   This command waits for user input and stores it in the variable `name`.
3.  **Printing Output (`echo "Welcome $name"`)**
    
    -   Uses **variable expansion (`$name`)** to insert the inputted name into the output.

----------

### **Example Execution**

#### **Input:**

`Alice` 

#### **Output:**

`Welcome Alice` 

----------

### **How to Run the Script**

1.  **Save the script** in a file, e.g., `greet.sh`.
2.  **Make it executable** using:
    
    `chmod +x greet.sh` 
    
3.  **Run the script**:
    
    `./greet.sh` 
    
4.  **Enter a name** when prompted.
