#Treemap

Plantilla de visualización tipo Treemap.<br>
Descripción de archivos principales:

- `treemap.html` <br>- Archivo html en el que se importan principalmente:
  * Librería de la visualización
  * Archivo `js` con diversas funcionalidades (`js/treemap.js`)
  * **Contendor para la gráfica**, que en este caso se debe definir en el html como: `<div id="treemapd3"></div>`<br><br>
  
  
- `partials/treemap_example.json`<br>- **Json base** para definir los valores que mostrará la visualización, se debe respetar la **estructura** y los **nombres** o `keys` de los valores.<br><br>

- `js/treemap.js`<br>- Javascript que contiene las funcionalidades **necesarias** para dibujar la visualización.
