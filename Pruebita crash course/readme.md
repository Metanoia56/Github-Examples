## Cloning

Se puede clonar conHTTPS, SSH, Github CLi

Para crear un directorio temporal en codespaces
```sh
mkdir workspaces/tmp
cd workspaces/tmp
```

### HTTPS

```sh
git clone https://github.com/Metanoia56/Github-Examples.git
```

### SSH
Primero ssh-keygen -t ed25519 -C "tu_email@example.com"
Luego eval "$(ssh-agent -s)" y ssh-add ~/.ssh/id_ed25519
Luego cat ~/.ssh/id_ed25519.pub

```
git@github.com:Metanoia56/Github-Examples.git
```
Se necesitará crear una key SSH

```
ssh-keygen -t rsa
luego un cat al archivo.pub y se añade a la cuenta de github

Comandos que pueden ayudar: ssh-add C:\Users\JDiego\.ssh
```

## CLI
No se tiene que tener una clave ssh agregada a la cuenta. Se empieza con:
```
gh auth login
```
Y luego se selecciona la key local .pub
```
gh repo clone Metanoia56/Github-Examples
```
Luego comit y push

## Git hidden folder

Si se quisiera inicializar Git manualmente, se podia hacer así

```sh
mkdir /workspaces/tmp/new-prj
cd /workspaces/tmp/new-prj
git init --Se iniciar Git--
touch readme.md
open readme.md
git commit -a -m "readme file anadido"
```
## commits
```sh
Para hacer un commit: git commit
```
Para configurar el editor global
```
git config --global core.editor emacs
```
Hacer commit y agregar detalles
```
git commit -m "detalles"
```
## branches
Para ver la lista de branches
```
git branches
```
Para crear un branch
```
git branch "name"
```

Tambien se tiene que crear el branch en el repositorio
```
git push -u origin pangod
```
## remotes

## stashing

## merging

## add
```sh
git . para agregar todos los files a staged
```

## Reset
```sh
git reset removerá los documentos que iban a ser staged
```

## Git config file
El config file almacena la config global
```
git config --list
```
Variables a configurar
```
git config --global user.name "Pancito Man"
git config --global user.email juanasda@gmail.com
```

## Log
Para revisar el log de los commits
```
git log
```

## Push

Para hacer push a un repositorio a un remote origin osea agregar commits desde un lugar externo, se usa el personal token, antes de eso se hace un git glone del repositorio

```
git push
```