### Descripción: 
Descargue esta imagen de disco y busque la bandera.Nota: si está usando el shell web, descargue y extraiga la imagen del disco en un `/tmp`directorio que no sea su directorio de inicio.

- [Descargar imagen de disco comprimida](https://artifacts.picoctf.net/c/214/disk.flag.img.gz)
### Solución:

picoCTF{h4un71ng_p457_1d02081e}
### Notas:
```shell
Descargué y descomprimí la imagen `disk.flag.img.gz`, usé SleuthKit (`mmls`, `fls`, `icat`) para extraer `flag.txt.enc` y lo desencripté con `openssl aes256 -k unbreakablepassword1234567`.  
Flag: `picoCTF{h4un71ng_p457_1d02081e}`
```
### Referencias: