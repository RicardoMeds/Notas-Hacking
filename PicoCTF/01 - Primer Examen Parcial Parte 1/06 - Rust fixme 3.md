#### - **Descripción** 
¿Has oído hablar de Rust? ¡Corrige los errores de sintaxis en este archivo de Rust para imprimir la bandera!Descargue el código de Rust [aquí](https://challenge-files.picoctf.net/c_verbal_sleep/dcdaf491b35c1d0f5075e9583edbbb7aaea1dffb6ad32bc000e4d87b5200ff7b/fixme3.tar.gz) .

#### Pista 
Lee los comentarios...¡maldita sea!
#### - **Solución** 
Entrar al codigo main y editar el codigo para corregir los errores:
Solo era quitar unos comentarios y listo:
richi@RicardoMedina:~/fixme3/src$ nano main.rs
richi@RicardoMedina:~/fixme3/src$ cargo build
   Compiling rust_proj v0.1.0 (/home/richi/fixme3)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 2.65s
richi@RicardoMedina:~/fixme3/src$ cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.01s
     Running `/home/richi/fixme3/target/debug/rust_proj`
Using memory unsafe languages is a: PARTY FOUL! Here is your flag: picoCTF{n0w_y0uv3_f1x3d_1h3m_411}
richi@RicardoMedina:~/fixme3/src$

picoCTF{n0w_y0uv3_f1x3d_1h3m_411}
