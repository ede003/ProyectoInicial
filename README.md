

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

<details><summary> <b> CLASE 3️⃣ </b></summary></details>

## ¿Para qué sirven las ramas?
Permiten realizar un desarrollo no lineal y colaborativo

>Las ramas pueden acabar de dos maneras:
>* Terminar en el olvido
>* Ser fusionada en otra rama

## Fusionar ramas
 Es el proceso en el cual se integran los cambios de una rama en otra

