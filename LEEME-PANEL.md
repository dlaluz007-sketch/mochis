# Mochis · Sitio + Panel de administración

## Qué hay en la carpeta
- `index.html` → página pública (la del QR). Lee el menú desde `menu.json`.
- `admin.html` → tu panel. Edita `menu.json` y sube fotos a `fotos/`.
- `menu.json` → todos los productos y el menú programado por fecha.
- `fotos/`, `banners/`, `logo.png`, `logo-circulo.png` → imágenes.

## Puesta en marcha (una sola vez)
1. Crea una cuenta en **github.com** y un repositorio **público** nuevo (ej. `mochis`).
2. Sube TODO el contenido de esta carpeta al repositorio (botón *Add file → Upload files*).
3. En el repositorio: *Settings → Pages → Branch: main / (root) → Save*. Tu sitio quedará en
   `https://TU-USUARIO.github.io/mochis/` (ese link es el que va en el QR).
4. Crea un token: *Settings (de tu cuenta) → Developer settings → Personal access tokens →
   Fine-grained tokens → Generate new token*.
   - Repository access: **Only select repositories** → elige `mochis`.
   - Permissions → Repository permissions → **Contents: Read and write**.
   - Copia el token (solo se muestra una vez).
5. Abre `admin.html` (en tu computadora, o en `.../mochis/admin.html`), pulsa **Conexión** y escribe
   tu usuario, el repositorio (`mochis`), la rama (`main`) y el token → **Conectar**.

## Uso diario
- **🗓️ Agregar menú manual:** elige la fecha, y arrastra (o toca) los productos desde "Mis productos"
  al "Menú del día". Se agrupan solos por apartado (Panadería, Gelatinas, Desayunos…). Quita con ✕.
  Al terminar pulsa **Guardar y publicar este menú**.
- **➕ Agregar producto nuevo:** nombre, descripción, apartado (elige uno o escribe uno nuevo), foto
  (se achica sola) → **Guardar**. Se guarda, se publica y ya aparece en "Mis productos" para armar menús.
- **✎ en cada producto:** editar nombre, descripción, foto, apartado, o borrarlo.
- Si un día no se programa, se muestran los productos marcados "Sale por defecto".
- La página pública se actualiza en 1 o 2 minutos tras publicar.

## Seguridad
- El token se guarda solo en el navegador donde lo escribes. Úsalo en tu computadora, no en equipos ajenos.
- No pongas el link de `admin.html` en el QR ni en redes. Sin el token nadie puede guardar cambios,
  y si el token se filtra, bórralo en GitHub y crea otro.
- Si alguien cambia `menu.json` desde otro lugar, el panel avisará (error 409): reconecta para recargar.

## Notas
- Las fotos se suben ya redimensionadas (máx. 800 px) para que la página cargue rápido.
- Los banners (`banners/`) se asignan por día de la semana en `menu.json`, sección `"banners"`
  (por ahora se editan a mano en ese archivo).
- `index.html` debe abrirse desde un sitio web (GitHub Pages, Netlify); si lo abres con doble clic
  desde tu disco, el navegador bloquea la lectura de `menu.json`.
