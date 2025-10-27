### Descripción: 
RED, RED, RED, REDDownload the image: [red.png](https://challenge-files.picoctf.net/c_verbal_sleep/831307718b34193b288dde31e557484876fb84978b5818e2627e453a54aa9ba6/red.png)
### Solución:

picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}
### Notas:
```shell
Analicé `red.png` con **zsteg** y extraje datos ocultos en el canal LSB (b1,rgba,lsb) que contenían una cadena Base64 repetida.  
Al decodificarla obtuve la bandera **picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}**.
```
### Referencias: