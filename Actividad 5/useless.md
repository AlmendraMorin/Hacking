### Descripción: 
Autor: Loic Shema

Descripción
Hay un script interesante en el directorio personal del usuario.
Se proporcionarán más detalles tras iniciar la instancia del desafío.

Información de depuración: [u:882743 e:p:c:384 i:295263]

Este desafío inicia una instancia bajo demanda.
Su estado actual es: NO_EN_EJECUCIÓN
### Solución:
picoCTF{us3l3ss_ch4ll3ng3_3xpl0it3d_6140}
### Notas:
```shell
Morin-picoctf@webshell:~$ ssh -p 61255 picoplayer@saturn.picoctf.net
The authenticity of host '[saturn.picoctf.net]:61255 ([13.59.203.175]:61255)' can't be established.
ED25519 key fingerprint is SHA256:DiJcS90U9QussLS8HLR6l6BGJb5eCA0vRmA18IvDvw8.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:61255' (ED25519) to the list of known hosts.
picoplayer@saturn.picoctf.net's password: 
Welcome to Ubuntu 20.04.6 LTS (GNU/Linux 6.8.0-1035-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

picoplayer@challenge:~$ ls -la
total 16
drwxr-xr-x 1 picoplayer picoplayer   20 Sep 13 17:02 .
drwxr-xr-x 1 root       root         24 Aug  4  2023 ..
-rw-r--r-- 1 picoplayer picoplayer  220 Feb 25  2020 .bash_logout
-rw-r--r-- 1 picoplayer picoplayer 3771 Feb 25  2020 .bashrc
drwx------ 2 picoplayer picoplayer   34 Sep 13 17:02 .cache
-rw-r--r-- 1 picoplayer picoplayer  807 Feb 25  2020 .profile
-rwxr-xr-x 1 root       root        517 Mar 16  2023 useless
picoplayer@challenge:~$ file useless
useless: Bourne-Again shell script, ASCII text executable
picoplayer@challenge:~$ ls -l useless
-rwxr-xr-x 1 root root 517 Mar 16  2023 useless
picoplayer@challenge:~$ stat useless
  File: useless
  Size: 517             Blocks: 8          IO Block: 4096   regular file
Device: 3eh/62d Inode: 407006697   Links: 1
Access: (0755/-rwxr-xr-x)  Uid: (    0/    root)   Gid: (    0/    root)
Access: 2023-03-16 01:30:52.000000000 +0000
Modify: 2023-03-16 01:30:52.000000000 +0000
Change: 2023-08-04 21:57:24.057492213 +0000
 Birth: -
picoplayer@challenge:~$ getfacl useless 2>/dev/null || true
picoplayer@challenge:~$ cat useless
#!/bin/bash
# Basic mathematical operations via command-line arguments

if [ $# != 3 ]
then
  echo "Read the code first"
else
        if [[ "$1" == "add" ]]
        then 
          sum=$(( $2 + $3 ))
          echo "The Sum is: $sum"  

        elif [[ "$1" == "sub" ]]
        then 
          sub=$(( $2 - $3 ))
          echo "The Substract is: $sub" 

        elif [[ "$1" == "div" ]]
        then 
          div=$(( $2 / $3 ))
          echo "The quotient is: $div" 

        elif [[ "$1" == "mul" ]]
        then
          mul=$(( $2 * $3 ))
          echo "The product is: $mul" 

        else
          echo "Read the manual"
         
        fi
fi
picoplayer@challenge:~$ man useless

useless
     useless, -- This is a simple calculator script

SYNOPSIS
     useless, [add sub mul div] number1 number2

DESCRIPTION
     Use the useless, macro to make simple calulations like addition,subtraction, multi-
     plication and division.

Examples
     ./useless add 1 2
       This will add 1 and 2 and return 3

     ./useless mul 2 3
       This will return 6 as a product of 2 and 3

     ./useless div 6 3
       This will return 2 as a quotient of 6 and 3

     ./useless sub 6 5
       This will return 1 as a remainder of substraction of 5 from 6

Authors
     This script was designed and developed by Cylab Africa

     picoCTF{us3l3ss_ch4ll3ng3_3xpl0it3d_6140}

picoplayer@challenge:~$ Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.

```
### Referencias:
Shell