# MOD 03 - DÍA 02


## Inicializamos proyecto

Por la terminal ejecutamos en orden los siguientes comandos:

```bash
# Creamos carpeta de proyecto del día y nos metemos en ella
mkdir dia-02 && cd dia-02

# Agregamos contenido
echo "# MOD 03 - DÍA 02" >> README.md

## Agregamos al repositorio
git add --all
git commit -m "🎉 Commit inicial. MOD 03 - Día 02"

# Inicializamos el proyecto NodeJS
npm init

# Instalamos como dependencia de desarollo la librería
# que permite ejecutar en el navegador código en caliente
npm install -D browser-sync

# Excluímos node_modules generado por NodeJS
echo "node_modules" >> .gitignore

## Agregamos al repositorio
git add --all
git commit -m "📝 Init proyecto. MOD 03 - Día 02"

# Arrancamos Visual Studio Code en esa carpeta
code .
```

Editamos el `package.json` para declarar en la sección `scripts` la ejecución `start` que nos permitirá levantar un servidor en caliente:

```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "browser-sync start --server './' --files './'"
}
```

Y creamos sendos archivos `index.html` y `src/index.js` desde consola:

```bash
touch index.html
mkdir src
touch src/index.js
```

Snippet mínimo para el `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MOD03 - Día 02</title>
</head>
<body>
    <h1>Día 02</h1>
    <script type="module" src="src/index.js"></script>
</body>
</html>
```

Snippet mínimo para el `src/index.js`:

```javascript
'use strict';

console.log("Hello World!");
```

## Puesta en ejecución

Arrancamos el servidor en caliente con:

```bash
# Lanzamos la tarea que definimos anteriormente en el package.json
npm start
```

y se nos debería abrir nuestro navegador de internet. Si abrimos las devtools deberíamos ver el siguiente mensaje en la consola:

```
"Hello World!"
```

Para parar el servidor... `CTRL+C`.


## VS Code extensions

Es útil instalar:

- [ESLint](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner): Nos permite que nuestro código pase un analizador de sintaxis en segundo plano a partir de unas reglas _(indentación, formateado...)_ que definamos flexiblemente mediante ficheros de configuración `[package.json, eslintrc, .eslintignore]` bajo la estructura de nuestro proyecto.

- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner): Nos permite ejecutar de forma simple mediante un comando o un click cualquier trozo de código (snippet) o fichero en una gran variedad de lenguajes, entre ellos Javascript.


## How to contribute

For information ℹ️ on adding any content, please see first the [CONTRIBUTING file](../CONTRIBUTING.md).


## License

The content of this project itself and the underlying source code used to format and display that content is licensed under the [The GNU Affero General Public License Version 3](../LICENSE).
