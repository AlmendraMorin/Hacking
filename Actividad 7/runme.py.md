### Descripción: 
Ejecuta el script runme.py para obtener la bandera. Descarga el script con tu navegador o con wget en la shell web.
Descarga el script runme.py de Python. 
https://artifacts.picoctf.net/c/34/runme.py
Consejos
1. Si tienes Python en tu ordenador, puedes descargar el script y ejecutarlo normalmente. De lo contrario, usa el comando wget en la shell web.
2. Para usar wget en el webshell, primero haga clic derecho en el enlace de descarga y seleccione 'Copiar enlace' o 'Copiar dirección de enlace'
3. Escribe todo después del signo de dólar en el webshell: $ wget, luego pega el enlace después del espacio después de wget y presiona Enter. Esto descargará el script en el webshell para que puedas ejecutarlo.
4. Finalmente, para ejecutar el script, escribe todo lo que esté después del signo de dólar y luego presiona Enter: $ python3 runme.py ¡Deberías tener la bandera ahora!
### Solución:
picoCTF{run_s4n1ty_run}

### Notas:
```shell
wget -O runme.py "https://artifacts.picoctf.net/c/34/runme.py"

head -n 40 runme.py
less runme.py    # q para salir

python3 runme.py 2>&1 | tee out.txt
grep -oE "picoCTF\{[^}]+\}" out.txt || true

```
### Referencias:
Shell