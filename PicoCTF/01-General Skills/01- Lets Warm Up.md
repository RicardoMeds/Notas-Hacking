- #### **Reto** 
Lets Warm Up

#### - **Descripción** 
If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

**Pista**
Envíe su respuesta en nuestro formato de bandera. Por ejemplo, si su respuesta fue "hola", deberá enviar "picoCTF{hola}" como bandera.
#### - **Solución** con python 
Para esta resolución hay varios métodos pero el que hice yo fue el poner un una linea de codigo en la aplicación de ubutun la cual fue: echo -e "\x70"
Y lo que hace es decodifica el 70 en hexadecimal a texto normal, que equivale a la "p"
y la llave seria:
- picoCTF{p}

 #### **Solución** con convertido 
Para esta resolución utilice una pagina de convertidores para resolver este problema
Y lo que hace es decodifica el 70 en hexadecimal a texto normal, que equivale a la "p"
y la llave seria:
- picoCTF{p}

#### - Referencias 
https://gchq.github.io/CyberChef/#recipe=To_Binary('Space',8)From_Binary('Space',8)From_Octal('CRLF')&input=NDI