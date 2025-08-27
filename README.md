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








