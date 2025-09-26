### Descripción: 
¡Encuentra la bandera en el script de Python!
Descarga el script de Python (https://artifacts.picoctf.net/c/37/serpentine.py)

Sugerencias
Intenta ejecutar el script y observa qué sucede.
En la shell web, intenta examinar el script con un editor de texto como nano.
Para salir de nano, presiona Ctrl y x y sigue las instrucciones en pantalla.
No es necesario aplicar ingeniería inversa a la función str_xor para este desafío.
### Solución:
picoCTF{7h3_r04d_l355_7r4v3l3d_8e47d128}
### Notas:
```shell
wget https://artifacts.picoctf.net/c/37/serpentine.py
ls -l serpentine.py

head -n 200 serpentine.py
tail -n 200 serpentine.py

python3 -c "from serpentine import print_flag; print_flag()"

```
### Referencias:
