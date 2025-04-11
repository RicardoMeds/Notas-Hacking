#### - **Descripción** 

¿La saga Rust continúa? ¿Me lo prestas, por favooooor?Descargue el código de Rust [aquí](https://challenge-files.picoctf.net/c_verbal_sleep/babfbee79718a6363826ba86300173ffde6d81577e9dd07d4130c53a7eecf6c3/fixme2.tar.gz) .

#### Pista 
https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html

#### - **Solución** 
Entrar al codigo main y editar el codigo para corregir los errores:
richi@RicardoMedina:~/fixme2/src$ nano main.rs
richi@RicardoMedina:~/fixme2/src$ cargo build
   Compiling rust_proj v0.1.0 (/home/richi/fixme2)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.57s
richi@RicardoMedina:~/fixme2/src$ cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.01s
     Running `/home/richi/fixme2/target/debug/rust_proj`
Using memory unsafe languages is a: PARTY FOUL! Here is your flag: picoCTF{4r3_y0u_h4v1n5_fun_y31?}
richi@RicardoMedina:~/fixme2/src$
picoCTF{4r3_y0u_h4v1n5_fun_y31?}