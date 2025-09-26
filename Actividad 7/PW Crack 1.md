### Descripción: 
¿Puedes descifrar la contraseña para obtener la bandera?
Descarga el verificador de contraseñas aquí (https://artifacts.picoctf.net/c/11/level1.py). También necesitarás la bandera cifrada (https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) en el mismo directorio.
Consejos
Para ver el archivo en la webshell, escribe: $ nano level1.py
Para salir de nano, presiona Ctrl y x y sigue las instrucciones en pantalla.
No es necesario aplicar ingeniería inversa a la función str_xor para este desafío.
### Solución:
picoCTF{545h_r1ng1ng_fa343060}
### Notas:
```shell
wget https://artifacts.picoctf.net/c/11/level1.py
wget https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
ls -l level1.py level1.flag.txt.enc

nano level1.py

python3 level1.py

CONTRASEÑA: 1e1a

```
### Referencias: