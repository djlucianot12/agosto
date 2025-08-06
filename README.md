# 📁 GESTIÓN DE PROYECTOS - LT STUDIO DESIGN

Esta carpeta contiene toda la información de los proyectos organizadamente. Puedes modificar contenido sin tocar el código.

## 🗂️ ESTRUCTURA

```
projects-data/
├── park-mansion/
│   ├── config.json          ← Información del proyecto
│   └── images/              ← Coloca aquí las imágenes
│       ├── 01-exterior.jpg
│       ├── 03-lobby.jpg
│       └── ...
├── kawana/
│   ├── config.json          ← Información del proyecto  
│   └── images/              ← Coloca aquí las imágenes
│       ├── 01-exterior.jpg
│       ├── 03-living.jpg
│       └── ...
└── README.md               ← Este archivo
```

## ✏️ CÓMO EDITAR INFORMACIÓN

### 1. DATOS DEL PROYECTO
Edita el archivo `config.json` de cada proyecto:

```json
{
  "project": {
    "name": "NOMBRE DEL PROYECTO",
    "subtitle": "Subtítulo",
    "description": "Descripción completa del proyecto...",
    "details": {
      "location": "Ubicación",
      "year": "2024", 
      "area": "350 m²",
      "type": "Tipo de proyecto"
    }
  }
}
```

### 2. IMÁGENES
- Coloca las imágenes en la carpeta `images/` del proyecto
- Usa los nombres exactos del `config.json`:
  - `01-exterior.jpg`
  - `03-living.jpg` 
  - `04-kitchen.jpg`
  - etc.

### 3. VIDEOS
Edita la sección `videos` en `config.json`:

```json
"videos": [
  {
    "position": 2,                    ← Posición en la galería
    "youtube_url": "https://www.youtube.com/embed/TU_VIDEO_ID",
    "poster": "url_imagen_preview",
    "caption": "Descripción del video"
  }
]
```

## 🖼️ FORMATOS RECOMENDADOS

### Imágenes:
- **Formato**: JPG o PNG
- **Resolución**: 1200x800px mínimo
- **Peso**: Máximo 2MB cada una

### Videos:
- **Plataforma**: YouTube
- **URL**: Usar formato embed: `https://www.youtube.com/embed/VIDEO_ID`

## 📋 LISTA DE ARCHIVOS REQUERIDOS

### Park Mansion:
- `01-exterior.jpg` - Fachada urbana
- `03-lobby.jpg` - Lobby con instalaciones artísticas  
- `04-penthouse.jpg` - Suite penthouse
- `05-terrace.jpg` - Terrazas jardín privadas
- `06-pool.jpg` - Piscina infinita
- `08-kitchen.jpg` - Cocina premium
- `09-gym.jpg` - Centro fitness
- `10-night.jpg` - Iluminación nocturna
- `11-details.jpg` - Detalles arquitectónicos
- `12-community.jpg` - Espacios comunitarios

### Kawana:
- `01-exterior.jpg` - Fachada exterior
- `03-living.jpg` - Área de estar abierta
- `04-kitchen.jpg` - Diseño de cocina minimalista
- `05-bedroom.jpg` - Dormitorio principal
- `06-bathroom.jpg` - Baño tipo spa
- `08-garden.jpg` - Patio jardín japonés
- `09-terrace.jpg` - Terraza elevada
- `10-night.jpg` - Iluminación nocturna
- `11-detail.jpg` - Detalle arquitectónico
- `12-aerial.jpg` - Vista aérea

## ⚠️ IMPORTANTE

1. **Nombres exactos**: Usa los nombres de archivo exactos del `config.json`
2. **No tocar código**: Todo se actualiza automáticamente
3. **Backup**: Haz copia de seguridad antes de cambios importantes
4. **Testing**: Verifica que las imágenes se vean correctamente

## 🔄 AGREGAR NUEVO PROYECTO

1. Crear carpeta: `nuevo-proyecto/`
2. Agregar: `config.json` con la misma estructura
3. Crear: carpeta `images/`
4. Actualizar código para incluir el nuevo proyecto

---

💡 **Tip**: Si una imagen no aparece, verifica que el nombre del archivo coincida exactamente con el `config.json`
