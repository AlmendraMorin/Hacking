### Descripción: 
There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 43239`, but it doesn't speak English...
### Solución:
```shell
Morin-picoctf@webshell:~$ nc mercury.picoctf.net 43239
112 
105 
99 
111 
67 
84 
70 
123 
103 
48 
48 
100 
95 
107 
49 
116 
116 
121 
33 
95 
110 
49 
99 
51 
95 
107 
49 
116 
116 
121 
33 
95 
55 
99 
48 
56 
50 
49 
102 
53 
125 
10 
^C
Morin-picoctf@webshell:~$ printf "\x70\x69\x63\x6f\x43\x54\x46\x7b\x67\x30\x30\x64\x5f\x6b\x31\x74\x74\x79\x21\x5f\x6e\x31\x63\x33\x5f\x6b\x31\x74\x74\x79\x21\x5f\x37\x63\x30\x38\x32\x31\x66\x35\x7d\n"
picoCTF{g00d_k1tty!_n1c3_k1tty!_7c0821f5}
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ ^C
Morin-picoctf@webshell:~$ 
```

### Notas:
printf - Imprimir letras
### Referencias:
Shell