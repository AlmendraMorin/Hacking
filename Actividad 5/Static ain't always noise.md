### Descripción: 
¿Puedes ver los datos en este binario estático? ¡Este script BASH podría ayudarte!
### Solución:
picoCTF{d15a5m_t34s3r_6f8c8200}
### Notas:
```powerShell
Morin-picoctf@webshell:~$ curl -O https://mercury.picoctf.net/static/0f6ea599582dcce7b4f1ba94e3617baf/static
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  8376  100  8376    0     0  29292      0 --:--:-- --:--:-- --:--:-- 29286
Morin-picoctf@webshell:~$ curl -O https://mercury.picoctf.net/static/0f6ea599582dcce7b4f1ba94e3617baf/ltdis.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   785  100   785    0     0   2811      0 --:--:-- --:--:-- --:--:--  2813
Morin-picoctf@webshell:~$ chmod +x ltdis.sh
Morin-picoctf@webshell:~$ ./ltdis.sh static
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
Morin-picoctf@webshell:~$ cat static.ltdis.strings.txt | grep -i pico
   1020 picoCTF{d15a5m_t34s3r_6f8c8200}
Morin-picoctf@webshell:~$ 
```
### Referencias:
Webshell