# Bingo de los GOTY

Un cartón de bingo para la noche de los premios. Cada persona escribe sus predicciones y las tacha cuando se cumplen. Una fila, columna o diagonal completa activa la animación y el sonido de victoria.

## Publicarlo con GitHub Pages

1. Creá un repositorio público nuevo en GitHub.
2. Subí `index.html`, `logo.png` y `1.mp3` a la raíz del repo (con esos nombres exactos).
3. Andá a **Settings → Pages**. En **Build and deployment** elegí **Deploy from a branch**, seleccioná `main` y `/ (root)`, y guardá.
4. Al minuto el sitio queda online en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Cómo funciona

- **Agregar predicción** completa la próxima casilla vacía (también podés tocar cualquier casilla vacía).
- Tocá una casilla para tacharla con una X roja. Tocala de nuevo para deshacer.
- **Editar casillas** activa el modo edición: tocá una casilla para cambiarla o eliminarla.
- El campo **Ancho** (arriba) define cuántas casillas tiene la grilla por lado, de 2 a 10.
- Una línea cuenta solo si todas sus casillas están completas y tachadas.
- Cada cartón se guarda en el navegador de cada persona (localStorage). No hay servidor.
- El botón de sonido silencia el sonido de victoria.
