### Descripción: 
¿Puedes entender este archivo?
Descarga el archivo aquí.
### Solución:
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_dfe803c6}
### Notas:
```powershell
Morin-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/473/enc_flag
--2025-09-13 19:31:44--  https://artifacts.picoctf.net/c/473/enc_flag
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.170.131.33, 3.170.131.18, 3.170.131.72, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.170.131.33|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 349 [application/octet-stream]
Saving to: 'enc_flag.1'

enc_flag.1             100%[============================>]     349  --.-KB/s    in 0s      

2025-09-13 19:31:44 (171 MB/s) - 'enc_flag.1' saved [349/349]

Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ ls -l enc_flag
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 349 Mar 16  2023 enc_flag
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ cat enc_flag
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbHBWV0VKVVZGWm9RMlZzV2tWUmJFNVNDbUpXV25wWmExSmhWMGRHZEdWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ cat stage1
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlpVWEJUVFZoQ2VsWkVRbE5SCmJWWnpZa1JhV0dGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d enc_flag > stage1
Morin-picoctf@webshell:~$ cat stage1
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlpVWEJUVFZoQ2VsWkVRbE5SCmJWWnpZa1JhV0dGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
Morin-picoctf@webshell:~$ base64 -d enc_flag > stage2
Morin-picoctf@webshell:~$ cat stage2
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlpVWEJUVFZoQ2VsWkVRbE5SCmJWWnpZa1JhV0dGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d enc_flag | base64 -d
V1RCa2MyRnRTWGRVYkZaVFltNVNjRmRXYUU5aVJUVnhWVzFhYVdGck5UWmFSVkpQWVRGbmVWVnVR
bHBsYTBweVUxWmpNRTVHWjNsVgpXR1JyVFdwV2VsUlZVbE5oTURCNVZXMWFZUXBTTVhCelZEQlNR
bVZzYkRaWGFteEVXbm93T1VOblBUMEsK
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d enc_flag | base64 -d > stage2
Morin-picoctf@webshell:~$ cat stage2
V1RCa2MyRnRTWGRVYkZaVFltNVNjRmRXYUU5aVJUVnhWVzFhYVdGck5UWmFSVkpQWVRGbmVWVnVR
bHBsYTBweVUxWmpNRTVHWjNsVgpXR1JyVFdwV2VsUlZVbE5oTURCNVZXMWFZUXBTTVhCelZEQlNR
bVZzYkRaWGFteEVXbm93T1VOblBUMEsK
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d stage2 > flag.txt
Morin-picoctf@webshell:~$ cat flag.txt
WTBkc2FtSXdUbFZTYm5ScFdWaE9iRTVxVW1aaWFrNTZaRVJPYTFneVVuQlpla0pyU1ZjME5GZ3lV
WGRrTWpWelRVUlNhMDB5VW1aYQpSMXBzVDBSQmVsbDZXamxEWnowOUNnPT0K
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d flag.txt > final_flag.txt
Morin-picoctf@webshell:~$ cat final_flag.txt
Y0dsamIwTlVSbnRpWVhObE5qUmZiak56ZEROa1gyUnBZekJrSVc0NFgyUXdkMjVzTURSa00yUmZa
R1psT0RBell6WjlDZz09Cg==
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d final_flag.txt > picoCTF_flag.txt
Morin-picoctf@webshell:~$ cat picoCTF_flag.txt
cGljb0NURntiYXNlNjRfbjNzdDNkX2RpYzBkIW44X2Qwd25sMDRkM2RfZGZlODAzYzZ9Cg==
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ base64 -d picoCTF_flag.txt > final_flag_decoded.txt
Morin-picoctf@webshell:~$ cat final_flag_decoded.txt
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_dfe803c6}
Morin-picoctf@webshell:~$ 
Morin-picoctf@webshell:~$ 
```
### Referencias: