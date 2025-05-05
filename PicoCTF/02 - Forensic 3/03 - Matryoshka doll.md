#### - **Descripción** 
Las matrioskas son un conjunto de muñecas de madera de tamaño decreciente, colocadas una dentro de otra. ¿Cuál es la última? Imagen: [esta](https://mercury.picoctf.net/static/205adad23bf9d8303081a0e71c9beab8/dolls.jpg)
#### Pista 
Espera, ¿se pueden ocultar archivos dentro de otros archivos? ¿Pero cómo encontrarlos?

Asegúrese de enviar la bandera como picoCTF{XXXXX}
#### - **Solución** 
3_c.jpg  _3_c.jpg.extracted
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images$ cd _3_c.jpg.extracted/
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted$ ls
1E2D6.zip  base_images
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted$ cd base_images/
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images$ ls
4_c.jpg
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images$ binwalk -e 4_c.jpg

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             PNG image, 320 x 768, 8-bit/color RGBA, non-interlaced
3226          0xC9A           TIFF image data, big-endian, offset of first image directory: 8
79578         0x136DA         Zip archive data, at least v2.0 to extract, compressed size: 63, uncompressed size: 81, name: flag.txt
79785         0x137A9         End of Zip archive, footer length: 22

richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images$ ls
4_c.jpg  _4_c.jpg.extracted
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images$ cd _4_c.jpg.extracted/
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images/_4_c.jpg.extracted$ ls
136DA.zip  flag.txt
richi@RicardoMedina:~/_dolls.jpg.extracted/base_images/_2_c.jpg.extracted/base_images/_3_c.jpg.extracted/base_images/_4_c.jpg.extracted$ cat flag.txt
picoCTF{96fac089316e094d41ea046900197662}


picoCTF{96fac089316e094d41ea046900197662}