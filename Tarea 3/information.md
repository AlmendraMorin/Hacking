### Descripción: 
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/e5825f58ef798fdd1af3f6013592a971/cat.jpg)
### Solución:

picoCTF{the_m3tadata_1s_modified}
### Notas:
```shell
Descargué la imagen `cat.jpg` y analicé sus metadatos con **exiftool**, encontrando un campo codificado en Base64.  
Decodifiqué ese valor y obtuve la bandera **picoCTF{the_m3tadata_1s_modified}**.
```
### Referencias: