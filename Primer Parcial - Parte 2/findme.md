### Descripción: 
Ayúdenos a probar el formulario enviando el nombre de usuario `test`y la contraseña como`test!`

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.
### Solución:
picoCTF{proxies_all_the_way_a0fe074f}
### Notas:
```shell
Entre a link que me proporciona y entre con usuario: test y contraseña:test!, después me fije en la URL que cambio y regrese a la pagina, en el id= me daba cGljb0NURntwcm94aWVzX2Fs y volvi a regresar y lo cambió el id= bF90aGVfd2F5X2EwZmUwNzRmfQ==, me fui a la paguina de base64 y acomode los dos id y me dió la bandera.
```
### Referencias:
https://www.base64decode.org/