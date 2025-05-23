

<details><summary> <b> CLASE  1️⃣</b></summary>

# Introducción a Git
---
Antes de empezar...
> 💡 **Nota:** ¿Qué es un control de versiones?  
> Un control de versiones es un historial de cada cambio que se realiza en el código fuente de un proyecto. Es importante porque da rendimiento, seguridad y flexibilidad.

#### Un poco de historia de Git

- **1990** → Nace CVS, primer controlador de versiones.
- **2005** → *Linus Torvalds crea Git* ✨  Después de caída de Bitkeeper.
- **2008** → Creación de **GitHub**
- **2018** → Microsoft compra GitHub, pero sigue siendo gratuito.
- **2024** → Git domina el mercado.

entonces:

## ¿Qué es Git?

<img src="https://avatars.githubusercontent.com/u/18133?s=280&v=4" align="right" alt="Logo de Git" width="100" height="100">


Git es un sistema distribuido de control de versiones, donde los cambios en el código son registrados por un historial en sus ficheros para saber quién y cuándo lo hizo.
Puede tener uno o varios repositorios remotos para sincronizarlos.

## ¿Qué es un repositorio?  

Es una carpeta de almacenamiento de varias versiones de los ficheros de un proyecto y el historial de los cambios hechos en ellos.  
Los repositorios pueden ser de dos tipos:
* **Locales** (en nuestro ordenador)  
* **Remotos** (en un servidor externo)
  
<img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj7CpqGNI2ceZA6Kc5VJL6l2OopC2GE-4xCdduHCyo8ZhwUhxREhEfFkH0IthUE5HqVASxGXl2SET_CrKEMmmagqSxEeSfxxV9Hq_7wf41vHuXZhAOAeO59K0lvXY7MWSlV7VwLKINVf4k/s640/Repositorios.PNG" alt="Repositorios Git" width="500" height="150"/>


## ¡Inicia tu proyecto con Git!
Crea tu proyecto en una carpeta de tu preferencia con el comando:
 ```
git init <nombre de tu proyecto>
```
aparecerá un **(main)** al lado de tu ruta
</details>

Resumen comandos:

| Comando                     | Descripción                                                                |
| -------------------------   | -----------------------------------------------------------------          |
| `git init <nuevo_proyecto>` | Inicia un nuevo repositorio Git.                                           |


<details><summary> <b> CLASE 2️⃣ </b></summary>

# States y Commits
Git tiene 3 estados, los cuales son:

1.  *Modified:* Cuando un archivo tiene cambios marcados para ser confirmados 

2.  *Staged:* Los archivos modificados ya están listos para ser confirmados en el repositorio local.

3.  *Commited:* Los cambios fueron guardados en el repositorio local (commit).
   
## ¿Qué es un commit?
Son aquellos que sirven para registrart los cambios que se han hecho en el repositorio

> 💡 **Nota:** Podriamos imaginar un commit como una fotografía, cada una es como un estado de todos los archivos del repositorios

## ¿Cómo hacer un commit?

Para guardar los cambios que se tienen en el área de staging, añadiendo directamente un mensaje, se usará el siguiente comando:

 ```
git commit -m "Mensaje"
```
>El mensaje se usará como el título del commit.

Si se quiere añadir información adicional, se puede volver a usar el parámetro **-m** las veces que se requiera.

 ```
git commit -m "Mensaje" -m "Mensaje adicional"
```
## ¿Qué es el HEAD?
Es como un indicador que dice: "ESTÁS AQUÍ"
Solo se puede estar en un lugar, ese es el HEAD.

## ¿Qué es una rama?
Es una instantánea (snapshot) de la división del estado del código

>Es como un nuevo apuntador hacia una de las confirmaciones

<img src="https://res.cloudinary.com/snyk/images/f_auto,q_auto/w_1240,h_384,c_scale/v1/wordpress-sync/image1-11/image1-11-1240x384.png" alt="Repositorios Git" width="500" height="150"/>

</details>

Comandos nuevos:

| Comando                     | Descripción                                                                |
| -------------------------   | -----------------------------------------------------------------          |
| `git status`                | Muestra el estado actual del proyecto.                                     |
| `git add .`                   | Agrega todos los archivos al repositorio de Git.                           |
| `git restore --staged`      | Evita que los cambios en el área de preparación se incluyan en el commit.  |
| `git commit`                | Genera un registro del cambio realizado.                                   |
| `git log`                   | Muestra un historial de los commits realizados.                            |
| `git commit -amend-m`       | Permite editar el mensaje del commit.                                      |
| `git branch `               | Nos muestra todas las ramas del repositorio actual.                        |
| `git branch <nombre_rama>`  | Crear una rama este tiene diferentes complementos.                         |
| `git switch <nombre_rama>`  | Permite cambiar de una rama a otra en nuestro repositorio loca.            |
| `git checkout <nombre_rama>`| Cambia la ubicación actual al "nombre_rama" con todos los cambios.         |
| `git branch -a`             | Permite ver a las ramas locales y remotas.                                 |
| `git branch -d`             | Permite eliminar una rama.                                 |
| `git branch -m currentName newName`             | Permite cambiar nombre de una rama                                |

