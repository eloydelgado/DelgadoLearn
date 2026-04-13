# DelgadoLearn

Portal de aprendizaje autocontenido y colaborativo publicado en GitHub Pages. 

## 🚀 Inicio Rápido

### Requisitos
- Python 3.8+
- pip

### Instalación

1. Clone el repositorio:
```bash
git clone https://github.com/delgadolearn/delgadolearn.git
cd delgadolearn
```

2. Instale las dependencias:
```bash
pip install -r requirements.txt
```

3. Ejecute el servidor local:
```bash
mkdocs serve
```

4. Abra su navegador en `http://localhost:8000`

## 📝 Estructura del Proyecto

```
delgadolearn/
├── docs/
│   ├── index.md                 # Página principal
│   ├── contributing.md          # Guía de contribución
│   ├── comunidad.md            # Sección de comunidad
│   ├── cursos/                 # Todos los cursos
│   │   ├── intro.md
│   │   └── [cursos futuros]
│   └── assets/                 # Imágenes y recursos
├── mkdocs.yml                   # Configuración de MkDocs
├── requirements.txt             # Dependencias Python
└── .github/workflows/           # CI/CD automático
    └── deploy.yml
```

## 🤝 Contribución

¿Quieres ayudar? Lee nuestra [Guía de Contribución](docs/contributing.md)

En resumen:
1. Fork del repositorio
2. Crea una rama (`git checkout -b feature/nuevo-contenido`)
3. Haz commit de tus cambios
4. Push a la rama (`git push origin feature/nuevo-contenido`)
5. Abre un Pull Request

## 🌐 Publicación

El sitio se publica automáticamente en GitHub Pages cuando haces push a `main`:

- **URL**: https://delgadolearn.github.io/
- **Rama de publicación**: `gh-pages` (generada automáticamente)

## 🛠️ Desarrollo Local

### Comandos Útiles

```bash
# Servidor local con recarga automática
mkdocs serve

# Compilar sitio estático
mkdocs build

# Limpiar archivos generados
mkdocs build --clean
```

### Pre-visualizar cambios

Mientras ejecutas `mkdocs serve`, cualquier cambio en los archivos `.md` se reflejará automáticamente en el navegador.

## 📋 Roadmap

- [ ] Agregar primer curso
- [ ] Configurar sistema de comentarios (Utterances)
- [ ] Implementar búsqueda avanzada
- [ ] Traducción a otros idiomas
- [ ] Sistema de certificaciones

## 📞 Soporte

- 💬 [GitHub Discussions](https://github.com/delgadolearn/delgadolearn/discussions) - Preguntas y comunidad
- 🐛 [Issues](https://github.com/delgadolearn/delgadolearn/issues) - Reportar problemas
- 📚 [Documentación de MkDocs](https://www.mkdocs.org/) - Referencia técnica

## 📄 Licencia

Este proyecto está bajo licencia [MIT](LICENSE) - siéntete libre de usarlo y adaptarlo.

---

**DelgadoLearn** - Aprendizaje colaborativo para todos 🚀
