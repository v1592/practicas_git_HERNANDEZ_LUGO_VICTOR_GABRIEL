# Práctica de Git y GitHub

## Datos del estudiante

**Nombre completo:** VICTOR GABRIEL HERNANDEZ LUGO
**Matrícula:** 2630005

## Nombre de la práctica

**Creación y sincronización de un repositorio local con GitHub**

## Objetivo

El objetivo de esta práctica es aprender a crear un repositorio local utilizando Git, vincularlo con un repositorio remoto en GitHub y comprobar la sincronización de información en ambos sentidos: del repositorio local hacia GitHub y de GitHub hacia el repositorio local.

## Descripción del procedimiento

Primero se creó una carpeta llamada `practica-git-nombre-apellido`. Dentro de esta carpeta se abrió PowerShell y se inicializó un repositorio utilizando Git.

Después se configuró la rama principal con el nombre `main` y se crearon los archivos `README.md` y `datos.txt`. En el archivo `datos.txt` se agregó información inicial relacionada con la práctica.

Posteriormente se verificó el estado del repositorio, se agregaron los archivos al área de preparación y se realizó el primer commit para guardar los cambios en el historial de Git.

Después se creó un repositorio público en GitHub con el mismo nombre. El repositorio remoto se dejó vacío para que los primeros archivos provinieran del repositorio local.

Finalmente, se vinculó el repositorio local con GitHub y se enviaron los archivos mediante `git push`.

## Comandos de Git utilizados

| Comando                     | Función                                                                          |
| --------------------------- | -------------------------------------------------------------------------------- |
| `git init`                  | Inicializa un nuevo repositorio de Git en la carpeta actual.                     |
| `git branch -M main`        | Cambia el nombre de la rama principal a `main`.                                  |
| `git status`                | Muestra el estado actual del repositorio y los archivos que tienen cambios.      |
| `git add .`                 | Agrega los archivos modificados al área de preparación.                          |
| `git commit -m "mensaje"`   | Guarda los cambios preparados en el historial del repositorio.                   |
| `git remote add origin URL` | Vincula el repositorio local con un repositorio remoto.                          |
| `git remote -v`             | Muestra los repositorios remotos configurados.                                   |
| `git push -u origin main`   | Envía los commits de la rama `main` desde el repositorio local hacia GitHub.     |
| `git push`                  | Envía los nuevos commits locales al repositorio remoto.                          |
| `git pull origin main`      | Descarga los cambios realizados en GitHub y los integra en el repositorio local. |

## Creación del repositorio local

El repositorio local se creó mediante el comando `git init`. Después se estableció la rama principal como `main`. Se crearon los archivos necesarios para la práctica y se registraron los primeros cambios mediante un commit.

## Vinculación del repositorio local con GitHub

Para conectar el repositorio local con GitHub se utilizó el comando `git remote add origin` seguido de la URL del repositorio remoto. Después se utilizó `git remote -v` para comprobar que el repositorio remoto estuviera configurado correctamente.

## Sincronización Local → GitHub

La primera sincronización se realizó utilizando `git push -u origin main`. Este comando permitió enviar los archivos y commits que estaban en el repositorio local hacia el repositorio remoto de GitHub.

Posteriormente se realizó una modificación en el archivo `datos.txt` desde la computadora. El cambio se registró utilizando `git add`, `git commit` y finalmente `git push`, enviando la actualización a GitHub.

## Sincronización GitHub → Local

Para comprobar el flujo contrario, se modificó directamente el archivo `datos.txt` desde GitHub. Después se utilizó el comando `git pull origin main` desde PowerShell para descargar los cambios realizados en GitHub y actualizarlos en el repositorio local.

De esta manera se comprobó que los cambios realizados en GitHub también podían obtenerse en la computadora.

## Archivos contenidos en el repositorio

### README.md

Contiene la documentación de la práctica, incluyendo los datos del estudiante, objetivo, procedimiento, comandos utilizados y conclusión.

### datos.txt

Contiene información relacionada con la práctica y fue utilizado para comprobar la sincronización entre GitHub y el repositorio local.

## Historial de cambios

Durante la práctica se realizaron varios commits para registrar los cambios del proyecto. También se realizó una modificación desde GitHub y otra desde el repositorio local para comprobar el funcionamiento de la sincronización en ambos sentidos.

## Conclusión

Con esta práctica aprendí a utilizar Git para controlar las versiones de un proyecto y GitHub como repositorio remoto. También aprendí a enviar cambios desde mi computadora hacia GitHub utilizando `git push` y a descargar cambios realizados en GitHub mediante `git pull`.

La práctica me permitió comprender cómo se relacionan un repositorio local y uno remoto, además de conocer la importancia de los commits para llevar un registro de las modificaciones realizadas en un proyecto.
