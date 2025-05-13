#### - **Descripción** 
¡Un fantasma digital ha traspasado mis defensas y me han robado mis datos confidenciales! 😱💻 Tu misión es descubrir cómo este intruso fantasma se infiltró en mi sistema y recuperar la bandera oculta.Para resolver este desafío, deberá analizar el archivo PCAP proporcionado y rastrear el método de ataque. El atacante ha ocultado sus movimientos con astucia y a tiempo. ¡Explore el tráfico de red, aplique los filtros adecuados, demuestre su pericia forense y desenmascare al intruso digital!Encuentre el archivo PCAP aquí [Archivo PCAP de tráfico de red](https://challenge-files.picoctf.net/c_verbal_sleep/bdda31c79c31975a5fe5402777bc87794655172e5d5bb2b569f1970df8efda34/myNetworkTraffic.pcap) e intente obtener la bandera.
#### Pista 
Filtra tus paquetes para limitar tu búsqueda.
Los ataques se realizaron en el momento oportuno.
El tiempo es esencial
#### - **Solución** 
Utilice el wireshark, el cual posicione a todo por medio del tiempo y todos los que empezaban con len=12 mostre los paquetes en byte y me daba la bandera por parte solo era juntarlos y listo 

picoCTF{1t_w4snt_th4t_34sy_tbh_4r_af160980}