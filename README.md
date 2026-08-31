# Water Monterreal — sitio estático

Sitio de una sola página (`index.html`), sin build ni dependencias. Listo para desplegar en Vercel.

## Opción A — Arrastrar y soltar (más rápido, sin cuenta de GitHub)
1. Entra a https://vercel.com/new
2. Elige **"Deploy without Git" / "Browse all templates" → Upload**, o arrastra esta carpeta completa a la zona de carga.
3. Framework Preset: **Other** (sitio estático, no requiere build command).
4. Deploy.

## Opción B — Vercel CLI
```bash
npm i -g vercel
cd monterreal-web
vercel        # deploy de prueba
vercel --prod # deploy a producción
```

## Opción C — Conectado a un repositorio Git
1. Sube esta carpeta a un repo de GitHub/GitLab/Bitbucket.
2. En Vercel: **Add New → Project** → importa el repo.
3. Framework Preset: **Other**. Build Command: (vacío). Output Directory: `.` (raíz).
4. Deploy.

## Notas
- No hay `package.json` ni proceso de build: Vercel sirve los archivos tal cual (HTML/CSS/JS inline + imágenes).
- `vercel.json` agrega URLs limpias y cache de un año para imágenes/íconos.
- Dominio propio: en el proyecto de Vercel → **Settings → Domains** → agrega `watermonterreal.cr` (o el dominio que uses) y sigue las instrucciones de DNS.
