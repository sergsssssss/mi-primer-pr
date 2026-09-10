# Git Cheatsheet

Una chuleta rápida con los comandos de Git más usados en el día a día.

## Configuración inicial

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

## Empezar un repositorio

```bash
git init                  # Crea un repo nuevo en la carpeta actual
git clone <url>            # Clona un repo remoto
```

## Estado y cambios

```bash
git status                 # Ver qué archivos han cambiado
git diff                   # Ver los cambios línea a línea
git add <archivo>           # Añadir un archivo al área de staging
git add .                  # Añadir todos los cambios
git commit -m "mensaje"    # Guardar los cambios en un commit
```

## Ramas

```bash
git branch                 # Listar ramas
git branch <nombre>        # Crear una rama nueva
git checkout <nombre>       # Cambiar de rama
git checkout -b <nombre>    # Crear y cambiar a una rama nueva
git merge <nombre>          # Fusionar una rama en la actual
```

## Remotos

```bash
git remote -v               # Ver remotos configurados
git push origin <rama>       # Subir cambios al remoto
git pull origin <rama>       # Traer cambios del remoto
```

## Historial

```bash
git log                    # Ver el historial de commits
git log --oneline           # Historial resumido, una línea por commit
```

## Guardar cambios temporalmente (stash)

```bash
git stash                  # Guardar cambios sin confirmar y limpiar el working directory
git stash list              # Ver la lista de stashes guardados
git stash pop               # Recuperar el último stash y eliminarlo de la lista
git stash apply             # Recuperar el último stash sin eliminarlo de la lista
git stash drop               # Eliminar el último stash sin aplicarlo
```

## Deshacer cambios

```bash
git checkout -- <archivo>   # Descartar cambios locales de un archivo
git reset HEAD <archivo>    # Sacar un archivo del staging
git revert <commit>         # Crear un commit que deshace otro
```
