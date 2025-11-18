## ¿Cómo crear el directorio .ssh?
``` Code
# Create directory
mkdir -p ~/.ssh
```
``` Code
# Assign permission
chmod 700 ~/.ssh
```
``` Code
# Verify archivos ocultos
ls -al ~/grep|.ssh
```

## ¿Cómo crear una copia de seguridad de los .ssh?
``` Code
# Backup
cp -r ~/.ssh ~/.ssh_backup
```
``` Code
# Si quieres empezar desde cero, puedes hacer backup y eliminar todo
cp -r ~/.ssh ~/.ssh_backup
rm -rf ~/.ssh
```

## ¿Cómo visualizar los archivos SSH?
``` Code
ls -al ~/.ssh
```
``` Code
ls -la ~/.ssh
```
``` Code
ls -a -l ~/.ssh
```
``` Code
ls -l -a ~/.ssh
```
``` Code
ls --all -l ~/.ssh
```

## ¿Cómo generar la clave SSH ed25519 o RSA 4096?
``` Keygen
ssh-keygen -t ed25519 -C "correo@domain.com" -f ~/.ssh/id_ed25519_<user_name>
```
``` Keygen
ssh-keygen -t rsa -b 4096 -C "correo@domain.com" -f ~/.ssh/id_rsa_<user_name>
```

## ¿Cómo eliminar la clave SSH?
`Eliminar la clave privada`
```
rm ~/.ssh/id_ed25519
```

`Eliminar la clave pública`
```
rm ~/.ssh/id_ed25519.pub
```

## ¿Cómo asignar permiso a la clave SSH?
``` Permission
# Iniciar el agente SSH en segundo plano
eval "$(ssh-agent -s)"
```
``` Permission
# Agregar tu clave privada (ejemplo para ed25519)
ssh-add ~/.ssh/id_ed25519_<username>
```

## ¿Cómo verificar si la conexión con GitHub fue exitoso?
``` Permission
ssh -T git@github.com
```
`
Hi <username>! You've successfully authenticated, but GitHub does not provide shell access.
`

## ¿Cómo ver la clave pública?
``` show keygen
cat ~/.ssh/id_ed25519_<username>.pub
```
