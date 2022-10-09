# Parcel - Bootstrap/SASS - Base

🔧 Comando para instalar las dependencias 

```
npm install
```
🔧 Comando para iniciar el servidor de desarrollo
```
npm run dev
```
🔧 Comando para crear la build
```
npm run build
```

## ❗ NOTAS IMPORTANTES:

💡 Una vez se termine de trabajar en el servidor de desarrollo se debera de borrar manualmente la carpeta 📂/dist y ejecutar el comando `npm run build` ya que por defecto Parcel deja los archivos de desarrollo en la carpeta y se mantienen ambos. (O en los scripts añadir --dist-dir ./carpeta) Esto sirve para tener una carpeta 📂/dist y otra 📂/docs por ejemplo.

💡 Si se va a trabajar en un sitio estatico no es necesario tener el `<script>` en el index.html ni la carpeta 📂assets/js.

💡 Si se trabajara en una app es necesario tener el `<script>` en el index, la importación de Bootstrap en main.js y instalar popper mediante el comando.
```
npm i --save bootstrap @popperjs/core
```
No es necesario importar popper en main.js ya que se importa junto a Bootstrap.

💡 Las variables de Bootstrap se pueden modificar en el archivo _variables.scss y se pueden añadir mas en styles.scss. Para mas información ver [Bootstrap-DOCS](https://getbootstrap.com/docs/5.2/customize/sass/).

💡 Para modificar el formato de salida de las imagenes en producción (png a webp) es necesario usar query parameters, para mas info [Parcel-DOCS](https://parceljs.org/recipes/image/).