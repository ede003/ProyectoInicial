

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

<details><summary> <b> CLASE 2️⃣ </b></summary></details>

# States y Commits
Git tiene 3 estados, los cuales son:

1.  *Modified:* Cuando un archivo tiene cambios marcados para ser confirmados 

2.  *Staged:* Los archivos modificados ya están listos para ser confirmados en el repositorio local.

3.  *Commited:* Los cambios fueron guardados en el repositorio local (commit).
   
## ¿Qué es un commit?
Son aquellos que sirven para registrart los cambios que se han hecho en el repositorio

> 💡 **Nota:** Podriamos imaginar un commit como una fotografía, cada una es como un estado de todos los archivos del repositorios

