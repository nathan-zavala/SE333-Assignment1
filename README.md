# Part 1
## Question 1:
A  
570 is on point because it is greater than or equal to 570, whereas 571 is off point because it is greater than 570.

## Question 2:
The on point would be 10 and the off points would be 9 and 11 since x must equal 10.

## Question 3:
Input: 0999CM -> Would be invalid because: the leading 0 is dropped, making the number 3 digits long, must be 4 long and must be greater than or equal to 1000.  
Input: 2435DHK -> Would be invalid because there are too many letters, must contain only 2 letters.


# Part 2
See NumberUtilsTest.java


# Part 3
Based on the specifications in NumberUtils.java:  
- Each element in the input lists must be a digit between 0 and 9, otherwise throw an IllegalArgumentException.
- A null input should make the method return null.
- An empty list represents the number 0.
- The method should correctly add two numbers, represented as a list of digits, carrying when needed.

I wrote tests that covered: null inputs, invalid digits, same length lists (without carrying), and different length lists (with carrying). In all my cases, NumberUtils.add() behaved as I expected. I did not find any bugs.



## Collaboration Policy

I have read and followed the collaboration policy for this assignment.
All the wrk submitted is my own and I did not share my solutions with any one.

### Collaboration Consulted
- ChatGPT (for explaining the questions in simpler terms and writing this collaboration policy and somewhat formatting README)
