# INSTRUCCIONES: CÓMO MIGRAR TODOS LOS ARCHIVOS

## Archivos a descargar desde SAM-v3.0-AI-Teacher

### 1. Archivos HTML (Versiones del Sitio)
```
SAM-v3.0-AI-Teacher/gl-strategic/
├── index.html (versión final)
├── index_v6.html (versión de referencia estética)
├─┐ index_v7.html (versión actual funcional)
```

### 2. CSS
```
SAM-v3.0-AI-Teacher/gl-strategic/
├── styles.css (estilos principales)
```

### 3. Carpeta Assets
```
SAM-v3.0-AI-Teacher/gl-strategic/assets/
├── images/team/ (25 fotos del equipo)
└── videos/ (5 videos de fondo)
```

### 4. Documentación
```
Google Drive > GL Strategic > Maqueta-version-08.docx
(FUENTE DE VERDAD principal)
```

### 5. README del Proyecto Original
```
SAM-v3.0-AI-Teacher/gl-strategic/README.md
```

## Pasos para Migrar

### Opción 1: Usando Git CLI (Recomendado)

```bash
# Clonar el repo nuevo
git clone https://github.com/CarlosVergaraChile/GL-Strategic-Web-Site.git
cd GL-Strategic-Web-Site

# Copiar archivos desde SAM-v3.0-AI-Teacher/gl-strategic
cp -r ../SAM-v3.0-AI-Teacher/gl-strategic/* .

# Agregar y commit
git add .
git commit -m "feat: Add all GL Strategic website files from SAM project"
git push origin main
```

### Opción 2: Usando GitHub Web UI

1. Ir a: https://github.com/CarlosVergaraChile/GL-Strategic-Web-Site
2. Click en "Add file" > "Upload files"
3. Seleccionar archivos del directorio `gl-strategic/` de SAM-v3.0-AI-Teacher
4. Subir por lotes (HTML primero, luego assets)
5. Commit cambios

## Estructura Final Esperada

```
GL-Strategic-Web-Site/
├── README.md (CREADO)
├── .gitignore (CREADO)
├── index.html (POR AGREGAR)
├── index_v6.html (POR AGREGAR)
├─┐ index_v7.html (POR AGREGAR)
├── styles.css (POR AGREGAR)
├── assets/ (POR AGREGAR)
│   ├── images/
│   │   ├── team/ (25 fotos)
│   │   └── logo.png
│   └── videos/ (5 videos)
├── docs/ (POR AGREGAR)
│   ├── Maqueta-version-08.docx
│   └── README-GL-Strategic.md
```

## Archivos Clave

- **README.md** - Documentación del proyecto
- **index.html** - Sitio principal
- **index_v6.html** - Referencia de diseño
- **styles.css** - Estilos CSS
- **assets/images/team/** - 25 fotos del equipo
- **assets/videos/** - 5 videos de fondo
- **Maqueta-version-08.docx** - Fuente de verdad

## Status de Migración

- ✅ README.md
- ✅ .gitignore
- ⚠️ HTML files (index.html, v6, v7)
- ⚠️ CSS files
- ⚠️ Assets (images, videos)
- ⚠️ Documentation

## Notas

- Las 25 fotos del equipo ya están en: `SAM-v3.0-AI-Teacher/gl-strategic/assets/images/team/`
- La maqueta Word (v08) es la fuente de verdad para contenidos
- Mantener la estructura de carpetas exactamente como se especifica
