### Descripción: 
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.
### Solución:
#### Forma1
``` shell
Morin-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291 | grep picoCTF
picoCTF{digital_plumb3r_ea8bfec7}
^C
Morin-picoctf@webshell:~$ 
```
#### Forma 2
``` Shell
Morin-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291 > bandera     

Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ cat bandera | grep pico
picoCTF{digital_plumb3r_ea8bfec7}
Morin-picoctf@webshell:~$ 

```
### Notas:
grep | palabra - me filtra lo que estoy buscando
cat bandera | grep pico - Me filtra la bandera
### Referencias:
Shell