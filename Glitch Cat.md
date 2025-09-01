### Descripción: 
Additional details will be available after launching your challenge instance.

Our flag printing service has started glitching!`$ nc saturn.picoctf.net 51537`
### Solución:
``` shell
Morin-picoctf@webshell:~$ nc saturn.picoctf.net 51537
'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'

Morin-picoctf@webshell:~$ python
Python 3.10.12 (main, Feb  4 2025, 14:57:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> nc saturn.picoctf.net 51537
  File "<stdin>", line 1
    nc saturn.picoctf.net 51537
       ^^^^^^
SyntaxError: invalid syntax
>>> 
KeyboardInterrupt
>>> 'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'
'picoCTF{gl17ch_m3_n07_bda68f75}'
>>> 
>>> 
KeyboardInterrupt
>>> 
```
### Notas:

### Referencias:
Shell

