### Descripción: 
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file)? This would be really tedious to look through manually, something tells me there is a better way.

### Solución:
1.Descargar
```shell
Morin-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file -O file
--2025-09-01 17:06:16--  https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 14551 (14K) [application/octet-stream]
Saving to: 'file'

file                100%[==================>]  14.21K  --.-KB/s    in 0s      

2025-09-01 17:06:16 (62.8 MB/s) - 'file' saved [14551/14551]

Morin-picoctf@webshell:~$ 
```
2. Leer con grep
```shell
Morin-picoctf@webshell:~$ ^C
Morin-picoctf@webshell:~$ wc file
    6   317 14551 file
Morin-picoctf@webshell:~$ grep 'picoCTF' file
picoCTF{grep_is_good_to_find_things_f77e0797}
Morin-picoctf@webshell:~$ 
```
### Notas:
wc - Cuenta lineas, bytes, caracteres
file - Archivos
### Referencias:
Shell