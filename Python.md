## Entorno virtual
``` Code
# instalar virtualenv modo global
pip install virtualenv
```

``` Code
# crear entorno virtual
virtualenv -p python3 env
```

``` Code
# activar entorno virtual
.\env\Scripts\activate
```

``` Code
# desactivar entorno virtual
deactivate
```

``` Code
# visualizar las librerias instaladas en el entorno virtual
pip list
```

``` Code
# actualizar pip
python.exe -m pip install --upgrade pip
```

``` Code
# ejecutar py (es necesario estar dentro del entorno)
python .\src\app.py
```

``` Code
# exportar los paquetes instalados en el proyecto
pip freeze > requirements.txt
```

``` Code
# importar los paquetes del proyecto
pip install -r .\requirements.txt
```


## Librerias
``` Code
# instalar flask
pip install flask
```

``` Code
# instalar dotenv
pip install python-dotenv
```

``` Code
# instalar requests
pip install requests
```

``` Code
# instalar selenium scrapper
pip install selenium
```

``` Code
# instalar conexión con PostgreSQL
pip install psycopg2
```

``` Code
# instalar conexión con PostgreSQL otras dependencias
pip install psycopg2-binary
```

``` Code
# instalar conexión con MySQL
pip install mysql-connector-python
```

``` Code
# instalar pymysql
pip install pymysql
```

``` Code
# instalar Django
py -m pip install Django==#version
# revisar la pagina oficial de Django "https://www.djangoproject.com/download/"
```
