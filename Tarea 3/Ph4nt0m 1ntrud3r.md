### Descripción: 
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/a917f567b9cc0f1a730a7801b309955df4d2234a8114326857b9759e9e5d0453/myNetworkTraffic.pcap) and try to get the flag.
### Solución:

picoCTF{1t_w4snt_th4t_34sy_tbh_4r_959f50d3}
### Notas:
```shell
abri el archivo en wireshark y lo acomode por tiempo y tamaño, copie los paquetes uno por uno en cyberchef con base 64 y me dio la flag
```
### Referencias:
[From Base64 - CyberChef](https://gchq.github.io/CyberChef/#recipe=From_Base64\('A-Za-z0-9%2B/%3D',true,false\)&input=Y0dsamIwTlVSZz09CmV6RjBYM2MwY3c9PQpiblJmZEdnMGRBPT0KWHpNMGMzbGZkQT09ClltaGZOSEpmT1E9PQpOVGxtTlRCa013PT0KZlE9PQ)