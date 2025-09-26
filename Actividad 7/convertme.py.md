### Descripción: 
Ejecute el script de Python y convierta el número dado de decimal a binario para obtener la bandera. [Descargar script de Python] https://artifacts.picoctf.net/c/23/convertme.py
Consejos
1. ¡Busca una aplicación de conversión de números decimales a binarios en la web o usa la calculadora de tu computadora!
2. No es necesario realizar ingeniería inversa a la función str_xor para este desafío.
3. Si tiene Python en su computadora, puede descargar el script y ejecutarlo normalmente. De lo contrario, use el comando wget en la shell web.
4. Para usar wget en el webshell, primero haga clic derecho en el enlace de descarga y seleccione 'Copiar enlace' o 'Copiar dirección de enlace'
5. Escribe todo después del signo de dólar en el webshell: $ wget, luego pega el enlace después del espacio después de wget y presiona Enter. Esto descargará el script en el webshell para que puedas ejecutarlo.
6. Finalmente, para ejecutar el script, escriba todo después del signo de dólar y luego presione Enter: $ python3 convertme.py

### Solución:
picoCTF{4ll_y0ur_b4535_9c3b7d4d}
### Notas:
```shell
Morin-picoctf@webshell:~$ wget -O convertme.py "https://artifacts.picoctf.net/c/23/convertme.py"
--2025-09-22 20:51:40--  https://artifacts.picoctf.net/c/23/convertme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.170.131.33, 3.170.131.72, 3.170.131.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.170.131.33|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1189 (1.2K) [application/octet-stream]
Saving to: 'convertme.py'

convertme.py           100%[============================>]   1.16K  --.-KB/s    in 0s      

2025-09-22 20:51:40 (425 MB/s) - 'convertme.py' saved [1189/1189]

Morin-picoctf@webshell:~$ sed -n '1,200p' convertme.py

import random



def str_xor(secret, key):
    #extend key to secret length
    new_key = key
    i = 0
    while len(new_key) < len(secret):
        new_key = new_key + key[i]
        i = (i + 1) % len(key)        
    return "".join([chr(ord(secret_c) ^ ord(new_key_c)) for (secret_c,new_key_c) in zip(secret,new_key)])


flag_enc = chr(0x15) + chr(0x07) + chr(0x08) + chr(0x06) + chr(0x27) + chr(0x21) + chr(0x23) + chr(0x15) + chr(0x5f) + chr(0x05) + chr(0x08) + chr(0x2a) + chr(0x1c) + chr(0x5e) + chr(0x1e) + chr(0x1b) + chr(0x3b) + chr(0x17) + chr(0x51) + chr(0x5b) + chr(0x58) + chr(0x5c) + chr(0x3b) + chr(0x4c) + chr(0x06) + chr(0x5d) + chr(0x09) + chr(0x5e) + chr(0x00) + chr(0x41) + chr(0x01) + chr(0x13)


num = random.choice(range(10,101))

print('If ' + str(num) + ' is in decimal base, what is it in binary base?')

ans = input('Answer: ')

try:
  ans_num = int(ans, base=2)
  
  if ans_num == num:
    flag = str_xor(flag_enc, 'enkidu')
    print('That is correct! Here\'s your flag: ' + flag)
  else:
    print(str(ans_num) + ' and ' + str(num) + ' are not equal.')
  
except ValueError:
  print('That isn\'t a binary number. Binary numbers contain only 1\'s and 0\'s')
Morin-picoctf@webshell:~$ python3 convertme.py
If 84 is in decimal base, what is it in binary base?
Answer: 1010100
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_9c3b7d4d}
Morin-picoctf@webshell:~$ 
```
### Referencias:
Shell