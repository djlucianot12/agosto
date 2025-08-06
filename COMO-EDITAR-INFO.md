# 📝 CÓMO EDITAR LA INFORMACIÓN DEL PROYECTO

## 🎯 **QUÉ PUEDES CAMBIAR EN CONFIG.JSON**

### 1. **INFORMACIÓN BÁSICA DEL PROYECTO**
```json
"name": "PARK MANSION",           ← NOMBRE DEL PROYECTO (no cambies)
"subtitle": {
  "es": "Elegancia Urbana",       ← CAMBIA ESTO: Subtítulo en español
  "en": "Urban Elegance"          ← CAMBIA ESTO: Subtítulo en inglés
}
```

### 2. **DESCRIPCIÓN COMPLETA**
```json
"description": {
  "es": "Descripción completa en español...",  ← CAMBIA ESTO
  "en": "Complete description in English..."   ← CAMBIA ESTO
}
```

### 3. **DETALLES TÉCNICOS**
```json
"details": {
  "es": {
    "ubicación": "Tokyo Central Park",  ← CAMBIA: Donde está ubicado
    "año": "2024",                     ← CAMBIA: Año del proyecto
    "área": "1,250 m²",                ← CAMBIA: Tamaño del proyecto
    "tipo": "Residencial de Lujo"      ← CAMBIA: Tipo de proyecto
  },
  "en": {
    "location": "Tokyo Central Park",   ← CAMBIA: Same in English
    "year": "2024",                    ← CAMBIA: Same in English
    "area": "1,250 m²",                ← CAMBIA: Same in English
    "type": "Luxury Residential"       ← CAMBIA: Same in English
  }
}
```

### 4. **DESCRIPCIONES DE IMÁGENES**
```json
"images": [
  {
    "filename": "01.jpg",              ← NO CAMBIES: Nombre del archivo
    "caption": {
      "es": "Descripción en español",  ← CAMBIA ESTO
      "en": "Description in English"   ← CAMBIA ESTO
    }
  }
]
```

### 5. **LINKS DE VIDEOS DE YOUTUBE**
```json
"videos": [
  {
    "position": 3,                                    ← NO CAMBIES: Posición
    "youtube_url": "PEGA_AQUI_TU_LINK_DE_YOUTUBE",   ← CAMBIA ESTO
    "caption": {
      "es": "Descripción del video",                  ← CAMBIA ESTO
      "en": "Video description"                       ← CAMBIA ESTO
    }
  }
]
```

## 🎥 **CÓMO AGREGAR VIDEOS DE YOUTUBE**

1. **Ve a tu video en YouTube**
2. **Copia el ID del video** (ejemplo: si el link es `https://youtube.com/watch?v=ABC123`, el ID es `ABC123`)
3. **Reemplaza** `PEGA_AQUI_TU_LINK_DE_YOUTUBE` con: `https://www.youtube.com/embed/ABC123`

**Ejemplo:**
```json
"youtube_url": "https://www.youtube.com/embed/dQw4w9WgXcQ"
```

## ⚠️ **QUÉ NO TOCAR**

❌ **NO cambies:**
- `"filename"`: Nombres de archivos de imagen
- `"position"`: Posición de videos
- `"main_image"`: Siempre debe ser "main.jpg"
- Las llaves `{}` y corchetes `[]`
- Las comillas `""`

## 📁 **ESTRUCTURA DE ARCHIVOS**

```
tu-proyecto/
├── config.json          ← Edita AQUÍ la información
└── images/
    ├── main.jpg         ← Imagen del círculo de inicio
    ├── 01.jpg           ← Imagen 1 de la galería
    ├── 02.jpg           ← Imagen 2 de la galería
    └── ... (hasta 11.jpg)
```

## 💡 **CONSEJOS**

- ✅ **Guarda una copia** antes de editar
- ✅ **Usa comillas dobles** siempre: `"texto"`
- ✅ **Incluye español E inglés** en todo
- ✅ **Mantén las comas** al final de las líneas
- ✅ **No borres las llaves** `{}`

## 🚨 **SI ALGO SE ROMPE**

1. Verifica que todas las comillas estén cerradas
2. Verifica que todas las llaves `{}` estén cerradas
3. Verifica que no falten comas `,`
4. Restaura desde el backup si es necesario

---

**¡Ahora puedes editar toda la información sin tocar código!** 📝✨
