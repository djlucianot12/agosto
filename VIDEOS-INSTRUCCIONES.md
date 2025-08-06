# 📹 DÓNDE PONER LOS LINKS DE VIDEOS

## ❌ NO van en la carpeta de imágenes

Los videos **NO** se ponen en la carpeta `images/`. Esta carpeta es solo para archivos de imagen (JPG, PNG, etc.).

## ✅ Los videos van en config.json

Los links de YouTube se configuran en el archivo `config.json` de cada proyecto:

### Ubicación del archivo:
```
projects-data/[NOMBRE-DEL-PROYECTO]/config.json
```

### Sección de videos en config.json:
```json
"videos": [
  {
    "position": 3,
    "youtube_url": "PEGA_AQUI_TU_LINK_DE_YOUTUBE",
    "caption": {
      "es": "Descripción del video en español",
      "en": "Video description in English"
    }
  },
  {
    "position": 7,
    "youtube_url": "PEGA_AQUI_TU_SEGUNDO_LINK_DE_YOUTUBE",
    "caption": {
      "es": "Segundo video en español", 
      "en": "Second video in English"
    }
  }
]
```

## 📝 Cómo agregar tus videos:

### Paso 1: Obtener el link de YouTube
- Ve a tu video en YouTube
- Copia la URL completa (ejemplo: `https://www.youtube.com/watch?v=dQw4w9WgXcQ`)

### Paso 2: Reemplazar en config.json
- Abre el archivo `config.json` del proyecto
- Busca la sección `"videos"`
- Reemplaza `"PEGA_AQUI_TU_LINK_DE_YOUTUBE"` con tu link real

### Paso 3: Configurar posición
- `"position": 3` significa que el video aparecerá después de la imagen 3
- `"position": 7` significa que el video aparecerá después de la imagen 7
- Puedes cambiar estos números según donde quieras que aparezcan

### Ejemplo completo:
```json
"videos": [
  {
    "position": 3,
    "youtube_url": "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
    "caption": {
      "es": "Recorrido virtual de Park Mansion",
      "en": "Virtual tour of Park Mansion"
    }
  }
]
```

## 🎯 Resumen rápido:
1. **Videos = config.json** (no en carpeta images)
2. **Imágenes = carpeta images/** (archivos JPG/PNG)
3. **Reemplaza** `PEGA_AQUI_TU_LINK_DE_YOUTUBE` con tu link real
4. **Configura** la posición donde quieres que aparezca el video

---

**¿Necesitas ayuda?** Revisa el archivo `COMO-EDITAR-INFORMACION.md` para más detalles.
