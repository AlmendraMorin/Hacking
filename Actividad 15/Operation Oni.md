### Descripción: 
Download this disk image, find the key and log into the remote machine.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

Additional details will be available after launching your challenge instance.
### Solución:

picoCTF{k3y_5l3u7h_b5066e83}
### Notas:
```shell
Descargué y descomprimí la imagen `disk.img`, usé SleuthKit (`mmls`, `fls`, `icat`) para localizar y extraer la llave privada SSH (`id_ed25519`), ajusté permisos (`chmod 600`) y me conecté con `ssh -i key_file -p 54164` para leer `/home/ctf-player/flag.txt`.  
Flag: `picoCTF{k3y_5l3u7h_b5066e83}`
```
### Referencias: