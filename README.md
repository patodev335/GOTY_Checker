# Bingo de los GOTY

Un cartón de bingo para la noche de los premios. Cada persona escribe sus predicciones y las tacha cuando se cumplen. Una fila, columna o diagonal completa activa la animación y el sonido de victoria.

## Publicarlo con GitHub Pages

1. Creá un repositorio público nuevo en GitHub.
2. Subí `index.html`, `logo.png`, `1.mp3`, `bond.mp3` y `wololo.mp3` a la raíz del repo (con esos nombres exactos).
3. Andá a **Settings → Pages**. En **Build and deployment** elegí **Deploy from a branch**, seleccioná `main` y `/ (root)`, y guardá.
4. Al minuto el sitio queda online en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Cómo funciona

- **Agregar predicción** completa la próxima casilla vacía (también podés tocar cualquier casilla vacía).
- Cada predicción pide tu nombre y un color. Cada persona tiene un color único: los colores ya usados aparecen tachados y, si repetís un nombre, se reutiliza su color. El nombre se muestra abajo de la casilla en ese color.
- Tocá una casilla para tacharla con una X roja. Tocala de nuevo para deshacer.
- **Editar casillas** activa el modo edición: tocá una casilla para cambiarla o eliminarla.
- El campo **Ancho** (arriba) define cuántas casillas tiene la grilla por lado, de 2 a 10.
- Una línea cuenta solo si todas sus casillas están completas y tachadas.
- Si tachás una casilla pegada a otra ya tachada (de lado o en diagonal), aparece "¡COMBO!" con su sonido.
- Sin configurar nada, cada cartón se guarda solo en el navegador de cada persona. Para que **todos compartan el mismo cartón** (con sus colores únicos), seguí los pasos de abajo.
- El botón de sonido silencia el sonido de victoria.
- El control de volumen va de 0 a 300 % (se puede amplificar, con un limitador para evitar distorsión), ajusta todos los sonidos y se recuerda en cada navegador. Al soltarlo suena un "bloop" de gota para mostrar el nivel. Si suenan dos sonidos a la vez, solo sobrevive el último. En iPhone/iPad el volumen del teléfono sigue mandando.
- Al pasar el mouse sobre el logo aparece un botón verde "?" que reproduce un sonido secreto.

## Cartón compartido entre amigos (Firebase, gratis)

1. Entrá a https://console.firebase.google.com y creá un proyecto (podés desactivar Analytics).
2. En el menú **Build → Realtime Database**, creá una base de datos. Elegí **modo de prueba** (test mode).
3. Copiá la URL de la base (algo como `https://mi-proyecto-default-rtdb.firebaseio.com`).
4. Abrí `index.html`, buscá la línea `const FIREBASE_URL = '';` y pegá la URL entre las comillas.
5. Subí el sitio a GitHub Pages. Todos los que abran el link ven y editan el mismo cartón, y se actualiza solo cada pocos segundos.

Notas:
- Para tener varios cartones distintos, usá `?sala=nombre` al final del link (por ejemplo `.../?sala=amigos`).
- El modo de prueba de Firebase deja la base abierta a cualquiera que tenga la URL y vence a los 30 días. Para después, cambiá las reglas en la pestaña **Reglas**.
