#### - **Descripción** 
Encontramos esta [captura de paquetes](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap) . Recupera la bandera robada de la red.
#### Pista 
#### - **Solución** 

en la información de cada paquete, hay un número de 4 dígitos que empieza por el 5. Si tomamos los últimos 3 dígitos de cada número, según el orden de llegada de los paquetes, y los convertimos a ASCII, obtenemos nuestra bandera.
![[Pasted image 20250429100253.png]]
picoCTF{p1LLf3r3d_data_v1a_st3g0}
