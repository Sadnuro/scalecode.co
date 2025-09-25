# 🌐 Scale Code SAS — Landing Page

Landing page oficial de **Scale Code SAS**, empresa de tecnología e inteligencia artificial que impulsa soluciones de software e IA en Colombia y Latinoamérica.  
El sitio está diseñado para publicarse de manera gratuita con **GitHub Pages** y soporta versión **multilingüe (ES/EN)**.

---

## 📂 Estructura del repositorio

```
scalecode.co/           ← raíz del proyecto
│
├── index.html          # Landing principal (ES/EN con toggle)
├── 404.html            # Redirección para /en, /es y rutas inválidas
│
├── /assets/            # Recursos estáticos (imágenes, íconos, etc.)
│    ├── logo.svg
│    ├── og-image.jpg
│    └── ...
│
├── /css/               # (Opcional) estilos adicionales
│    └── style.css
│
└── README.md           # Documentación del repo
```

---

## 🚀 Deploy en GitHub Pages

1. Crear un repositorio en GitHub llamado **`scalecode.co`**.
2. Subir los archivos (`index.html`, `404.html`, `/assets`...).
3. Ir a **Settings → Pages**:
   - **Source**: seleccionar branch `main`, folder `/ (root)`.
4. Configurar dominio personalizado:
   - En **Custom Domain**: `scalecode.co`
   - Marcar **Enforce HTTPS**.
5. Ajustar DNS del dominio (en tu proveedor):
   - `A` → 185.199.108.153  
   - `A` → 185.199.109.153  
   - `A` → 185.199.110.153  
   - `A` → 185.199.111.153  
   - `CNAME` (www) → `<usuario>.github.io`

---

## 🌍 Multilenguaje

- El sitio soporta **Español e Inglés** con un botón `EN/ES` en la barra superior.
- El idioma se recuerda en el navegador (localStorage).
- También se puede forzar por URL:
  - `https://scalecode.co/?lang=en`
  - `https://scalecode.co/?lang=es`
- Gracias al archivo `404.html`, también funcionan:
  - `https://scalecode.co/en`
  - `https://scalecode.co/es`

---

## 🛠️ Cómo editar el sitio

- **Contenido principal** → dentro de `index.html`:
  - Hero (encabezado principal).
  - Servicios (50% software, 50% IA).
  - Soluciones IA.
  - Casos de éxito.
  - Equipo.
  - Contacto.
- **Imágenes** → en `/assets/`.
- **Colores/estilos** → configurados con [TailwindCSS](https://tailwindcss.com/) (usando CDN).
- **Textos ES/EN** → cada bloque tiene etiquetas `<span class="lang-es">` y `<span class="lang-en">`.

---

## 👨‍💻 Contribuir

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/<usuario>/scalecode.co.git
   cd scalecode.co
   ```
2. Crear una nueva rama:
   ```bash
   git checkout -b feature/nueva-seccion
   ```
3. Hacer cambios y commitear:
   ```bash
   git add .
   git commit -m "Agrega nueva sección de casos de éxito"
   ```
4. Subir cambios y abrir un Pull Request:
   ```bash
   git push origin feature/nueva-seccion
   ```

---

## ⚙️ Line endings (Windows vs Linux)

Para evitar warnings de `LF/CRLF`, este repo incluye un archivo **`.gitattributes`** con:

```
* text=auto eol=lf
```

De esta forma todos los colaboradores usan **LF** (estándar en servidores Linux).

---

## 📧 Contacto

- 🌐 [scalecode.co](https://scalecode.co)  
- 📩 contacto@scalecode.co  

---

Hecho con ❤️ por **Scale Code SAS** 🚀
