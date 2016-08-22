#Treemap

Plantilla de visualización tipo Treemap.<br>
Descripción de archivos principales:

- `treemap.html` <br>- Archivo html en el que se importan principalmente:
  * Librería de la visualización
  * Archivo `js` con diversas funcionalidades (`js/treemap.js`)
  * **Contendor para la gráfica**, que en este caso se debe definir en el html como: `<div id="treemapd3"></div>`<br><br>
  
  
- `partials/treemap_example.json`<br>- **Json base** para definir los valores que mostrará la visualización.<br><br>

- `js/treemap.js`<br>- Javascript que contiene las funcionalidades **necesarias** para dibujar la visualización.

##Json base

El Json que consumirá la visualización debe estar en todo momento dentro del folder `partials` y debe tener asignado el nombre `treemap_example.json`<br>

La **estructura** debe ser igual a la del archivo `treemap_example.json`, si exisite alguna diferencia, por mínima que sea, la gráfica no se visualizará en el navegador.

Además los **nombres** o `keys` de los valores deben ser iguales a los dej Json de ejemplo para que estos se puedan mostrar en la visualización.

**Estructura**


{
	"unidad": "Personas",
	"valores": [
		{
			"nivel1": "Manufactura y construcción",
			"nivel2": "Apoyo a la juventud",
			"nivel3": "Servicios personales",
			"nivel4": "Prima quinquenal por años de servicios efectivos presta dos.",
			"valor": 55000
		}
	]
}

- "unidad" //Se muestra como texto dentro del popup de cada área del treemap
- "valores" //Son los valores en que se agrupa el Treemap, si se quieren tener más o menos niveles de profundidad, estos se deben especificar en el archivo `js/treemap.js` en la variable `idVal`
- "valor" //Asigna valor y porcentaje a cada elemento del Treemap
