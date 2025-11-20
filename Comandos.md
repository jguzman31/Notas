# Comandos por consola
### Visualizar carpetas creadas
```
dir
```
```
ls
```

### Crear una carpeta
```
mkdir "ruta\destino"
```
```
mkdir carpeta1 carpeta2
```

### Eliminar una carpeta
```
sudo rm -rf folderName
```
### Eliminar un archivo
```
sudo rm fileName
```

### Mover carpeta

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

# Ocultar o visualizar un archivo o carpeta como administrador
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

# Habilitar puerto en la VM
Usage: ufw COMMAND


|Commands               |Description                                    |
|-----------------------|-----------------------------------------------|
|enable                 |enables the firewall                           |
|disable                |disables the firewall                          |
|default ARG            |set default policy                             |
|logging LEVEL          |set logging to LEVEL                           |
|allow ARGS             |add allow rule                                 |
|deny ARGS              |add deny rule                                  |
|reject ARGS            |add reject rule                                |
|limit ARGS             |add limit rule                                 |
|delete RULE\|NUM       |delete RULE                                    |
|insert NUM RULE        |insert RULE at NUM                             |
|prepend RULE           |prepend RULE                                   |
|route RULE             |add route RULE                                 |
|route delete RULE\|NUM |delete route RULE                              |
|route insert NUM RULE  |insert route RULE at NUM                       |
|reload                 |reload firewall                                |
|reset                  |reset firewall                                 |
|status                 |show firewall status                           |
|status numbered        |show firewall status as numbered list of RULES |
|status verbose         |show verbose firewall status                   |
|show ARG               |show firewall report                           |
|version                |display version information                    |
```
sudo ufw status
```
```
sudo ufw allow <port>
```
