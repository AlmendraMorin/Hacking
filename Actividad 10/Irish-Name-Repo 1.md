### Descripción: 
There is a website running at `https://jupiter.challenges.picoctf.org/problem/39720/` ([link](https://jupiter.challenges.picoctf.org/problem/39720/)) or http://jupiter.challenges.picoctf.org:39720. Do you think you can log us in? Try to see if you can login!
### Solución:
picoCTF{s0m3_SQL_c218b685}
### Notas:
Se obtuvo la bandera explotando un **SQL Injection** en el campo `username` de `login.php` con la carga `' OR '1'='1`, que permitió el login sin credenciales.
### Referencias:

