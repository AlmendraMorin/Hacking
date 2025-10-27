### Descripción: 
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/137/disk.flag.img.gz)
### Solución:

picoCTF{by73_5urf3r_adac6cb4}
### Notas:
```shell
Descarguee y descomprimi `disk.flag.img.gz`, use SleuthKit (`mmls`, `fls`) para localizar la partición y los inodos, y extraje el archivo con `icat -o 360448 2371` para leer la flag.  
Flag: `picoCTF{by73_5urf3r_adac6cb4}`
```
### Referencias: