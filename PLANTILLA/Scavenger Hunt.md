### Descripción: 
Usar un shell seguro (SSH) será muy importante.
¿Puedes usar SSH como ctf-player para acceder a titan.picoctf.net en el puerto 53951 para obtener la bandera?
También necesitarás la contraseña 84b12bae. Si se te solicita, acepta la huella digital con "sí".
Si tu dispositivo no tiene shell, puedes usar: https://webshell.picoctf.org
Si no estás seguro de qué es un shell, consulta nuestro manual: https://primer.picoctf.com/#_the_shell
### Solución:

### Notas:
```shell
Morin-picoctf@webshell:~$ ssh -p 53951 ctf-player@titan.picoctf.net
The authenticity of host '[titan.picoctf.net]:53951 ([3.139.174.234]:53951)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:53951' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_07a987ac}
Connection to titan.picoctf.net closed.
```
### Referencias:
Shell