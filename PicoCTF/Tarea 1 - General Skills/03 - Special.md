#### - **Descripción** 
¿Los usuarios avanzados no se cansan de cometer errores ortográficos en el shell? ¡Ya no! Presentamos Special, la interfaz de corrección ortográfica para Linux. Ahora, cada palabra está escrita y capitalizada correctamente... ¡automáticamente y en segundo plano! Sea el primero en probar Special en versión beta y no dude en contarnos todo sobre cómo Special agiliza cada proceso de desarrollo al que se enfrenta. Cuando sus compañeros de trabajo vean su increíble interfaz de shell, dígales: Eso es Special (TM)Inicie su instancia para ver los detalles de la conexión.

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

**Pista**
Experimente con diferentes sintaxis de shell

#### - **Solución** 
Special$ ls
Is 
sh: 1: Is: not found
Special$ ls
Is 
sh: 1: Is: not found
Special$ whoami
Whom 
sh: 1: Whom: not found
Special$ pwd
Pod 
sh: 1: Pod: not found
Special$ ${parameter=ls}
${parameter=ls} 
blargh
Special$ ${parameter=cd blargh}
${parameter=cd blargh} 
Special$ ${parameter=ls blargh}
${parameter=ls blargh} 
flag.txt
Special$ ${parameter=cat < blargh/flag.txt}
${parameter=cat < blargh/flag.txt} 
cat: '<': No such file or directory
picoCTF{5p311ch3ck_15_7h3_w0r57_3befb794}Special$ 

picoCTF{5p311ch3ck_15_7h3_w0r57_3befb794}