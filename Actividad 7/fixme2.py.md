### Descripción: 
Corrija el error de sintaxis en el script de Python para imprimir la bandera. [Descargar script de Python] https://artifacts.picoctf.net/c/5/fixme2.py
Sugerencias
¿Son la igualdad y la asignación el mismo símbolo?
Para ver el archivo en la shell web, ejecute: $ nano fixme2.py
Para salir de nano, presione Ctrl y x y siga las instrucciones en pantalla.
No es necesario aplicar ingeniería inversa a la función str_xor para este desafío.

### Solución:
picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
### Notas:
```shell
Morin-picoctf@webshell:~$ rm fixme2.py
Morin-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/5/fixme2.py
--2025-09-26 17:55:50--  https://artifacts.picoctf.net/c/5/fixme2.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.170.131.18, 3.170.131.77, 3.170.131.33, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.170.131.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1029 (1.0K) [application/octet-stream]
Saving to: 'fixme2.py'

fixme2.py              100%[============================>]   1.00K  --.-KB/s    in 0s      

2025-09-26 17:55:50 (37.7 MB/s) - 'fixme2.py' saved [1029/1029]

Morin-picoctf@webshell:~$ head -n 10 fixme2.py

import random



def str_xor(secret, key):
    #extend key to secret length
    new_key = key
    i = 0
    while len(new_key) < len(secret):
Morin-picoctf@webshell:~$ grep "if " fixme2.py -n
22:if flag = "":
Morin-picoctf@webshell:~$ nano +22 fixme2.py
Morin-picoctf@webshell:~$ python3 fixme2.py
  File "/home/Morin-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
Morin-picoctf@webshell:~$ nano +22 fixme2.py
Morin-picoctf@webshell:~$ python3 fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
```
### Referencias: