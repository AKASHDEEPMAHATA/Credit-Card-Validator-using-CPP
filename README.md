# Credit-Card-Validator-using-CPP

This project is based on  Luhn’s algorithm.


Luhn's algorithm determines whether or not a credit card number is valid. For a given credit card number:

Double the value of every other digit from right to left, beginning with the second to last digit.
Add the digits of the results of Step 1 to the remaining digits in the credit card number.
If the result mod 10 is equal to 0, the number is valid. If the result mod 10 is not equal to 0, the validation fails.
Example

A credit card of type Visa is added with the number 4624 7482 3324 9080.

This credit card number starts with 4, as it should be in all Visa cards. It also has 16 digits, which is valid for a Visa card. Now, execute Luhn's algorithm:

a) Double the value of every other digit from right to left, beginning with the second to last digit.
4624 7482 3324 9080:

8*2 = 16
9*2 = 18
2*2 = 4
3*2 = 6
8*2 = 16
7*2 = 14
2*2 = 4
4*2 = 8

b) Add the digits of the results of the previous step to the remaining digits in the credit card number.
The digits of the result of Step a amount to the following:
1+6+1+8+4+6+1+6+1+4+4+8 = 50

The remaining digits in the credit card number amount to the following:
6+4+4+2+3+4+0+0 = 23

The sum of the two sub results is:
23+50 = 73

c) If the result mod 10 is equal to 0, the number is valid. If the result mod 10 is not equal to 0, the validation fails.
73 mod 10 is 3, therefore the card number is not valid.

A Visa credit card of number 4624 7482 3324 9780, on the other hand, passes the validation.
