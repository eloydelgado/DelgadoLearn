# 🚀 DelgadoLearn - Portal Listo para Usar

## ✅ Lo que hemos creado

Tu portal **DelgadoLearn** está completamente configurado con **MkDocs**. Aquí está todo lo que necesitas:

### 📁 Estructura del Proyecto

```
DelgadoLearn/
├── docs/                           # Contenido del portal
│   ├── index.md                   # Página principal
│   ├── contributing.md            # Guía de contribución
│   ├── comunidad.md              # Sección de comunidad
│   ├── estructura-carpetas.md    # Guía de organización
│   ├── cursos/                   # Directorio de cursos
│   │   └── intro.md             # Introducción a cursos
│   ├── assets/                   # Imágenes y recursos
│   └── snippets/                # Templates para contribuidores
│       ├── leccion-template.md
│       ├── modulo-template.md
│       └── ejercicio-template.md
├── .github/
│   └── workflows/
│       └── deploy.yml            # CI/CD automático a GitHub Pages
├── mkdocs.yml                    # Configuración del portal
├── requirements.txt              # Dependencias Python
├── README.md                     # Documentación del proyecto
└── .gitignore                    # Archivos a ignorar en Git
```

## 🎯 Características

✅ **Búsqueda avanzada** - Busca por palabras clave  
✅ **Tema Material** - Interfaz moderna y responsive  
✅ **Soporte Markdown** - Contenido fácil de escribir  
✅ **Publicación automática** - GitHub Actions + GitHub Pages  
✅ **Colaborativo** - PRs para contribuciones  
✅ **Multiidioma listo** - Estructura para traducción futura  

## 🚀 Próximos Pasos

### 1. Inicializar Repositorio Git

```bash
cd DelgadoLearn
git init
git add .
git commit -m "Initial commit: DelgadoLearn portal setup

Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

### 2. Crear Repositorio en GitHub

1. Ve a https://github.com/new
2. Nombre: `delgadolearn`
3. Descripción: "Portal de aprendizaje colaborativo de la empresa"
4. Asegurate de que sea **público**
5. **No inicialices** con README (ya lo tienes)
6. Crear repositorio

### 3. Conectar Tu Repositorio Local

```bash
git remote add origin https://github.com/[tu-usuario]/delgadolearn.git
git branch -M main
git push -u origin main
```

### 4. Configurar GitHub Pages

1. Ve a Settings → Pages
2. En "Build and deployment"
3. Selecciona "Deploy from a branch"
4. Branch: `gh-pages` / `root`
5. Guarda

La URL será: `https://[tu-usuario].github.io/delgadolearn/`

## 💻 Trabajar Localmente

### Instalar Dependencias (primera vez)

```bash
pip install -r requirements.txt
```

### Servidor Local

```bash
mkdocs serve
```

Abre http://localhost:8000 en tu navegador. Cualquier cambio se reflejará automáticamente.

### Compilar Sitio Estático

```bash
mkdocs build
```

Genera la carpeta `site/` lista para publicar.

## 📚 Agregar Contenido

### Opción 1: Agregar Archivo Directamente

1. Crea un archivo en `docs/cursos/nombre-curso.md`
2. Actualiza `mkdocs.yml` con la nueva entrada
3. Prueba localmente con `mkdocs serve`

### Opción 2: Usar Templates

En `docs/snippets/` encontrarás:
- `leccion-template.md` - Template para lecciones
- `modulo-template.md` - Template para módulos
- `ejercicio-template.md` - Template para ejercicios

Copia, personaliza y coloca en tu curso.

### Ejemplo: Primer Curso

```bash
# Crear estructura
mkdir docs/cursos/python-basico
mkdir docs/cursos/python-basico/modulo-1

# Crear archivos (puedes copiar de templates)
copy docs/snippets/leccion-template.md docs/cursos/python-basico/modulo-1/leccion-1.md
```

Luego edita `mkdocs.yml`:

```yaml
nav:
  - Inicio: index.md
  - Cursos:
    - Introducción: cursos/intro.md
    - Python Básico:
      - Módulo 1:
        - Lección 1: cursos/python-basico/modulo-1/leccion-1.md
  - ...
```

## 🔄 Flujo de Contribución (Para Colaboradores)

1. **Fork** del repositorio
2. **Clone** tu fork
3. **Crea una rama**: `git checkout -b feature/nuevo-curso`
4. **Edita** y prueba localmente
5. **Commit**: `git commit -m "Add: nuevo curso de X"`
6. **Push**: `git push origin feature/nuevo-curso`
7. **Pull Request** en GitHub

Revisa `docs/contributing.md` para detalles completos.

## 📖 Documentación de Referencia

### MkDocs
- [Documentación oficial](https://www.mkdocs.org/)
- [Markdown extensions](https://python-markdown.github.io/extensions/)

### Material for MkDocs
- [Documentación](https://squidfunk.github.io/mkdocs-material/)
- [Icons & Emojis](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/)

### Markdown
- [Cheatsheet](https://www.markdownguide.org/cheat-sheet/)

## 🐛 Troubleshooting

### El servidor no inicia
```bash
# Reinstala dependencias
pip install --upgrade -r requirements.txt
mkdocs serve
```

### Cambios no aparecen
```bash
# Limpia caché
mkdocs build --clean
mkdocs serve
```

### Error: port 8000 in use
```bash
# Usa puerto diferente
mkdocs serve --dev-addr 127.0.0.1:8001
```

## ❓ Preguntas Frecuentes

**P: ¿Cómo agrego comentarios?**  
R: El tema Material permite Disqus o Utterances. Configura en `mkdocs.yml`

**P: ¿Puedo cambiar colores?**  
R: Sí, edita `mkdocs.yml` en la sección `palette`

**P: ¿Cómo agrego un logo?**  
R: Copia la imagen a `docs/assets/` y configura en `mkdocs.yml`

**P: ¿Soporte para otros idiomas?**  
R: Usa Material's i18n plugin. Consulta la documentación.

## 🎉 ¡Listo!

Tu portal está listo para:
- ✅ Desarrollo local
- ✅ Publicación en GitHub
- ✅ Actualizaciones automáticas
- ✅ Colaboración comunitaria

---

**Próximo**: Sube tu primer curso y ¡abre el portal! 🚀

Para dudas, consulta `docs/contributing.md` o abre un Issue en GitHub.
