### Descripción: 
Descripción
Descomprime este archivo y busca el archivo "uber-secret.txt".
Descarga el archivo zip
### Solución:
picoCTF{f1nd_15_f457_ab443fd1}
### Notas:
``` shell
wget https://artifacts.picoctf.net/c/501/files.zip
unzip files.zip

find . -type f -name "uber-secret.txt" -print

grep -R "picoCTF" .

```
### Referencias:
Shell