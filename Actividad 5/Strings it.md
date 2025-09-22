### Descripción: 
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?
### Solución:
picoCTF{5tRIng5_1T_7f766a23}
### Notas:
``` shell:~$ wget https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
--2025-09-10 06:06:14--  https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 776032 (758K) [application/octet-stream]
Saving to: 'strings.4'

strings.4              100%[============================>] 757.84K  1.86MB/s    in 0.4s    

2025-09-10 06:06:14 (1.86 MB/s) - 'strings.4' saved [776032/776032]

Morin-picoctf@webshell:~$ ls
37          ]        file      flag     strings.1  strings.3
README.txt  bandera  file.hex  strings  strings.2  strings.4
Morin-picoctf@webshell:~$ cat string
cat: string: No such file or directory
Morin-picoctf@webshell:~$ /usr/bin/strings strings.4 | grep "picoCTF{"
picoCTF{5tRIng5_1T_7f766a23}
Morin-picoctf@webshell:~$ ```
### Referencias:
WebShell