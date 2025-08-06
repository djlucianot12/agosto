# CÓMO EDITAR LA INFORMACIÓN DE LOS PROYECTOS

## ¿Qué archivo modificar?

Para cambiar la información de cualquier proyecto, debes editar el archivo `config.json` que está dentro de la carpeta del proyecto.

**Ruta del archivo:**
```
projects-data/[NOMBRE-DEL-PROYECTO]/config.json
```

## Estructura del archivo config.json

### 1. INFORMACIÓN BÁSICA DEL PROYECTO

```json
"project": {
  "name": "PARK MANSION",
  "subtitle": {
    "es": "Elegancia Urbana",
    "en": "Urban Elegance"  
  },
  "description": {
    "es": "Tu descripción en español aquí...",
    "en": "Your description in English here..."
  }
}
```

**¿Qué puedes cambiar?**
- `name`: El nombre del proyecto (aparece grande en la página)
- `subtitle.es`: Subtítulo en español 
- `subtitle.en`: Subtítulo en inglés
- `description.es`: Descripción completa en español
- `description.en`: Descripción completa en inglés

### 2. DETALLES DEL PROYECTO

```json
"details": {
  "es": {
    "ubicación": "Tokyo Central Park",
    "año": "2024", 
    "área": "1,250 m²",
    "tipo": "Residencial de Lujo"
  },
  "en": {
    "location": "Tokyo Central Park",
    "year": "2024",
    "area": "1,250 m²", 
    "type": "Luxury Residential"
  }
}
```

**¿Qué puedes cambiar?**
- Todos los valores (ubicación/location, año/year, área/area, tipo/type)
- Puedes agregar nuevos campos siguiendo el mismo patrón

### 3. IMÁGENES

```json
"media": {
  "main_image": "main.jpg",
  "images": [
    {
      "filename": "01.jpg",
      "caption": {
        "es": "Tu descripción en español",
        "en": "Your description in English"
      }
    }
  ]
}
```

**¿Qué puedes cambiar?**
- `main_image`: Siempre debe ser "main.jpg" (esta es la imagen del círculo)
- Para cada imagen (01.jpg a 11.jpg):
  - `filename`: El nombre del archivo (NO cambiar)
  - `caption.es`: Descripción de la imagen en español
  - `caption.en`: Descripción de la imagen en inglés

### 4. VIDEOS DE YOUTUBE

```json
"videos": [
  {
    "position": 3,
    "youtube_url": "PEGA_AQUI_TU_LINK_DE_YOUTUBE",
    "caption": {
      "es": "Recorrido virtual del desarrollo", 
      "en": "Virtual tour of the development"
    }
  }
]
```

**¿Cómo agregar videos?**
1. Reemplaza `"PEGA_AQUI_TU_LINK_DE_YOUTUBE"` con tu enlace real de YouTube
2. Cambia `position`: en qué número de imagen quieres que aparezca el video
3. Modifica las descripciones en español e inglés

**Ejemplo de enlace válido:**
```json
"youtube_url": "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
```

## ¿Cómo reemplazar las imágenes?

### Paso 1: Ubicar la carpeta de imágenes
```
projects-data/[NOMBRE-DEL-PROYECTO]/images/
```

### Paso 2: Reemplazar archivos
- `main.jpg` → Imagen principal (aparece en el círculo del inicio)
- `01.jpg` a `12.jpg` → Imágenes de la galería (12 imágenes total)

**IMPORTANTE:** 
- Mantén exactamente los mismos nombres de archivo
- Formatos recomendados: JPG, PNG
- Resolución recomendada: mínimo 1920x1080px

## Ejemplo práctico: Editando Park Mansion

### Antes:
```json
"subtitle": {
  "es": "Elegancia Urbana",
  "en": "Urban Elegance"
}
```

### Después (tu cambio):
```json
"subtitle": {
  "es": "Nuevo Subt��tulo Aquí",
  "en": "New Subtitle Here" 
}
```

## ⚠️ IMPORTANTES REGLAS DE SINTAXIS

1. **Siempre usar comillas dobles**: `"texto"` ✅ NO `'texto'` ❌
2. **No olvidar las comas**: Cada línea termina en coma, excepto la última
3. **Mantener la estructura**: No eliminar llaves `{}` o corchetes `[]`
4. **Respetar la indentación**: Los espacios son importantes para legibilidad

## Verificar que funciona

Después de hacer cambios:
1. Guarda el archivo config.json
2. Actualiza la página web (F5 o Ctrl+R)
3. El proyecto debería mostrar los nuevos datos

## Proyectos disponibles para editar

- `park-mansion` - Park Mansion
- `kawana` - Kawana Project  
- `azabu-gardens` - Azabu Gardens
- `brillia-hongo` - Brillia Hongo
- `century-forest` - Century Forest
- `minamiaoyama-house` - Minamiaoyama House
- `nishiazabu-residence` - Nishiazabu Residence  
- `proud-rokakoen` - Proud Rokakoen

## 🆘 Si algo sale mal

1. Verifica que no falten comas o comillas
2. Usa un validador JSON online para verificar sintaxis
3. Restaura desde una copia de seguridad si es necesario
4. Los nombres de archivos de imagen NUNCA deben cambiar

---

**¿Necesitas ayuda?** Revisa este archivo cada vez que vayas a hacer cambios.
