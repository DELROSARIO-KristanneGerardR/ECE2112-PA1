# PROGRAMMING-ASSIGNMENT-1
This repository contains the Jupyter Notebook and README file for Experiment 1 - Introduction to Python Programming.

1. ALPHABET SOUP PROBLEM: Create a function that takes a string and returns a string with its letters in alphabetical order.  

Step 1: We need to define a function wherein we will process the string input.
```py
def alphabet_soup(text):
```

Step 2: Inside the function, we need to sort the characters of the string. We will use the built-in function sorted() to arrange them into a list in alphabetical order. Then, using the join() function will merge that list into a single string.
```py
return ''.join(sorted(text))
```

Step 3: We now need to ask the user for a string by using the input() function and assign it to a variable.
```py
user_input=input("Enter a string: ")
```

Step 4: Finally, we print the sorted version of the string by calling the alphabet_soup() function with 'user_input'.
```py
print("Sorted string: ", alphabet_soup(user_input))
```
