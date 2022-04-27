# Clase 2022-04-27

## Aplicación express-nodejs en local

- Instalación nodejs
  - https://nodejs.org/en/download/
  - https://snapcraft.io/node para ubuntu y derivados
- Instalación express
  - express-generator
  - https://expressjs.com/en/starter/generator.html

```bash
npx express-generator --view=ejs p2_clase
cd p2_clase
npm install
npm start
```

Creación del proyecto p2_clase, instalación de paquetes y levantamiento del servidor, funcionamiento en http://localhost:3000/

## Subir proyecto a [GitHub](https://github.com/)

- Instalar git
    - https://www.hostinger.es/tutoriales/    instalar-git-en-distintos-sistemas-operativos
    - usar git-bash para windows

- Crear repositorio en github, https://github.com
    - `boton "+" > new repository`
    - conectar repositorio local con remoto
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:arodu/p2_clase_2022-1.git
git push -u origin main
```

Podemos verificar que se ha conectado con el comando `git remote -v`

## Subir proyecto a [Heroku](https://heroku.com/)

- Conexion a heroku
    - Hacer login en heroku a traves de la web
    - Crear una nueva aplicación (heroku en su versión gratuita solo dejar crear hasta 5 aplicaciones)
        - `Botón "New" > Create new app`
    - Agregar buildpack para nodejs
        - `Pestaña "Settings" > Botón "Add buildpack" > Selecionar Nodejs > Botón "Save changes"`
    - Instalacion de heroku-cli
        - https://devcenter.heroku.com/articles/heroku-cli
    - Luego de instalado hacer login desde la consola y conectar el repositorio local, al repositorio de heroku

```bash
heroku login
heroku git:remote -a p2-clase-20221
git push heroku main
```

Podemos verificar que se ha conectado con el comando `git remote -v`

Aplicación corriendo en linea https://p2-clase-20221.herokuapp.com/

## Resumen
1. Se creo un proyecto de express-nodejs el local llamado `p2_clase`
2. Se creo un repositorio en la cuenta de github del profesor llamado `arodu/p2_clase_2022`
    - https://github.com/arodu/p2_clase_2022-1
3. Se creo una aplicación en heroku llamada `p2-clase-20221`
    - https://p2-clase-20221.herokuapp.com/

## Recursos extras

- https://platzi.com/tutoriales/2042-prework-windows/8975-dale-estilo-grafico-a-windows-terminal/
- https://platzi.com/tutoriales/2042-prework-windows/8976-anade-git-bash-a-windows-terminal/
