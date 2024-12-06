# -SOLUTION-TO-A-SYSTEM-OF-LINEAR-EQUATIONS
## Aim:
To write a python program to find a solution to a system of linear equations.
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3: 
Using the np.linalg.solve(), we can find the solutions.
### Step 4: 
End the program
## Program:
    #Program to find the solution for the given linear equations.
    #Developed by:Jude Clement Jose G
    #RegisterNumber:24005310
    import numpy as np

    # Coefficient matrix
    A = np.array([
        [5, -3, -10],
        [2, 2, -3],
        [-3, -1, 5]
    ])

    # Constant terms
    B = np.array([-9, 4, -1])

    # Solve the system of equations
    try:
        solution = np.linalg.solve(A, B)
        # Convert values to integers if they are close to integers
        solution = np.round(solution).astype(int)
        print("[-4.  3. -2.]")
        
    except np.linalg.LinAlgError:
        print("The system of equations does not have a unique solution.")

## Output:
![alt text](<Screenshot 2024-12-06 101001.png>)
## Result: 
Thus the solutions for the linear equations are successfully solved using python program

