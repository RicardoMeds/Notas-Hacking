#### - **Descripción** 
¡Conéctese a este servidor PostgreSQL y encuentre la bandera!

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

`psql -h saturn.picoctf.net -p 65424 -U postgres pico`La contraseña es`postgres`
#### Pista 
¿Qué contiene una base de datos SQL?

#### - **Solución** 
pico=# Select * from flags;
 id | firstname | lastname  |                address                 
----+-----------+-----------+----------------------------------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 rows)

pico=# 

picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
