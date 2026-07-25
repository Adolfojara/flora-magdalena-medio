# Flora del Magdalena Medio — Géneros de Plantas Vasculares

Catálogo web interactivo de los géneros de plantas vasculares registrados en el Magdalena Medio (Colombia).

## ¿Qué contiene?

- **1.286 géneros** en **233 familias**
- Búsqueda por nombre de género o familia
- Filtro por familia
- Vista en fichas o tabla
- Ficha por género con: descripción, distribución, diversidad global y regional, links a GBIF / Tropicos / Plants of the World Online / iNaturalist
- **Editor integrado**: cualquier usuario puede agregar información en su navegador (los datos se guardan localmente)

## 🚀 Publicar en GitHub Pages (paso a paso)

### 1. Crea un repositorio en GitHub
- Ve a [github.com/new](https://github.com/new)
- Nombre sugerido: `flora-magdalena-medio`
- Dejarlo **Public**
- Haz clic en **Create repository**

### 2. Sube los archivos
Tienes dos opciones:

**Opción A — desde la web (más fácil):**
1. En tu repositorio, haz clic en **Add file > Upload files**
2. Arrastra `index.html` y `data.json`
3. Haz clic en **Commit changes**

**Opción B — desde la terminal (si tienes Git):**
```bash
git init
git add index.html data.json README.md
git commit -m "Publicación inicial: géneros Magdalena Medio"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/flora-magdalena-medio.git
git push -u origin main
```

### 3. Activa GitHub Pages
1. Ve a **Settings > Pages**
2. En **Source**, selecciona **Deploy from a branch**
3. Branch: `main` / Folder: `/ (root)`
4. Haz clic en **Save**
5. En unos minutos el sitio estará en: `https://TU_USUARIO.github.io/flora-magdalena-medio/`

## 📝 Agregar información a los géneros

### Opción 1: Directamente en la web
- Abre cualquier ficha y usa el formulario al final para agregar texto
- Los datos se guardan en el navegador del usuario (localStorage)
- **Ideal para consulta personal o demostraciones**

### Opción 2: Editar data.json (recomendado para datos definitivos)
Cada género tiene esta estructura en `data.json`:

```json
{
  "genus": "Inga",
  "family": "Fabaceae",
  "description": "Árboles o arbustos con hojas paripinnadas...",
  "distribution_mm": "Común en bosques riparios y selvas...",
  "global_diversity": "~350 spp. en trópicos americanos",
  "regional_diversity": "~30 spp. registradas en el Magdalena Medio",
  "notes": "Importante en sucesión ecológica; frutos comestibles.",
  "image_url": "https://inaturalist-open-data.s3.amazonaws.com/photos/...",
  "gbif_url": "https://www.gbif.org/species/search?q=Inga&rank=GENUS",
  "tropicos_url": "https://www.tropicos.org/Name/Search?name=Inga",
  "powo_url": "https://powo.science.kew.org/taxon/urn:lsid:ipni.org:names:Inga"
}
```

Edita el archivo, guarda y sube los cambios a GitHub. El sitio se actualiza automáticamente.

## 🔗 Fuentes de imágenes recomendadas
- **iNaturalist**: `https://www.inaturalist.org/taxa?q=GENERO`
- **GBIF**: `https://www.gbif.org/species/search?q=GENERO&rank=GENUS`
- **Wikimedia Commons**: `https://commons.wikimedia.org`

## Créditos
Datos basados en colecciones de herbarios colombianos depositadas en el Sistema de Información sobre Biodiversidad de Colombia (SiB).
