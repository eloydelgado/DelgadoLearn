# Guía de Contribución

¡Gracias por querer contribuir a DelgadoLearn! Este es un proyecto comunitario y colaborativo.

## 📋 Antes de Empezar

1. Asegúrate de tener acceso al repositorio
2. Familiarízate con nuestra [estructura de contenido](#estructura-de-contenido)
3. Revisa los [estándares de contenido](#estándares-de-contenido)

## 🏗️ Estructura de Contenido

```
docs/
├── index.md              # Página principal
├── contributing.md       # Esta guía
├── cursos/              # Todos los cursos
│   ├── intro.md
│   └── nivel-basico/
│       ├── modulo-1/
│       │   ├── leccion-1.md
│       │   └── leccion-2.md
│       └── modulo-2/
├── assets/              # Imágenes, videos, recursos
└── snippets/            # Ejemplos de código reutilizables
```

## ✏️ Cómo Contribuir

### Opción 1: Pull Request (Recomendado)

1. Fork el repositorio
2. Crea una rama: `git checkout -b feature/nuevo-curso`
3. Realiza tus cambios
4. Commit: `git commit -m "Add: nuevo curso de X"`
5. Push: `git push origin feature/nuevo-curso`
6. Abre un Pull Request

### Opción 2: Issues

Si encuentras un error o tienes una sugerencia, abre un Issue describiendo:
- Qué encontraste (error, contenido desactualizado, etc.)
- Dónde (página, sección)
- Sugerencia de solución (si aplica)

## 📝 Estándares de Contenido

### Formato y Estructura

- Usa **Markdown** con extensiones de Material for MkDocs
- Cada curso debe tener: Descripción, Objetivos, Contenido, Ejercicios
- Estructura jerárquica clara: Curso → Módulo → Lección

### Ejemplo de Estructura

```markdown
# Nombre del Curso

## Descripción
[Descripción breve del curso]

## Objetivos
- Objetivo 1
- Objetivo 2
- Objetivo 3

## Contenido

### Módulo 1: Introducción
#### Lección 1.1: Conceptos Básicos
[Contenido]

#### Lección 1.2: Primer Ejercicio
[Contenido]

### Módulo 2: Nivel Intermedio
[...]

## Ejercicios Prácticos
[Descripción de ejercicios]

## Referencias
- [Link 1](url)
- [Link 2](url)
```

## Estándares de Redacción

- ✅ Lenguaje claro y conciso
- ✅ Español neutro (evitar regionalismos)
- ✅ Ejemplos prácticos y reales
- ✅ Incluir referencias externas
- ❌ No copiar contenido protegido sin atribuir
- ❌ Evitar promoción de productos/servicios

```python
# Incluye explicaciones claras
def ejemplo_funcion(parametro):
    """Descripción de qué hace esta función."""
    resultado = parametro * 2
    return resultado
```

## 🖼️ Agregar Imágenes y Recursos

1. Guarda en `docs/assets/`
2. Organiza por curso/módulo
3. Usa nombres descriptivos: `curso-nombre-concepto.png`
4. Comprime imágenes antes de subir
5. Incluye alt text en Markdown:

```markdown
![Descripción de la imagen](../assets/imagen.png)
```

## 🎬 Embeber Videos

```markdown
<iframe width="100%" height="400" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
```

## 🔍 Antes de Hacer Submit

- [ ] El contenido es original o está correctamente atribuido
- [ ] Las imágenes tienen alt text
- [ ] Los enlaces funcionan
- [ ] La ortografía está correcta
- [ ] El formato es consistente
- [ ] Testeaste localmente: `mkdocs serve`

## 📊 Proceso de Review

1. Se revisa el PR en 24-48 horas
2. Se solicitan cambios si es necesario
3. Se aprueba y fusiona
4. Se publica automáticamente en GitHub Pages

## ❓ Preguntas?

- Abre un Discussion en GitHub
- Contacta al equipo de Learning & Development

¡Gracias por contribuir! 🙌
