# Mis Restaurantes

App personal para llevar el control de tus restaurantes favoritos, reservas y visitas. Funciona como una app instalable en iPhone/iPad (PWA), sin necesidad de subirla a la App Store.

## Contenido del proyecto

```
index.html          → la app completa (HTML + CSS + JS en un solo fichero)
manifest.json        → configuración de la app instalable (nombre, colores, iconos)
icons/
  icon-192.png        → icono 192x192
  icon-512.png        → icono 512x512
  apple-touch-icon.png → icono 180x180 para iOS
  favicon-32.png       → icono pequeño para la pestaña del navegador
```

---

## Paso 1 — Subir el proyecto a GitHub

1. Entra en [github.com](https://github.com) e inicia sesión (o crea una cuenta gratuita).
2. Pulsa el botón **"+"** de arriba a la derecha → **"New repository"**.
3. Ponle un nombre, por ejemplo `mis-restaurantes`. Puede ser público o privado (para GitHub Pages gratis, debe ser **público**).
4. Pulsa **"Create repository"**.
5. En la página del repositorio recién creado, pulsa **"uploading an existing file"** (o el botón **"Add file" → "Upload files"**).
6. Arrastra dentro **todo el contenido** de esta carpeta descomprimida (el fichero `index.html`, `manifest.json`, y la carpeta `icons` completa con sus 4 imágenes). Asegúrate de que `icons` se sube como carpeta, no que las imágenes queden sueltas en la raíz.
7. Abajo, escribe un mensaje como "Primera versión" y pulsa **"Commit changes"**.

## Paso 2 — Activar GitHub Pages

1. Dentro del repositorio, ve a **"Settings"** (arriba a la derecha).
2. En el menú de la izquierda, pulsa **"Pages"**.
3. En **"Branch"**, selecciona `main` (o `master`) y la carpeta `/ (root)`. Pulsa **"Save"**.
4. Espera 1-2 minutos. GitHub te mostrará una URL parecida a:
   `https://tu-usuario.github.io/mis-restaurantes/`
5. Esa es la dirección de tu app. Guárdala.

## Paso 3 — Instalar en iPhone / iPad

1. Abre **Safari** (tiene que ser Safari, no Chrome ni otro navegador) en el iPhone o iPad.
2. Ve a la URL del Paso 2.
3. Pulsa el icono **⬆️ Compartir** (el cuadrado con la flecha hacia arriba) en la barra inferior (iPhone) o superior (iPad).
4. Baja hasta **"Añadir a pantalla de inicio"** y pulsa.
5. Pulsa **"Añadir"** arriba a la derecha.

Verás el icono del plato, tenedor y cuchillo en tu pantalla de inicio, y al abrirlo funcionará a pantalla completa como una app normal, sin barra de Safari.

Repite el Paso 3 en cada dispositivo (iPhone, iPad) donde quieras instalarla — es la misma URL para todos.

## Actualizar la app en el futuro

Cuando tengas una nueva versión de `index.html` (por ejemplo, generada aquí en Claude), solo tienes que:
1. Entrar en el repositorio de GitHub.
2. Abrir el fichero `index.html` → pulsar el lápiz (✏️ Edit) → pegar el contenido nuevo → "Commit changes".
   *(O bien "Add file → Upload files" y subir el nuevo `index.html`, sobrescribiendo el anterior.)*
3. Los cambios tardan uno o dos minutos en aparecer en GitHub Pages.
4. En el iPhone/iPad no hace falta reinstalar nada: la próxima vez que abras la app instalada, Safari cargará la versión nueva automáticamente (puede que tengas que cerrarla del todo y reabrirla una vez).

## Notas

- Los datos de tus restaurantes se guardan **en el propio dispositivo** (localStorage), no en GitHub. Cada iPhone/iPad tendrá su propia lista independiente salvo que uses **Exportar JSON / Importar JSON** desde "Acerca de" para pasar los datos de un dispositivo a otro.
- El icono que verás en la pantalla de inicio es el que subiste (plato, tenedor y cuchillo sobre fondo naranja).
