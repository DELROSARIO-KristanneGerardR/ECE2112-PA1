# PROGRAMMING-ASSIGNMENT-1
This repository contains the Jupyter Notebook and README file for Experiment 1 - Introduction to Python Programming.  


ALPHABET SOUP PROBLEM: Create a function that takes a string and returns a string with its letters in alphabetical order.  

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
<br>
EMOTICON PROBLEM: Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:  

Step 1: We define a function named 'emotify' that takes one parameter 'sentence'. This function will search for certain keywords in the sentence and replace them with their corresponding emoticons.
```py
def emotify(sentence):
```

Step 2: We convert the sentence to lowercase when searching for keywords so that the function will work regardless of the text case (e.g., "smile" or "SmIlE")
```py
if "smile" in sentence.lower():
```
```py
sentence=sentence.replace("smile", ":)")
```
  If the word "smile" is found, then all occurrences of the word "smile" will be converted to ":)".

Step 3: Check if the word "grin" is contained in the sentence.
```py
if "grin" in sentence.lower():
```
```py
sentence=sentence.replace("grin", ":D")
```
  If the word "grin" is found, then all occurrences of the word "grin" will be converted to ":D".

Step 4: Check if the word "sad" is contained in the sentence.
```py
if "sad" in sentence.lower():
```
```py
sentence=sentence.replace("sad", ":(")
```
  If the word "sad" is found, then all occurrences of the word "sad" will be converted to ":(".

Step 5: Check if the word "mad" is contained in the sentence.
```py
if "mad" in sentence.lower():
```
```py
sentence=sentence.replace("mad", ">:(")
```
  If the word "mad" is found, then all occurrences of the word "mad" will be converted to ">:(".
<br>

UNPACKING LIST PROBLEM: Unpack the list write your code here into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.  

Step 1: We need to take user input as a string and assign it to a variable.
```py
user_input = input("Enter numbers separated by spaces: ")
```

Step 2: We then split the input into several string elements that will be stored in a list using the string method .split().
```py
split_input = user_input.split()
```

Step 3: We initialize an empty list to store converted values.
```py
lst=[]
```

Step 4: We now use a for loop to go through each element of split_input wherein int(num) converts the string to an integer and list.append() adds the integer to the list.
```py
for num in split_input:
    lst.append(int(num))
```

Step 5: We now unpack the list into variables.
```py
first, *middle, last = lst
```
  * "first" takes the first element of the list.
  * "last" takes the last element of the list.
  * "middle" collects all elements in between into a list.






