### Descripción: 
¿Qué tan bien puedes realizar operaciones binarias básicas?

### Solución:
picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6ab1ad84}
### Notas:
Morin-picoctf@webshell:~/drop-in/drop-in/drop-in/drop-in/drop-in$ nc titan.picoctf.net 58474
 
Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10111111
Binary Number 2: 01010101


Question 1/6:
Operation 1: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 00101010
Correct!

Question 2/6:
Operation 2: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111111
Correct!

Question 3/6:
Operation 3: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 100010100
Correct!

Question 4/6:
Operation 4: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 111111010001011
Incorrect. Try again
Enter the binary result: 01101011
Incorrect. Try again
Enter the binary result: 11111100101011
Incorrect. Try again
Enter the binary result: 01101011
Incorrect. Try again
Enter the binary result: ^Z
[7]+  Stopped                 nc titan.picoctf.net 58474
Morin-picoctf@webshell:~/drop-in/drop-in/drop-in/drop-in/drop-in$ nc titan.picoctf.net 58474
 
Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10011101
Binary Number 2: 00000111


Question 1/6:
Operation 1: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 

Incorrect input. Provide the right input
Enter the binary result: 10011111
Correct!

Question 2/6:
Operation 2: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00000101
Correct!

Question 3/6:
Operation 3: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10001001011
Correct!

Question 4/6:
Operation 4: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 100111010
Correct!

Question 5/6:
Operation 5: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10100100
Correct!

Question 6/6:
Operation 6: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 00000011
Correct!

Enter the results of the last operation in hexadecimal: 3

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6ab1ad84}
### Referencias: