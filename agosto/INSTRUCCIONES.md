# 🖼️ CÓMO REEMPLAZAR IMÁGENES Y CONTENIDO

## 📁 **ESTRUCTURA DE CARPETAS**

```
projects-data/
├── park-mansion/
│   ├── config.json          ← Edita texto e información
│   └── images/              ← Coloca tus imágenes aquí
│       ├── 01-exterior.jpg  ← Reemplaza con tu imagen
│       ├── 03-lobby.jpg     
│       ├── 04-penthouse.jpg
│       └── ... (etc)
├── kawana/
│   ├── config.json          
│   └── images/
│       ├── 01-exterior.jpg
│       ├── 03-living.jpg
│       └── ... (etc)
```

## ✏️ **PARA CAMBIAR INFORMACIÓN DEL PROYECTO**

1. Abre `config.json` del proyecto
2. Edita estos campos:

```json
{
  "project": {
    "name": "NOMBRE DEL PROYECTO",
    "subtitle": {
      "es": "Subtítulo en español",
      "en": "Subtitle in English"
    },
    "description": {
      "es": "Descripción completa en español...",
      "en": "Complete description in English..."
    },
    "details": {
      "es": {
        "ubicación": "Ciudad, País",
        "año": "2024",
        "área": "350 m²",
        "tipo": "Residencial"
      },
      "en": {
        "location": "City, Country",
        "year": "2024", 
        "area": "350 m²",
        "type": "Residential"
      }
    }
  }
}
```

## 🖼️ **PARA CAMBIAR IMÁGENES**

1. **Ve a la carpeta**: `projects-data/[proyecto]/images/`
2. **Reemplaza archivos** con los nombres exactos:
   - `01-exterior.jpg`
   - `03-lobby.jpg` 
   - `04-penthouse.jpg`
   - etc.

3. **Formatos aceptados**: JPG, PNG
4. **Tamaño recomendado**: 1200x800px mínimo

## 🎥 **PARA CAMBIAR VIDEOS**

En `config.json`, edita la sección videos:

```json
"videos": [
  {
    "position": 2,
    "youtube_url": "https://www.youtube.com/embed/TU_VIDEO_ID",
    "caption": {
      "es": "Descripción en español",
      "en": "Description in English"
    }
  }
]
```

## ⚠️ **IMPORTANTE**

- **Nombres exactos**: Los archivos deben tener los nombres exactos del JSON
- **No tocar código**: Solo edita archivos en `projects-data/`
- **Backup**: Haz copia antes de cambios importantes
- **Testing**: Recarga la página para ver cambios

## 🔧 **URLS DE PROYECTOS**

- **Park Mansion**: `project-template.html?project=park-mansion`
- **Kawana**: `project-template.html?project=kawana`

## 💡 **TIPS**

1. Si una imagen no aparece, verifica el nombre del archivo
2. Para agregar más imágenes, añade entradas en el JSON
3. Videos de YouTube: usa formato embed (`/embed/VIDEO_ID`)
4. Para captions, siempre incluye español e inglés

---

**¡Ya puedes editar contenido sin tocar código!** 🎉
