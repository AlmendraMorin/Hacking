### Descripción: 
Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/60f76192f6e1fea6f4e6e8c5fc9a6a27/server.py) [http://mercury.picoctf.net:44693/](http://mercury.picoctf.net:44693/)
### Solución:
picoCTF{pwn_4ll_th3_cook1E5_dbfe90bf}
### Notas:
```shell
Probé una lista de posibles secret_key para las cookies de Flask enviando la cookie firmada a http://mercury.picoctf.net:44693/display y encontré que butter validaba la sesión.  
Flag obtenida: picoCTF{pwn_4ll_th3_cook1E5_dbfe90bf}.
```
### Referencias:
