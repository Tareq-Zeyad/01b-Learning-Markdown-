## **Game of Greed 1**
### *How to use the Random Module in Python.*
### **The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.**
<br>

- ### **Randint:** If we wanted a random integer, we can use the randint function Randint accepts two parameters: a min and a max number. Generate integers between 1,5. The first value should be less than the second.
### import random
### print random.randint(0, 5)
### >> This will output either 1, 2, 3, 4 or 5.
<br>

- ### **Random:** If you want a larger number, you can multiply it.
### import random
### random.random() * 100
<br>

- ### **Choice:** Generate a random value from the sequence.
### random.choice( ['red', 'black', 'green'] ).
<br>

- ### **Shuffle:** The shuffle function, shuffles the elements in list in place, so they are in a random order.

### from random import shuffle
### x = [[i] for i in range(10)]
### shuffle(x)
<br>

- ### **Randrange:** Generate a randomly selected element from range(start, stop, step).
### import random
### for i in range(3):
 ###   print random.randrange(0, 101, 5)
<br>

## **What is Risk Analysis**
### **To start off, Risk Analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.**
<br>

## **How to perform Risk Analysis?**
- ### Searching the risk.


- ### Analyzing the impact of each individual risk.


- ### Measures for the risk identified.


