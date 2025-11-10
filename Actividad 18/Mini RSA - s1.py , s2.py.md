### Descripción: 
#### Description

Let's decrypt this.Can you decrypt this [ciphertext](https://challenge-files.picoctf.net/c_fickle_tempest/85842c29b0cfe5b651df70af3ae29e233ba1fb1fea0e969d0bd6328220e3d589/ciphertext)? Something seems a bit small.
### Solución:
picoCTF{n33d_a_lArg3r_e_3ed950f0}
### Notas:
Como e = 3 y el mensaje m era pequeño, el cifrado quedó como c = m³ sin reducir módulo n, así que solo calculé la raíz cúbica entera de c y convertí ese número a texto
### Referencias: