# hab-m03. Javascript ES6 - I

(_ES6 = EcmaScript 6_)

This project _(Module 03)_ holds the coding exercises 🧑‍💻 planed by teachers 🧑‍🏫 about topic _Javascript I_ during my [Hack A Boss bootcamp](https://hackaboss.dev/bootcamp-programacion-remoto).

Also some usefull notes taken during that remote classes happens.

We are hackers 🧑‍🎓🧑‍💻🧞, we are bossers 🕴️, we are remoters 🌐⛓️.


## Requirements

**Git**. https://git-scm.com

```bash
sudo apt-get install git
```

**NodeJS 12.x**. https://nodejs.org

1. se puede instalar globalmente mediante:
```bash
sudo apt-get install nodejs
```
2. o a través de sus paquetes de NodeSource:
  https://github.com/nodesource/distributions
```bash
# Instalamos el software previo
sudo apt-get install curl

# Descargamos el paquete, cargandolo en la sesion bash
sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -

# y lo instalamos tomando la caché bash como fuente
sudo apt-get install -y nodejs
```
3. también mediante su gestor de versiones **nvm** el cual nos permite una mayor flexibilidad.
  https://github.com/nvm-sh/nvm
  - Tener varias versiones instaladas a la vez e ir cambiando entre ellas según requisitos.
  - Es útil sobre todo si andamos desarrollando varios proyectos con código legacy.
  - No necesitar permisos de superusuario (root), porque su estructura de ficheros se guarda en nuestro `$HOME`.


**Visual Studio Code**. https://code.visualstudio.com/

1. se puede instalar desde la [tienda de Snaps](https://snapcraft.io/code) de Ubuntu
2. como paquete Snap desde la terminal:
```bash
sudo snap install --classic code
```
3. como paquete `.deb` utilizando `apt`:
```bash
# Instalamos el software previo
sudo apt-get update
sudo apt-get install software-properties-common apt-transport-https wget

# Descargamos e instalamos los certificados con los que estan firmados los paquetes de Microsoft
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

# Agregamos el repositorio
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

# Lanzamos la instalación
sudo apt install code
```


## Initialization

Por la terminal ejecutamos en orden los siguientes comandos:

```bash
# Creamos la carpeta del módulo y nos metemos en ella
mkdir hab-mod03
cd hab-mod03

# Inicializamos su repositorio
git init

# Agregamos contenido
echo "# MODULE 03 - Javascript ES6" >> README.md
echo "" >> .gitignore

## Agregamos al repositorio
git add --all
git commit -m "🎉 Commit inicial. MODULE 03 - Javascript ES6"

# Arrancamos Visual Studio Code la carpeta actual
code .
```


## Extensiones para VS Code

Es util instalar:

- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig): Permite a traves de un fichero `.editorconfig` dar unas reglas de formateo básico a nuestros ficheros mediante unas reglas básicas: espacios en blanco, tamaño y tipo de indentado...
- [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2): Ayuda visualmente al desarrollador con un mejor resaltado, entre otras cosas, de sintaxis en cuanto a parentesis, llaves y corchetes.


## How to contribute

For information ℹ️ on adding any content, please see first the [CONTRIBUTING file](CONTRIBUTING.md).


## License

The content of this project itself and the underlying source code used to format and display that content is licensed under the [The GNU Affero General Public License Version 3](LICENSE).
