- #### **Reto** 
2Warm

#### - **Descripción** 
¿Puedes convertir el número 42 (base 10) a binario (base 2)?

**Pista**
Envíe su respuesta en el formato de bandera de nuestro concurso. Por ejemplo, si su respuesta fue '11111', deberá enviar 'picoCTF{11111}' como bandera.
#### - **Solución** 
el número **42** en base 10 convertido a binario (base 2) es:
**Dividir por 2 y registrar el residuo**:

- 42 ÷ 2 = **21**, residuo **0**
- 21 ÷ 2 = **10**, residuo **1**
- 10 ÷ 2 = **5**, residuo **0**
- 5 ÷ 2 = **2**, residuo **1**
- 2 ÷ 2 = **1**, residuo **0**
- 1 ÷ 2 = **0**, residuo **1**
- 
- picoCTF{101010}

#### - Referencias 
https://gchq.github.io/CyberChef/