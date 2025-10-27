### Descripción: 
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/74274b96fe966126a1953c80762af80d/whitepages.txt) is all blank!
### Solución:

picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}
### Notas:
```shell
Leí whitepages.txt y convertí espacios especiales (`\xe2\x80\x83`) a `0` y espacios normales a `1`, filtré sólo esos bits y los agrupé en bytes.  
Convertí esos bytes a ASCII para obtener el mensaje/flag
```
### Referencias: