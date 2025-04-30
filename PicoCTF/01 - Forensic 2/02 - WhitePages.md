#### - **Descripción** 
Dejé de usar Páginas Amarillas y pasé a Páginas Blancas... ¡pero [la página que me dieron](https://jupiter.challenges.picoctf.org/static/95be9526e162185c741259a75dffa0ab/whitepages.txt) está toda en blanco!

#### Pista 

#### - **Solución** 
```
# coding=utf8

text = '                     '

firstType = ' '
secondType =  ' '
binaryString = ''

for char in text: #Foreach char
	if char == firstType: #Check if it is the first type
		binaryString += '0' #Mark it as 0
	else:
		binaryString += '1' #Mark it as 1

print(binaryString) #Print result
```

root@RicardoMedina:/home/richi# nano main.py
root@RicardoMedina:/home/richi# python3 main.py
Nos da un numero en binario, y ese numero lo convertimos a ASCII y nos daria la bandera: 
picoCTF{not_all_spaces_are_created_equal_7100860b0fa779a5bd8ce29f24f586dc}

#### - **Referencias** 
https://seostudio.tools/es/binary-to-ascii#google_vignette