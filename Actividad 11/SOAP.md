### Descripción: 
The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.

### Solución:
picoCTF{XML_3xtern@l_3nt1t1ty_4dbeb2ed}
### Notas:
```shell
 Interceptioné las peticiones XML de los 3 campos con Burp, las mandé a Repeater y exploté una **XXE** inyectando una entidad externa para leer archivos locales.  
Al enviar el XML modificado obtuve la respuesta con la flag (se reveló al leer el archivo objetivo).
```
### Referencias:
