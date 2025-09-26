### Descripción: 
Ejecute el script de Python code.py en el mismo directorio que codebook.txt.
Descargar code.py https://artifacts.picoctf.net/c/3/code.py
Descargar codebook.txt https://artifacts.picoctf.net/c/3/codebook.txt
### Solución:
picoCTF{c0d3b00k_455157_197a982c}
### Notas:
```shell
Morin-picoctf@webshell:~$ wget -O code.py  "https://artifacts.picoctf.net/c/3/code.py"
--2025-09-22 20:41:55--  https://artifacts.picoctf.net/c/3/code.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.170.131.18, 3.170.131.72, 3.170.131.33, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.170.131.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1278 (1.2K) [application/octet-stream]
Saving to: 'code.py'

code.py                100%[============================>]   1.25K  --.-KB/s    in 0s      

2025-09-22 20:41:55 (105 MB/s) - 'code.py' saved [1278/1278]

Morin-picoctf@webshell:~$ wget -O codebook.txt "https://artifacts.picoctf.net/c/3/codebook.txt"
--2025-09-22 20:42:06--  https://artifacts.picoctf.net/c/3/codebook.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.170.131.33, 3.170.131.77, 3.170.131.72, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.170.131.33|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 27 [application/octet-stream]
Saving to: 'codebook.txt'

codebook.txt           100%[============================>]      27  --.-KB/s    in 0s      

2025-09-22 20:42:06 (8.36 MB/s) - 'codebook.txt' saved [27/27]

Morin-picoctf@webshell:~$ ls -l code.py codebook.txt
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 1278 Mar 16  2023 code.py
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   27 Mar 16  2023 codebook.txt
Morin-picoctf@webshell:~$ file code.py
code.py: Python script, ASCII text executable, with very long lines (404)
Morin-picoctf@webshell:~$ sed -n '1,200p' code.py

import random
import sys



def str_xor(secret, key):
    #extend key to secret length
    new_key = key
    i = 0
    while len(new_key) < len(secret):
        new_key = new_key + key[i]
        i = (i + 1) % len(key)        
    return "".join([chr(ord(secret_c) ^ ord(new_key_c)) for (secret_c,new_key_c) in zip(secret,new_key)])


flag_enc = chr(0x13) + chr(0x01) + chr(0x17) + chr(0x07) + chr(0x2c) + chr(0x3a) + chr(0x2f) + chr(0x1a) + chr(0x0d) + chr(0x53) + chr(0x0c) + chr(0x47) + chr(0x0a) + chr(0x5f) + chr(0x5e) + chr(0x02) + chr(0x3e) + chr(0x5a) + chr(0x56) + chr(0x5d) + chr(0x45) + chr(0x5d) + chr(0x58) + chr(0x31) + chr(0x58) + chr(0x58) + chr(0x59) + chr(0x02) + chr(0x51) + chr(0x4c) + chr(0x5a) + chr(0x0c) + chr(0x13)



def print_flag():
  try:
    codebook = open('codebook.txt', 'r').read()
    
    password = codebook[4] + codebook[14] + codebook[13] + codebook[14] +\
               codebook[23]+ codebook[25] + codebook[16] + codebook[0]  +\
               codebook[25]
               
    flag = str_xor(flag_enc, password)
    print(flag)
  except FileNotFoundError:
    print('Couldn\'t find codebook.txt. Did you download that file into the same directory as this script?')



def main():
  print_flag()



if __name__ == "__main__":
  main()

Morin-picoctf@webshell:~$ less code.py

[1]+  Stopped                 less code.py
Morin-picoctf@webshell:~$ python3 code.py < codebook.txt > out.txt 2>&1
Morin-picoctf@webshell:~$ grep -oE "picoCTF\{[^}]+\}" out.txt || true
picoCTF{c0d3b00k_455157_197a982c}
Morin-picoctf@webshell:~$ 
```
### Referencias:
Shell