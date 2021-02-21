# Crash Course of Python

![Certification](https://user-images.githubusercontent.com/41291493/108625432-4531c600-748e-11eb-9e76-82644ace4591.png{: width="70%" height="70%"}

## Learning Objectives
* Understand what Python is
* Understand why Python is relevant to IT
* Understand the role of automation in IT
* Write scripts that use variables of different data types
* Understand how flow control works in Python
* Implement branches with conditional expressions
* Encapsulate code into functions
* Understand the role and value of loops
* Understand the differences between while and for loops
* Write code that uses while and for loops
* Understand recursion and why it may be useful in scripting
* Understand the difference between strings, lists, and dictionaries
* Manipulate strings in your code
* Create and use lists
* Create and use dictionaries

## Final Project
### Problem Statement
Create a "word cloud" from a text by procssing the text and return a dictionary that outputs the frequency of each words.

### Criteria
#### Input
* Processing the text
* Remove punctuation
* Ignore case and words that do not contain all alphabets
* Count the frequencies
* Ignore uninteresting or irrelevant words

#### Output
A dictionary is the output of the calculate_frequencies function. The wordcloud module will then generate the image from your dictionary.

### Apprach
1. Browse and upload a text to be processed
2. Remove puntuations and normalize the letters
3. Create a set to store the uninteresting words
4. Create a dictionary that uses a word as a key and frequencies of the word as a value
5. Use WordCloud framework to generate a image of world cloud 
