### Descripción: 
In the last challenge, you mastered octal (base 8), decimal (base 10), and hexadecimal (base 16) numbers, but this vault door uses a different change of base as well as URL encoding!The source code for this vault is here: [VaultDoor5.java](https://challenge-files.picoctf.net/c_fickle_tempest/bd4f8f70a70dacc0e57dfc24ff34f5297a3db3c9c4366fd8df02f6bf47c794c8/VaultDoor5.java)
### Solución:
picoCTF{c0nv3rt1ng_fr0m_ba5e_64_be9f10a4}

### Notas:
Decodifique el expected desde Base64, luego a URL-encoding (%xx), y finalmente obtuve la cadena original.
### Referencias:
