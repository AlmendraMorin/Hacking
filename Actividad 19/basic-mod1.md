### Descripción: 
We found this weird message being passed around on the servers, we think we have a working decryption scheme.Download the message [here](https://artifacts.picoctf.net/c/129/message.txt).Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore.Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)
### Solución:
picoCTF{R0UND_N_R0UND_ADD17EC2}

### Notas:
Leí los números en message.txt, para cada número calculé n % 37.
Mapeé 0–25 → A–Z, 26–35 → 0–9, 36 → 
Y concatené los caracteres y envolví el resultado
### Referencias:
