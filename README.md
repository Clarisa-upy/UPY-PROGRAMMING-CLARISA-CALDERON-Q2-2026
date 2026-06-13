# UPY-PROGRAMMING-CLARISA-CALDERON-Q2-2026
Hola mundo

# Git/GitHub Repository
This repository includes Python programs created during Unit 2 of the Programming course.
The goal of this project is to learn how to work like a professional developer by using Git for version control and GitHub to store and share the code.

# Project Overview: Numerical Integration Calculator
The main purpose of this application is to estimate the area under a mathematical function f(x) between two points, [a, b].
Because computers cannot solve integrals using regular math rules like humans do on paper, this script uses geometric shapes to find the answer. It splits the total area into 1,000 small pieces (n = 1000) and adds them all together to get the final result.

# 1.User Input and Setup
First, the program asks the user to enter the integration boundaries (a and b), the function they want to use, and their preferred calculation method.

Key Feature: The code includes a smart check for the mathematical constant pi. If a user inputs the word "pi", the program automatically changes it to the real numerical value from the math library using .replace().
After that, it calculates h, which is the width of each small section, using the formula: h = (b - a) / n.

# 2.Improving the Rectangle Methods (LRM, RRM, MRM)
To keep the code clean, the program does not use three separate for loops for the rectangle methods. Instead, it combines the logic into a single loop by using two variables: shift and constant.
LRM (Left Riemann Sum): The loop runs normally (shift = 0), which means it measures the height of the rectangle using the left side of the segment.
RRM (Right Riemann Sum): The loop moves forward by one step (shift = 1) to calculate the height from the right side of the segment.
MRM (Midpoint Riemann Sum): The program adds a specific value (h/2) to the position variable. This shifts the calculation point exactly to the middle of the segment before finding the height.

# 3.The Trapezoid Method
This technique has its own separate code because the mathematical formula is different. It does not use flat rectangles; instead, it works with trapezoids by averaging the sides:
First, the script calculates the start and end points of the curve by themselves.
Next, it uses a for loop to multiply all the middle heights by two and add them together, following the correct mathematical rule for trapezoids.Technologies UsedLanguage: Python 3.xVersion Control: GitPlatform: GitHubHow to Run the ProjectMake sure you have Python installed on your computer.