#### - **Descripción** 
¿Qué tal un poco de escondite?Descargue este archivo [aquí](https://artifacts.picoctf.net/c_titan/6/unknown.zip) .
#### Pista 
¿Cómo puedo ver la información sobre la imagen?
Si algo no está en la forma esperada, ¿tal vez merezca atención?
#### - **Solución** 
richi@RicardoMedina:~$ unzip unknown.zip
Archive:  unknown.zip
  inflating: ukn_reality.jpg
richi@RicardoMedina:~$ exiftool ukn_reality.jpg
ExifTool Version Number         : 12.40
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.2 MiB
File Modification Date/Time     : 2024:02:15 16:40:21-06:00
File Access Date/Time           : 2024:02:15 16:40:21-06:00
File Inode Change Date/Time     : 2025:05:12 21:52:59-06:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fYTZkZjhkYjh9Cg==

y utilice el cyberchf 
picoCTF{ME74D47A_HIDD3N_a6df8db8}

#### - **Referencias** 
https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=Y0dsamIwTlVSbnROUlRjMFJEUTNRVjlJU1VSRU0wNWZZVFprWmpoa1lqaDlDZz09