<details><summary> <b> CLASE 3️⃣ </b></summary>

# RAMAS

## ¿Para qué sirven las ramas?
Permiten realizar un desarrollo no lineal y colaborativo

>Las ramas pueden acabar de dos maneras:
>* Terminar en el olvido
>* Ser fusionada en otra rama

## Fusionar ramas
 Es el proceso en el cual se integran los cambios de una rama en otra

 <img src="https://blueelephpant.wordpress.com/wp-content/uploads/2018/08/1_tnvrls6dg7vft0zgdtfu_w.png" alt="Repositorios Git" width="500" height="230"/>

## Eliminar ramas

Eliminar ramas es una buena práctica 
> Recordemos que las ramas tienen un propósito único y  corto tiempo de periodo

## Conflictos en Git 
Un conflicto en Git ocurre cuando Git no puede fusionar automáticamente cambios de diferentes ramas porque hay modificaciones incompatibles en las mismas líneas de un archivo o archivos diferentes que interfieren entre sí.

### ¿Cómo resolver un conflicto en Git?
* Se debe elegir una versión
* Combinar ambas opciones
* Escribir algo nuevo

</details>

Resumen de comandos
| Comando                     | Descripción                                                                |
| -------------------------   | -----------------------------------------------------------------          |
| `git merge --edit`                | Abre el editor antes de hacer el commit.                                     |
| `git merge --no-commit`                | Evita que se haga commit automáticamente.                                     |
| `git branch <nombre rama>`                | Crea una nueva rama con el nombre especificado.                                     |
| `git branch -a`                | Lista todas la ramas, locales y remotas                                     |
| `ggit branch -d <nombre rama>`                | Eimina una rama local (solo si ya fue fusionada, de lo contrario, usar -D para forzar).                                     |
| `git merge <nombre rama>`                | Fusiona la rama especificada con la rama actual..                                     |

<details><summary> <b> CLASE 4️⃣  </b></summary>

# GIT HUB

## ¿Git y GitHub son lo mismo?
No... 
* Git es un control de versiones.
* GitHub es un servicio de alojamiento en la nube de código fuente basado en el sistema de control de versiones que git ofrece para manejar repositorios.

## Repositorios remotos
Es una copia de un proyecto en la nube, el cual se puede sincronizar con un repositorio local

# PUSH, PULL y PULL REQUEST
> git push
Nos sirve para empujar cualquier cmabio del repositorio local al remoto

> git pull
Nos sirve para descargar los cambios del repositorio remoro al local

### ¿Qué es una pull request?
Es una petición de cambios que se envía al respositorio original 
</details>

Comandos:
| Comando                     | Descripción                                                                |
| -------------------------   | -----------------------------------------------------------------          |
| `git remote add <alias> <URL-repositorio-remoto>`| Enlaza nuestro repositorio local con nuestro repositorio remoto.|
| `git push <alias> main`     | Sicroniza nuestros cambios de mi repositorio local con mi repositorio remoto.|
| `git clone <url-repositorio-remoto>`| Sirve para clonar un repositorio existente en un nuevo directorio local.|
| `git remote -v`             | Muestra que nuestro repositorio esta enlazado con el repositorio remoto.   |
| `git push origin <nombre_rama>`| Creamos una rama remota.				                   |
| `git fetch`                 | Actualiza la información entre mi repositorio remoto y local.	           |
| `git push -u`               | Envia los commits locales al repositorio remote y establece la rama como referencia. |
| `git push -d <alias> <rama-remota>` | Borrar una rama remota.                                            |
| `git push -f`               | Fuerza un push.                                                            |
| `git push <alias> <rama 1> <rama 2> <rama N>` | Enviar los commits locales de una o varias ramas específicas a un repositorio remoto.|
| `git pull`               | Envia los commits locales al repositorio remoto y establece a la rama como referencia. |
| `git pull --all`            | Descarga todos los cambios de todas las ramas remotas y  las fusiona con las del repositorio local. |


</details>

<details><summary> <b> CLASE 5️⃣  </b></summary>

# GIT FLOW, GIT HUB FLOW

## GIT FLOW
### ¿Qué es un GitFlow?
> Es la manera en la que el equipo de desarrollo va a utilizar Git para poder trabajar de manera colaborativa.

 <img src="https://www.bitbull.it/blog/git-flow-come-funziona/gitflow-1.png" alt="Repositorios Git" width="500" height="230"/>

Usa las ramas:
* Main, contiene el código de producción
* Develop: Esta rama de desarrollo donde se realizan los cambios principales.
* Features: Estos son caracteristicas nuevas del proyecto.
* Release: Estos son cambios de último momento.
* Hotflix: Son parches o arreglar bugs pequeños que son parte del main. 

