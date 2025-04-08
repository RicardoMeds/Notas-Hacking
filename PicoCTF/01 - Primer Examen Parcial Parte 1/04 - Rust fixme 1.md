#### - **Descripción** 
#### Description

¿Has oído hablar de Rust? ¡Corrige los errores de sintaxis en este archivo de Rust para imprimir la bandera!Descargue el código de Rust [aquí](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz) .
#### Pista 
Cargo es el gestor de paquetes de Rust y te facilitará la vida. Consulta la página de inicio [aquí.](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html)

Rust tiene algunos mensajes de error del compilador muy interesantes. ¿Quizás leerlos?
#### - **Solución** 
richi@RicardoMedina:/tmp/rust_proj$ ls
Cargo.lock  Cargo.toml  fixme1  src  target
richi@RicardoMedina:/tmp/rust_proj$ cd src
richi@RicardoMedina:/tmp/rust_proj/src$ ls
main.rs
richi@RicardoMedina:/tmp/rust_proj/src$ nano main.rs
richi@RicardoMedina:/tmp/rust_proj/src$ cd ..
richi@RicardoMedina:/tmp/rust_proj$ cargo build
   Compiling rust_proj v0.1.0 (/tmp/rust_proj)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.85s
richi@RicardoMedina:/tmp/rust_proj$ cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/rust_proj`
picoCTF{4r3_y0u_4_ru$t4c30n_n0w?}
richi@RicardoMedina:/tmp/rust_proj$

picoCTF{4r3_y0u_4_ru$t4c30n_n0w?}
