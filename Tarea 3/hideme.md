### Descripción: 
Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/258/flag.png).
### Solución:

picoCTF{Hiddinng_An_imag3_within_@n_ima9e_d55982e8}
### Notas:
```shell
Usé `binwalk -e` para extraer un archivo ZIP embebido dentro de `flag.png`, navé a `_flag.png.extracted/secret/` y recuperé `flag.png`.  
Transferí el `secret/flag.png` (por `sz`) para abrirlo localmente y obtener la bandera.
```
### Referencias: