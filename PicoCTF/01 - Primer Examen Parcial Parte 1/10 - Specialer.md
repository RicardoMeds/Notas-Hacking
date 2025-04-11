#### - **Descripción** 
La recepción de Special ha sido genial, como mínimo. Por eso creamos una versión exclusiva de Special, llamada Interfaz Segura e Integral para Afectar Linux Empíricamente Rad, o simplemente "Specialer". Con Specialer, nos esforzamos por eliminar las distracciones que genera el uso de una shell. Sí, eliminamos el corrector ortográfico debido a las quejas de todos. Pero creemos que les entusiasmará nuestro nuevo conjunto de funciones reducidas para que puedan concentrarse en lo que más lo necesitan. Creen una instancia para probar su propia copia de Specialer.

#### Pista 
¿A qué programas tienes acceso?
#### - **Solución** 
Specialer$ echo *
abra ala sim
Specialer$ eco "$(<abra)"
-bash: eco: command not found
Specialer$ eco "$(<ala)"
-bash: eco: command not found
Specialer$ echo "$(<ala)"

Specialer$ echo "$(<abra)"

Specialer$ file
-bash: file: command not found
Specialer$ echo */*
abra/cadabra.txt abra/cadaniel.txt ala/kazam.txt ala/mode.txt sim/city.txt sim/salabim.txt
Specialer$ echo "$(<abra/cadaniel.txt)"
Yes, I did it! I really did it! I'm a true wizard!
Specialer$ echo "$(<ala/kazam.txt)"
return 0 picoCTF{y0u_d0n7_4ppr3c1473_wh47_w3r3_d01ng_h3r3_49193632}
Specialer$
picoCTF{y0u_d0n7_4ppr3c1473_wh47_w3r3_d01ng_h3r3_49193632}
