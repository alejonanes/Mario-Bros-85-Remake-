# Super Mario Bros - Web Edition 🍄

Una recreación web del clásico juego "Super Mario Bros" (1985) desarrollado utilizando HTML5, CSS3 y JavaScript Vanilla. Este proyecto está diseñado para funcionar directamente en el navegador de manera fluida y sin requerir la instalación de dependencias, frameworks, o configuraciones de servidor.

## 🎮 Controles

| Acción | Teclado |
| :--- | :--- |
| **Moverse** | `Flechas direccionales` o `W A S D` |
| **Saltar** | `Espacio` o `Z` |
| **Correr / Disparar** | `X` |
| **Iniciar / Pausa** | `Enter` |

*También incluye controles táctiles en pantalla para dispositivos móviles.*

## 🚀 Cómo jugar

Existen dos formas sencillas de ejecutar este proyecto:

### Opción 1: Juego Local
Simplemente descarga o clona este repositorio y abre el archivo `index.html` haciendo doble clic sobre él. Se abrirá en tu navegador predeterminado y podrás jugar inmediatamente.

### Opción 2: Publicarlo para todo el mundo (GitHub Pages)
Dado que es un proyecto estático, puedes alojarlo gratis en **GitHub Pages** para compartir el enlace con tus amigos:

1. Sube este código a un repositorio público en tu cuenta de GitHub.
2. Ve a la pestaña **Settings** (Configuración) de tu repositorio.
3. En el menú lateral izquierdo, haz clic en **Pages** (Páginas).
4. En la sección *Build and deployment*, busca **Source** y asegúrate de que esté seleccionado "Deploy from a branch".
5. En **Branch**, selecciona tu rama principal (normalmente `main` o `master`) y la carpeta `/ (root)`.
6. Haz clic en **Save** (Guardar).
7. Espera unos minutos y recarga la página. Aparecerá un mensaje indicando que tu sitio está publicado junto con un enlace (ej. `https://tu-usuario.github.io/tu-repositorio/`). ¡Comparte ese enlace!

## 📁 Arquitectura del Código

El proyecto sigue una estructura limpia orientada a componentes lógicos separados en distintos archivos dentro de la carpeta `/js`:

- `index.html` & `style.css`: Interfaz de usuario, menú principal, controles móviles y canvas.
- `game.js`: El bucle principal del juego (`requestAnimationFrame`) y la gestión de estados (menú, jugando, pausa, game over).
- `config.js`: Constantes de gravedad, velocidad, fricción y tamaños.
- `renderer.js`: Se encarga exclusivamente de dibujar en el contexto 2D del Canvas.
- `entities.js`: Clases y lógica de colisión para Mario, Goombas, Koopas, Monedas y Power-ups.
- `levels.js`: Matriz de datos para cargar y parsear la geometría de los niveles (bloques, tuberías, etc.).
- `input.js`: Listener para el teclado y los botones táctiles en pantalla.
- `sprites.js` & `audio.js`: Manejo y precarga de los recursos multimedia.

## ⚖️ Licencia
Este es un proyecto educativo sin fines de lucro creado con el propósito de aprender y demostrar las capacidades del Canvas HTML5 y JavaScript. Los recursos gráficos y auditivos pertenecen a Nintendo®.
