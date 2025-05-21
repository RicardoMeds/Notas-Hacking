#### - **Descripción** 
¿Qué ocurre si el exponente es pequeño? Sin embargo, hay una peculiaridad: hemos rellenado el texto plano para que (M ** e) sea apenas mayor que N. Descifrémoslo: [texto cifrado.](https://mercury.picoctf.net/static/81689952b7442c3e23a9f703198c0a4c/ciphertext)

*PISTAS* 
[Tutorial](https://en.wikipedia.org/wiki/RSA_\(cryptosystem\)) de RSA[](https://en.wikipedia.org/wiki/RSA_\(cryptosystem\))
¿Cómo podría afectar un valor demasiado pequeño `e`la seguridad de esta clave?
Asegúrate de no perder precisión, los números son bastante grandes (además del `e`valor)
No deberías tener que hacer _demasiadas_ conjeturas
`pico`Está en la bandera, pero no al principio.

#### - **Solución** 
from decimal import *
from tqdm import tqdm

N = Decimal(16157656843214630540782260519598878842336783177348929017407633211352136367960754624019502746024050951385898>e = Decimal(3)
c = Decimal(12200123185888718861325247578988844221745345580555937133090883049102739910735547326599771339806853708992578>

def int_to_ascii(m):
    # Decode to ascii (from https://crypto.stackexchange.com/a/80346)
    m_hex = hex(int(m))[2:-1]  # Number to hex
    m_ascii = "".join(
        chr(int(m_hex[i : i + 2], 16)) for i in range(0, len(m_hex), 2)
    )  # Hex to Ascii
    return m_ascii
Find padding
getcontext().prec = 280  # Increase precision
padding = 0
for k in tqdm(range(0, 10_000)):
    m = pow(k * N + c, 1 / e)

    m_ascii = int_to_ascii(m)

    if "pico" in m_ascii:
        padding = k
        break

print("Padding: %s" % padding)

#Increase precision further to get entire flag
getcontext().prec = 700

m = pow(padding * N + c, 1 / e)
m_ascii = int_to_ascii(m)
print("Flag: %s" % m_ascii.strip())

picoCTF{e_sh0u1d_b3_lArg3r_7adb35b1