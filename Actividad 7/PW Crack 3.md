### Descripción: 
¿Puedes descifrar la contraseña para obtener la bandera?
Descarga el verificador de contraseñas aquí (https://artifacts.picoctf.net/c/16/level3.py). Necesitarás la bandera cifrada (https://artifacts.picoctf.net/c/16/level3.flag.txt.enc) y el hash (https://artifacts.picoctf.net/c/16/level3.hash.bin) en el mismo directorio.
Hay 7 posibles contraseñas, de las cuales una es correcta. Puedes encontrarlas examinando el script del verificador de contraseñas.

Sugerencias

Para ver el archivo level3.hash.bin en la webshell, escribe: $ bvi level3.hash.bin
Para salir de bvi, escribe :q y pulsa Intro.
No es necesario aplicar ingeniería inversa a la función str_xor para este desafío.
### Solución:
picoCTF{m45h_fl1ng1ng_2b072a90}
### Notas:
```shell
wget https://artifacts.picoctf.net/c/16/level3.py
wget https://artifacts.picoctf.net/c/16/level3.flag.txt.enc
wget https://artifacts.picoctf.net/c/16/level3.hash.bin
ls -l level3.py level3.flag.txt.enc level3.hash.bin

chmod +x solve_level3.py
python3 solve_level3.py

nano solve_level3.py  
chmod +x solve_level3.py
python3 solve_level3.py

```
### Referencias:
Shell 