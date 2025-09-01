### Descripción: 
What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.

### Solución:
'l3arn_th3_ypp35'

### Notas:
``` python
>>> base64.decode("bDNhcm5fdGgzX3lwcDM1")
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: decode() missing 1 required positional argument: 'output'
>>> base64.b64decode("bDNhcm5fdGgzX3lwcDM1")
b'l3arn_th3_ypp35'
>>> base64.b64decode("bDNhcm5fdGgzX3lwcDM1").decode()
'l3arn_th3_ypp35'
>>> 
```

### Referencias:
Python