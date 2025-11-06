Clonar repositorio HTTPS
```
git clone https://github.com/<username>/<repository_name>.git
```

Clonar repositorio SSH
```
git clone git@github.com:<username>/<repository_name>.git
```
`Tener en cuenta los pasos de la configuración .SSH`

Subir repositorio
```
git init
```
```
git remote add origin https://github.com/<username>/<repository_name>.git
```
```
git add .
```
```
git add .gitignore
```
```
git commit -m ""
```
```
git push -u origin main # Primera vez
```
```
git push # Envíos posteriores
```
```
git pull origin main
```

Eliminar carpeta completa
```
git rm -r --cached carpeta_que_ya_esta_subida/
```
`luego realizar los pasos "Subir repositorio"`

Eliminar archivo especifico
```
git rm --cached .env
```
`luego realizar los pasos "Subir repositorio"`
