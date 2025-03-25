#### - **Descripción** 

Este sitio web solo se puede visualizar con **picobrowser** . ¡Vaya y capture la bandera! `https://jupiter.challenges.picoctf.org/problem/26704/`( [enlace](https://jupiter.challenges.picoctf.org/problem/26704/) ) o http://jupiter.challenges.picoctf.org:26704

**Pista**
No necesitas descargar un nuevo navegador web
#### - **Solución** 
Aquí vemos un sitio que comprueba si el navegador es específico antes de permitirte acceder. Dado que picobrowser no es el nombre de un navegador web, te impedirá acceder. Aquí, debemos revisar las condiciones de red del sitio. En Chrome, después de acceder a las herramientas para desarrolladores, ve a los tres puntos en la esquina superior derecha y selecciona Más herramientas > Condiciones de red. Allí, deberías ver una opción para cambiar el agente de usuario a uno personalizado. Si lo cambias a **picobrowser** , el sitio te permitirá acceder a la bandera.
![[Pasted image 20250324123451.png]]
picoCTF{p1c0_s3cr3t_ag3nt_e9b160d0}