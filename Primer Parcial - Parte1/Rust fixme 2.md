### Descripción: 
¿La saga de Rust continúa? ¿Me lo prestas, por favooooor?
Descarga el código de Rust aquí.
### Solución:
picoCTF{4r3_y0u_h4v1n5_fun_y31?}
### Notas:
La variable party_foul mutable (mut), la pase como una referencia mutable (&mut) y actualice la función decrypt para que aceptara dicha referencia, solucionando así los errores de "préstamo" de Rust.
### Referencias:
