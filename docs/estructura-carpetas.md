# Estructura de Carpetas - DelgadoLearn

Guía para organizar nuevos cursos y contenido en el portal.

## 📁 Estructura Recomendada

```
docs/
├── cursos/
│   ├── intro.md                          # Página de introducción (actual)
│   ├── nivel-basico/
│   │   ├── index.md                      # Índice del nivel
│   │   ├── fundamentos/                  # Primer módulo
│   │   │   ├── index.md
│   │   │   ├── leccion-1-introduccion.md
│   │   │   ├── leccion-2-conceptos.md
│   │   │   └── leccion-3-practica.md
│   │   ├── herramientas/                 # Segundo módulo
│   │   │   ├── index.md
│   │   │   ├── leccion-1-setup.md
│   │   │   └── leccion-2-configuracion.md
│   │   └── ejercicios/
│   │       ├── index.md
│   │       └── proyecto-1.md
│   │
│   ├── nivel-intermedio/
│   │   ├── index.md
│   │   ├── modulo-avanzado/
│   │   │   └── [lecciones]
│   │   └── ejercicios/
│   │
│   └── nivel-avanzado/
│       ├── index.md
│       └── [contenido]
│
├── assets/
│   ├── images/
│   │   ├── conceptos/
│   │   ├── diagramas/
│   │   └── ejemplos/
│   ├── videos/              # Enlaces a videos (no archivos)
│   └── codigo/              # Ejemplos de código reutilizables
│
└── snippets/                # Código recurrente y plantillas
    ├── ejercicio-template.md
    ├── leccion-template.md
    └── modulo-template.md
```

## 📝 Convenciones de Nombres

### Archivos Markdown
- Usa **kebab-case**: `nombre-del-archivo.md`
- Sé descriptivo: `leccion-1-introduccion.md` en lugar de `leccion1.md`
- Para índices: `index.md`

### Carpetas
- Usa **kebab-case**: `nivel-basico/`, `modulo-conceptos/`
- Usa prefijos para orden: `01-fundamentos/`, `02-herramientas/`

### Imágenes
- Formato: `CURSO-MODULO-NOMBRE.png`
- Ejemplo: `javascript-funciones-flecha.png`
- Máximo ancho: 800px para mejor rendimiento

## 🔗 Estructura de URLs

Las URLs se generan automáticamente desde la estructura de carpetas:

```
docs/cursos/nivel-basico/fundamentos/leccion-1.md
→ https://delgadolearn.github.io/cursos/nivel-basico/fundamentos/leccion-1/
```

## 📋 Actualizar Menú de Navegación

Edita `mkdocs.yml` en la sección `nav` para agregar nuevos cursos:

```yaml
nav:
  - Inicio: index.md
  - Cursos:
    - Introducción: cursos/intro.md
    - Nivel Básico:
      - Inicio: cursos/nivel-basico/index.md
      - Fundamentos:
        - Leccion 1: cursos/nivel-basico/fundamentos/leccion-1.md
        - Leccion 2: cursos/nivel-basico/fundamentos/leccion-2.md
    - Nivel Intermedio:
      - Inicio: cursos/nivel-intermedio/index.md
  - Contribuir: contributing.md
  - Comunidad: comunidad.md
```

## 🎨 Elementos Reutilizables

### Admoniciones (Cajas destacadas)

```markdown
!!! note "Nota"
    Contenido importante pero no crítico

!!! warning "Advertencia"
    Algo que debes tener cuidado

!!! success "Éxito"
    Algo que funcionó bien

!!! danger "Peligro"
    Algo crítico o riesgoso

!!! info "Información"
    Información útil adicional
```

### Tabs (Pestañas)

```markdown
=== "Python"
    ```python
    print("Hola")
    ```

=== "JavaScript"
    ```javascript
    console.log("Hola")
    ```
```

### Código con Resaltado

```markdown
```python
def hola():
    print("Hola mundo")
```
```

## ✅ Checklist Para Nuevo Contenido

- [ ] Crear carpeta con nombre descriptivo
- [ ] Crear `index.md` en la carpeta
- [ ] Agregar contenido en lecciones
- [ ] Crear carpeta `ejercicios/` si hay ejercicios
- [ ] Guardar imágenes en `docs/assets/`
- [ ] Actualizar `mkdocs.yml` con la nueva estructura
- [ ] Probar localmente: `mkdocs serve`
- [ ] Hacer commit y push
