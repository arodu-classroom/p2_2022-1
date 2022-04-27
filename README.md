# Clase 2022-04-27

- Instalar nodejs
	- https://nodejs.org/en/download/
	- https://snapcraft.io/node
	
- Instalar express
	- express-generator
	- https://expressjs.com/en/starter/generator.html
		
```bash
npx express-generator --view=ejs p2_clase
cd p2_clase
npm install
npm start
```
		
- http://localhost:3000/
	
- Instalar git
	- https://www.hostinger.es/tutoriales/instalar-git-en-distintos-sistemas-operativos

- Crear repositorio en github
	- new repository

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:arodu/p2_clase_2022-1.git
git push -u origin main
```

- Conexion a heroku
	- crear app 
	- agregar buildpack nodejs
		
- Instalacion de heroku-cli
	- https://devcenter.heroku.com/articles/heroku-cli
	
```bash
heroku login
heroku git:remote -a p2-clase-20221
git push heroku main
```

- https://p2-clase-20221.herokuapp.com/




