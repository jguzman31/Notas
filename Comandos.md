## Visualizar Carpetas Creadas
```
# CMD
dir
```
## Crear una Carpeta
```
# CMD
mkdir "ruta\destino"
```

## Mover Carpeta
``
move origen destino
``
### Windows CMD
```
move "C:\Users\<username>\<folderName>" "D:\<folderName>"
```
### Windows PowerShell
```
Move-Item "C:\Users\<username>\<folderName>" "D:\<folderName>"
```
```
mv "C:\Users\<username>\<folderName>" "D:\<folderName>"
```
### Linux
```
sudo mv rutaOriente rutaDestino
sudo mv ~/folderName /var/www/
```

## Ocultar o visualizar un archivo o carpeta como administrador
``-S`` = Quitar atributo de Sistema

``-H`` = Quitar atributo de Oculto

``/S`` = Procesar subcarpetas

``/D`` = Procesar carpetas también

### Ocultar
```
# Desde CMD como Administrador
attrib +S +H "ruta\a\tu\archivo"
```
```
# Desde CMD como Administrador
attrib +S +H "C:\TuCarpeta"
```

### Visualizar
```
# Desde CMD como Administrador
attrib -S -H "ruta\a\tu\archivo"
```
```
# Desde CMD como Administrador
attrib -S -H "C:\TuCarpeta"
```
