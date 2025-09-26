### Descripción: 
¿Puedes descifrar la contraseña para obtener la bandera?
Descarga el verificador de contraseñas aquí (https://artifacts.picoctf.net/c/13/level2.py). Necesitarás la bandera cifrada (https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) en el mismo directorio.

Pistas

¿Te suena esta codificación?
No es necesario aplicar ingeniería inversa a la función str_xor para este desafío.
### Solución:
picoCTF{tr45h_51ng1ng_489dea9a}
### Notas:
```shell
wget https://artifacts.picoctf.net/c/13/level2.py
wget https://artifacts.picoctf.net/c/13/level2.flag.txt.enc
ls -l level2.py level2.flag.txt.enc

head -n 200 level2.py

python3 level2.py
CONTRASEÑA: de76

```
### Referencias:
Shell