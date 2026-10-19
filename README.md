# GPD 2

Prototipo funcional de una red social para amantes del cine (proyecto de la materia): rankeá películas, sumá amigos por nombre de usuario y descubrí qué ver con ellos.

## Funciones
- Cuenta con usuario único y contraseña (Firebase Authentication).
- Ranking de películas con estrellas y reseñas cortas.
- **Match con amigos:** recomendaciones grupales con % de afinidad, filtrando por géneros.
- **Gemelo de gustos:** personas que no son tus amigos pero rankean parecido, con chat.
- **Trivias en grupo:** "¿Quién la escribió?" y "Adiviná la portada", con enlace compartido, puntaje en vivo y podio.
- Diseño responsive: se adapta solo a celular o computadora.

## Tecnología
HTML + CSS + JavaScript en un solo archivo (`index.html`). Datos en Firebase (Authentication y Firestore). Búsqueda opcional de películas con la API de TMDB.

## Publicar
1. Subir `index.html` (y `.nojekyll`) a un repositorio público.
2. Settings > Pages > Deploy from a branch > `main` / root.
3. En Firebase: Authentication > Settings > Authorized domains > agregar `TU-USUARIO.github.io`.
4. En Firebase: habilitar Correo electrónico/contraseña y publicar `firestore.rules`.

## Modo local
Agregando `?local` a la dirección funciona sin servidor (cada pestaña es un usuario distinto), útil para mostrarlo sin internet.

_Este producto usa la API de TMDB pero no está avalado ni certificado por TMDB._
