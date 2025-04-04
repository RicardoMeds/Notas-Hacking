#### - **Descripción** 
¿Sabes cómo utilizar el inspector web?

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

**Pista**
Utilice el inspector web en otros archivos incluidos en la página web.

La bandera puede estar codificada o no.
#### - **Solución** 
Inspeccionabas la paginas y te ibas a ABOUT en la pagina y se veia el codigo fuente y nos mostraba algo fuera de lo comun :
section class="about" notify_true="cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfMDdiOTFjNzl9">
Se tenia que codificar estos datos:
cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfMDdiOTFjNzl9
y nos daba la bandera 
picoCTF{web_succ3ssfully_d3c0ded_07b91c79}

CyberChef
https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=Y0dsamIwTlVSbnQzWldKZmMzVmpZek56YzJaMWJHeDVYMlF6WXpCa1pXUmZNRGRpT1RGak56bDk