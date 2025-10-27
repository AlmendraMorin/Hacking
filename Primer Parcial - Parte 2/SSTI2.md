### Descripción: 
I made a cool website where you can announce whatever you want! I read about input sanitization, so now I remove any kind of characters that could be a problem :)

Additional details will be available after launching your challenge instance.
### Solución:
# picoCTF{sst1_f1lt3r_byp4ss_63b833cd}
### Notas:
```shell
Se explotó una vulnerabilidad SSTI en un entorno Flask/Jinja2 con múltiples filtros activos. Se usaron accesos indirectos (__globals__, __builtins__, attr(), y escapes hexadecimales) para ejecutar os.popen('cat flag') y revelar la bandera.
```
### Referencias:
https://onsecurity.io/article/server-side-template-injection-with-jinja2/