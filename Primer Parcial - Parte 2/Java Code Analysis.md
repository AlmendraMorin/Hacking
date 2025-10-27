### Descripción: 
BookShelf Pico, my premium online book-reading service.I believe that my website is super secure. I challenge you to prove me wrong by reading the 'Flag' book!

Additional details will be available after launching your challenge instance.
### Solución:
picoCTF{w34k_jwt_n0t_g00d_d7c2e335}
### Notas:
```shell
Abri el URL y entre con el usuario user y contraseña user, abri el zip y estuve navegando entre los archivos de códigos, después abri un jwt token decoder y pegue el token y le cambie el roo "Free" por "Admin", userId "1" por "2" y email por "admin" y puse el 1234 que mostraba en un documento, copie el nuevo token y en la inspeccion de la página copie el nuevo token y cambie los campos del payload y me salió la bandera. 
```
### Referencias:
https://supertokens.com/jwt-encoder-decoder