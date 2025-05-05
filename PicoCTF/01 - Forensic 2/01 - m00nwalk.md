#### - **Descripción** 
Decode this [message](https://jupiter.challenges.picoctf.org/static/d6fcea5e3c6433680ea4f914e24fab61/message.wav) from the moon.

#### Pista 
How did pictures from the moon landing get sent back to Earth?
What is the CMU mascot?, that might help select a RX option
#### - **Solución** 
richi@RicardoMedina:~/moonwalk$ cd /opt
richi@RicardoMedina:/opt$ sudo git clone https://github.com/colaclanth/sstv.git
[sudo] password for richi:
Sorry, try again.
[sudo] password for richi:
Cloning into 'sstv'...
remote: Enumerating objects: 221, done.
remote: Counting objects: 100% (59/59), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 221 (delta 51), reused 49 (delta 49), pack-reused 162 (from 1)
Receiving objects: 100% (221/221), 1.01 MiB | 2.75 MiB/s, done.
Resolving deltas: 100% (139/139), done.
richi@RicardoMedina:/opt$ cd sstv/
richi@RicardoMedina:/opt/sstv$ python3 setup.py install
richi@RicardoMedina:/opt/sstv$ sudo python3 setup.py install
richi@RicardoMedina:~/moonwalk$ sstv -d message.wav -o result.png
![[Pasted image 20250429224019.png]]
picoCTF{beep_boop_im_in_space}

