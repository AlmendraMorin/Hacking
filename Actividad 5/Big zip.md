### Descripción: 
Descripción
Descomprima este archivo y busque la bandera.
Descargar archivo zip
### Solución:
picoCTF{gr3p_15_m4g1c_ef8790dc}
### Notas:
wget https://artifacts.picoctf.net/c/503/big-zip-files.zip
unzip big-zip-files.zip -d big-zip-files
grep -r "picoCTF{" big-zip-files

### Referencias:
Shell