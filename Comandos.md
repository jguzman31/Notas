# Comandos por consola
`Visualizar carpetas creadas`
```
dir
```
```
ls
```

`Crear una carpeta`
```
mkdir "ruta\destino"
```
```
mkdir carpeta1 carpeta2
```

`Eliminar una carpeta`
```
sudo rm -rf folderName
```
`Eliminar un archivo`
```
sudo rm fileName
```

`Mover carpeta`

Windows CMD
```
move origen destino
```
```
move "C:\Users\<username>\<folderName>" "D:\<folderName>"
```

Windows PowerShell
```
Move-Item "C:\Users\<username>\<folderName>" "D:\<folderName>"
```
```
mv "C:\Users\<username>\<folderName>" "D:\<folderName>"
```

Linux
```
scp -r "rutaOrigen" username@ipaddress:/rutaDestino
```
```
scp -r "./esculapio" super@192.168.12.61:/var/www/
```
```
sudo mv rutaOriente rutaDestino
```
```
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
