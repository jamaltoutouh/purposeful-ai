# Sitio estático para GitHub Pages

Sitio limpio con HTML/CSS listo para publicar en GitHub Pages.

## Archivos

- `index.html`: página principal.
- `404.html`: página de error personalizada.
- `_config.yml`: configuración del sitio.

## Editar contenido

Modifica `index.html` directamente: cambia textos, agrega secciones, personaliza estilos.

## Publicar en GitHub Pages

Ya está en un repositorio Git. Para publicar:

### 1. Configura la rama y el usuario (si aún no lo has hecho)

```zsh
cd "/Users/jamal/Research-Production/Proyecto Pi-GANs/web"

# Si es la primera vez
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@gmail.com"
```

### 2. Haz commit y push

```zsh
cd "/Users/jamal/Research-Production/Proyecto Pi-GANs/web"

git add .
git commit -m "Sitio estático inicial"
git push origin main
```

### 3. Activa GitHub Pages

En GitHub:
1. Ve al repositorio → **Settings** → **Pages**
2. Source: selecciona `Branch: main`, `Folder: / (root)`
3. Espera a que el build termine (~1 minuto)
4. Tu sitio estará en: `https://jamaltoutouh.github.io/NOMBRE_DEL_REPO`

## Dominio personalizado (opcional)

Crea un archivo `CNAME` en la raíz:

```
tu-dominio.com
```

Configura los registros DNS en tu proveedor de dominios.

## Vista previa local

Abre `index.html` en el navegador o usa un servidor local:

```zsh
cd "/Users/jamal/Research-Production/Proyecto Pi-GANs/web"
python3 -m http.server 8000
# Abre: http://localhost:8000
```