## GIT HUB FLOW
>Es un flujo de trabajo de git mas simple, porque solo utiliza dos ramas.

<img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1668070000889/rvf5Hx764.png" alt="Repositorios Git" width="500" height="200"/>

</details>

<details><summary> <b> CLASE 6️⃣  </b></summary>

# BUENAS PRÁCTICAS DE GIT

## ¿Por qué son importantes las buenas prácticas?
* Funcionan como un estándar
* Resolver conflictos durante el desarrollo es más fácil
* El historial de commits es más legible

## **1. ¿Cada cuánto debería hacer un commit?**
A menudo.
>Los commits deben ser pequeños agrupando pequeñas mejoras o acciones.

### ¿Como escribir un buen commit?
>Se debe usar un verbo imperativo.Por ejemplo: "Add", "Feat", etc.
>No se debe usar puntos suspensivos o punto final.
>El commit debe tener como máximo 50 caracteres.
>El commit debe ser claro y especifico.
>Se debe usar un prefijo para los commits y que estos sean más semánticos.

#### Ejemplo

feat: add new search feature
^--^  ^--------------------^
│     │
│     └--> # Descripción de los cambios
│
└──------> # Tipo del cambio

### Prefijos para los commits

- **feat**: Nueva característica para el usuario.
- **fix** : Es cuando se arregla un bug que afecta al usuario..
- **perf**: Es para cambios que mejoran el rendimiento del sitio. 
- **build**: Es para cambios en el sistema de build, tareas de despliegue o instalación.
- **ci** : Es para cambios en la integración continua.
- **docs** : Es para cambios en la documentación.
- - **refactor**: Es para la refactorización del código como cambios de nombre de variables o funciones.
- **style** : Es para cambios de formato, tabulaciones, espacios o puntos y coma, etc; no afectan al usuario.
- **test** : Este añade tests o refactoriza uno existente.

## 2. Buenas prácticas en ramas
#### ¿Como elegir un buen nombre para mi rama?
>Para elegir un buen nombre de la rama, es recomendable usar el nombre de la accion que se va a realizar en la rama.

</details>

<details><summary> <b> CLASE 7️⃣ </b></summary>

# DESHACER CAMBIOS

## ¿Cuándo deshacer cambios?

>Cuando el proyecto deja de funcionar.
>Para recuperar código eliminado.
>Para recuperar archivos eliminados.

## ¿Qué comando debo usar para deshacer un cambio que hice en un archivo?

>Esto depende de si desea deshacer el cambio en todo el commit o solo en el archivo.
>Si desea deshacer el cambio en todo el commit, use git reset soft <commit_id>.
>Si desea deshacer el cambio solo en el archivo, use git checkout -- <commit_id> <archivo> && git checkout HEAD -- <archivo>.

## Comandos destructivos y no destructivos

### Comandos destructivos

>Estos afectan el historial de commits realizados.

>Entre estos tenemos:

- **git rebase**
- **git commit amend**
- **git reset**
- **git push --force**

### Comandos no destructivos
>Trabajan en base al historial sin afectarlo.
>Entre estos tenemos:

- **git checkout**
</details>

<details><summary> <b> CLASE 8️⃣ </b> </summary>

# HOOKS, ALIAS Y TRUCOS DE GIT

## ¿Qué son los Hooks?
>Los Hooks son scripts que se ejecutan automáticamente antes o después de que ocurra un evento específico en Git.
>Estos eventos pueden ser: commits, pushes, entre otros.
>Estos permiten automatizar tareas repetitivas, como enviar notificaciones por Slack o ejecutar pruebas unitarias.

>Existen dos:
- **Hooks del lado del cliente**
  >Afectan solo al repositorio local que los contiene.
  >Pueden ser:
  >-**Pre-commit**: Se ejecuta antes de que se realice un commit. Se puede utilizar para verificar que el código cumpla con ciertos estándares o para ejecutar pruebas unitarias.
  >-**Post-commit**: Se ejecuta después de que se realiza un commit. Se puede utilizar para enviar notificaciones por Slack o para actualizar automáticamente la documentación.
  >-**Pre-push**: Se ejecuta antes de que se envíe un push al repositorio remoto. Se puede utilizar para verificar que no se estén enviando cambios no deseados.
  >-**Post-push**: Se ejecuta después de que se envía un push al repositorio remoto. Se puede utilizar para actualizar automáticamente la rama de producción o para enviar notificaciones a otros desarrolladores.
  >-**Post-checkout-Post-merge**: Permite limpiar un directorio de trabajo, tras realizar un checkout.
- **Hooks del lado del servidor**
  >Pueden ser:
  >-**Pre-receive**: Comprueba los commits que se quieran guardar.
  >-**update**: Es cuando llega ese git push y haces comprobaciones.
  >-**post-receive**: Es cuando el push ya sea ha sincronizado y haces acciones. 
  
## ¿Qué son los Alias?
>Son atajos que permiten personalizar los comandos de Git.

</summary>
</details>