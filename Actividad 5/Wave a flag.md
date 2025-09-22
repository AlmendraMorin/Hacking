### Descripción: 
Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/b28b6021d6040b086c2226ebeb913bc2/warm) has extraordinarily helpful information...
### Solución:
picoCTF{b1scu1ts_4nd_gr4vy_d6969390}
### Notas:
```shell
Morin-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/b28b6021d6040b086c2226ebeb913bc2/warm
--2025-09-10 06:13:23--  https://mercury.picoctf.net/static/b28b6021d6040b086c2226ebeb913bc2/warm
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 10936 (11K) [application/octet-stream]
Saving to: 'warm'

warm                   100%[============================>]  10.68K  --.-KB/s    in 0s      

2025-09-10 06:13:23 (231 MB/s) - 'warm' saved [10936/10936]

Morin-picoctf@webshell:~$ chmod +x warm
Morin-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_d6969390}
Morin-picoctf@webshell:~$ ./warm --help
I don't know what '--help' means! I do know what -h means though!
Morin-picoctf@webshell:~$ 
```
### Referencias:
Webshell