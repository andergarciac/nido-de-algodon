# Nido de Algodón

Sitio del negocio familiar "Nido de Algodón" (edredones, sábanas, cortinas y línea infantil), con panel de administración en `/admin` para editar textos, fotos y precios sin tocar código.

## Cómo funciona

- `index.html` — el sitio público. Carga el contenido desde `content/site.json`.
- `content/site.json` — todo el texto y la estructura de categorías/fotos del sitio.
- `images/uploads/` — las fotos de los productos.
- `admin/` — el panel de administración (Decap CMS), que edita `content/site.json` y sube fotos a `images/uploads/`.

## Para activar el panel de administración (una sola vez)

1. En Netlify, entra al sitio conectado a este repositorio.
2. Ve a **Site configuration → Identity** y haz clic en **Enable Identity**.
3. En la configuración de Identity, en **Registration**, elige **Invite only** (para que solo las personas invitadas puedan entrar).
4. Ve a **Identity → Services → Git Gateway** y haz clic en **Enable Git Gateway**.
5. Ve a **Identity → Invite users** e invita el correo de la persona que va a administrar el sitio (por ejemplo, tu mamá). Le llegará un correo para crear su contraseña.
6. Listo — esa persona puede entrar en `tu-sitio.netlify.app/admin` con su correo y contraseña, y editar textos, fotos y precios. Los cambios quedan publicados automáticamente en unos minutos (Netlify reconstruye el sitio solo).
