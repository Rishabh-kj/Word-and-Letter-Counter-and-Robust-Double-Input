# Word-and-Letter-Counter-and-Robust-Double-Input

**Part 1 (Word and Letter Counter): -**

Objective Provided: Write a program that will read in a line of text and output the number of words 
in the line and the number of occurrences of each letter. Define a word to be any string of letters that 
is delimited at each end by either whitespace, a period, a comma, or the beginning or end of the line. 
You can assume that the input consists entirely of letters, whitespace, commas, and periods. When 
outputting the number of letters that occur in a line, be sure to count uppercase and lowercase 
versions of a letter as the same letter. Output the letters in alphabetical order and list only those 
letters that occur in the input line. For example, the input line I say Hi. should produce output similar 
to the following: 3 words 1 a 1 h 2 i 1 s 1 y 

Coding Language Used: C

Approach: Input is taken from the user and stored in a string named line → only the alphabets from 
the string named line is stored in another string named linelowered, while ensuring that the 
uppercase alphabets are converted to lowercase using tolower() → bubble sort is used to sort the 
string named linelowered in ascending order → the distinct elements of the string named 
linelowered are added to a string named linedistinct → counting of the number of occurrences of the 
different elements of (the string named) linedistinct in (the string named) linelowered is done, and 
the number of occurrences is added to an array named counted, with the number of occurrences of 
a particular alphabet having the same expected index as the alphabet in the string named linedistinct 
→ the final output line can then be printed.

**Part 2 (Robust Double Input): -**

Objective Provided: Give the function definition for the function with the following function 
declaration. Embed your definition in a suitable test program.  
void get_double(double* input_number); //Postcondition: input_number is given a value that the user approves of. 
You can assume that the user types in the input in normal everyday notation, such as 23.789. Model 
your definition of the definition of the function so that your function reads the input as characters, 
edits the string of characters, and converts the resulting string to a number of type double. You will 
need to define a function called read_and_clean with the following description: 
void read_and_clean(double * n);  
// reads a line of input,  
// i) discards all symbols except digits for 'whole part', 
// reading '.' goes to next part, '\n' terminates  
// ii)discards all symbols except digits for fractional  
//part, reading 'e' 'E', goes to next part, '\n' terminates  
//iii)discards all symbols except sign, then digits for 
//exponent part 
// reading '\n' terminates. 
Allow the user to enter the number in either the normal everyday notation, as discussed above, or in 
e-notation. Your function should decide whether or not the input is in e-notation by reading the 
input, not by asking the user whether she or he will use e-notation. 

Coding Language Used: C 

Approach: In the function read_and_clean (invoked via the function get_double) an input is taken 
from the user and stored in a string named strinput → the index for the decimal point, e or E symbol 
as well as the index for the sign symbol (+ or -) is taken from the string strinput → a string named 
strselective is used to store the desirable characters from the string named strinput → the string is 
converted to double and is stored in a variable of type double, which is initialised in the main 
function → the final double value is printed from the main function. 
