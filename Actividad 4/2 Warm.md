Descripción: ¿Puedes convertir el número 42 (base 10) a binario (base 2)?

Solución: picoCTF{101010}

Notas: 
## FORMA1
- 42÷2=2142 ÷ 2 = 2142÷2=21, residuo **0**
    
- 21÷2=1021 ÷ 2 = 1021÷2=10, residuo **1**
    
- 10÷2=510 ÷ 2 = 510÷2=5, residuo **0**
    
- 5÷2=25 ÷ 2 = 25÷2=2, residuo **1**
    
- 2÷2=12 ÷ 2 = 12÷2=1, residuo **0**
    
- 1÷2=01 ÷ 2 = 01÷2=0, residuo **1**

## FORMA 2
``` Python
Morin-picoctf@webshell:~$ python
Python 3.10.12 (main, Feb  4 2025, 14:57:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(bin(numero)[42:])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'numero' is not defined
>>> print(bin(10)[42:])

>>> 410
410
>>> 
>>> print(bin(42)(2:])
  File "<stdin>", line 1
    print(bin(42)(2:])
                   ^
SyntaxError: invalid syntax
>>> print(bin(42)[2:])
101010
```

Referencias: 
	Omni Calculator
	Python
	