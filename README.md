# Portfolio de desarrollo e investigación cuántica

Portfolio estático para mostrar proyectos de desarrollo de software, investigación doctoral en computación cuántica y formación. Escrito en HTML, CSS y JavaScript; no necesita dependencias, proceso de compilación ni paso de instalación.

## Publicar en GitHub Pages

1. Sube los cambios al repositorio.
2. En GitHub, abre **Settings → Pages**.
3. En **Build and deployment**, selecciona **Deploy from a branch**, la rama `main` y la carpeta `/ (root)`.
4. Guarda la configuración. GitHub mostrará la dirección de tu sitio en esa misma página.

La página se sirve desde [index.html](index.html). Como carga datos JSON con `fetch`, previsualízala con un servidor HTTP local (por ejemplo, `python3 -m http.server 8000`) y abre `http://localhost:8000`.

## Editar el sitio con Pages CMS

1. Sube el repositorio a GitHub y activa GitHub Pages según las instrucciones anteriores.
2. Abre [app.pagescms.org](https://app.pagescms.org/) e inicia sesión con GitHub.
3. Autoriza Pages CMS para acceder a este repositorio y selecciónalo en la aplicación.
4. Edita **Perfil del sitio**, **Proyectos**, **Experiencia y doctorado** o **Formación** en el panel.
5. Guarda los cambios en la rama publicada. GitHub Pages volverá a desplegar el sitio con el contenido actualizado.

La configuración del editor está en [.pages.yml](.pages.yml); los datos iniciales están en [content/profile.json](content/profile.json), [content/projects.json](content/projects.json), [content/experience.json](content/experience.json) y [content/education.json](content/education.json). Una vez conectado Pages CMS, puedes actualizarlos desde el panel sin editar HTML ni JSON. La primera vez tendrás que iniciar sesión y autorizar la aplicación de Pages CMS para acceder a tu repositorio de GitHub.

En los campos de imagen puedes subir una imagen al repositorio, donde quedará guardada en `media/`, o introducir una URL externa. Los datos personales marcados como ejemplo, el correo y los enlaces sociales deben sustituirse por los tuyos desde el panel antes de publicar.

## Previsualizar localmente

Como el sitio carga los JSON con `fetch`, previsualízalo mediante HTTP y no abriendo el archivo directamente. Ejecuta `python3 -m http.server 8000` desde la raíz y visita `http://localhost:8000`.
