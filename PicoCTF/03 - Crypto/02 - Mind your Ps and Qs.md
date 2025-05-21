#### - **Descripción** 
En RSA, un `e`valor pequeño puede ser problemático, pero ¿qué ocurre con [los valores](https://mercury.picoctf.net/static/bf5e2c8811afb4669f4a6850e097e8aa/values)`N` ? ¿Se puede descifrar?

*PISTAS* 
Las brocas son caras, usé solo un poco más de 100 para ahorrar dinero.
#### - **Solución** 
git clone https://github.com/RsaCtfTool/RsaCtfTool.git  
sudo apt-get install libgmp3-dev libmpc-dev  
cd RsaCtfTool  
pip3 install -r "requirements.txt"
python3 RsaCtfTool.py 
picoCTF{smal1_N_n0_g0od_55304594}