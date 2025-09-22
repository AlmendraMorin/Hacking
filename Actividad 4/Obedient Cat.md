### Descripción: 
This file has a flag in plain sight (aka "in-the-clear"). [Download flag](https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag).
### Solución:
``` shell
Morin-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag
--2025-09-01 17:17:12--  https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag                   100%[============================>]      34  --.-KB/s    in 0s      

2025-09-01 17:17:12 (28.6 MB/s) - 'flag' saved [34/34]

Morin-picoctf@webshell:~$ ls
README.txt  file  flag
Morin-picoctf@webshell:~$ cat flag
picoCTF{s4n1ty_v3r1f13d_4a2b35fd}
Morin-picoctf@webshell:~$ ^C
Morin-picoctf@webshell:~$ 
```

### Notas:
wget- Descargar archivos de terminal
cat - Mostrar archivos
cat -n - numera las lineas numeradas
### Referencias:
Shell
