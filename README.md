![Logo del Grupo NVI](https://raw.githubusercontent.com/jehna/readme-best-practices/master/sample-logo.png)

# Aprendiendo desarrollo Frontend

> La intención de este proyecto es familiarizar a los nuevos programadores con las mejores prácticas de desarrollo Frontend.

## Por dónde empezar

Para comenzar todo proyecto web que se respete debe tener un repositorio git, donde se debe llevar el seguimiento de todos los cambios realizados en el proyecto. Los repositorios públicos más comunes son:

* [GitHub](https://github.com/)
* [Bitbucket](https://bitbucket.org/product/)

Para aprender más sobre qué es un repositorio y aprender lo básico de git, consulte [aquí](https://uniwebsidad.com/libros/pro-git?from=librosweb).

También, una buena práctica es añadir un archivo README.md como este en el directorio raíz del proyecto. Para saber más detalles consulta [aquí](https://github.com/jehna/readme-best-practices).

### Configuración inicial

Los tutoriales que se están consultado para aprender HTML5 y CSS3 son:
* El gran libro de HTML5, CSS3 y JavaScript, 3a Edición, J.D. Gauchat.
* Udemy.com --- Desarrollo Web Completo con HTML5, CSS3, JS AJAX PHP y MySQL --- Instructor, Juan Pablo de la Torre

## Desarrollo

Comienza clonando este repositorio en el directorio de tu preferencia con el siguiente comando:

```shell
git clone https://github.com/GaboHb/CSS-GitHub.git
cd CSS-GitHub/
```

> Gabo: Aquí la práctica recomendable cuando trabajas proyectos web es nombrar los directorios en minúsculas y separados por guiones bajos.

### Archivo .gitignore

Piensa que no todos los archivos y carpetas son necesarios de gestionar a partir del sistema de control de versiones. Hay código que no necesitas enviar a Git, para ello deberás emplear siempre un archivo del tipo ```.gitignore````

Para máyores detalles, [consultar esto](https://desarrolloweb.com/articulos/archivo-gitignore.html).

### Scaffolding | .gitkeep

>[Definición en Wikipedia](https://es.wikipedia.org/wiki/Andamiaje_(programaci%C3%B3n))

En este caso, más que apegarme a la definición original, aquí me referiré a él como la buena práctica derivada de las 5S: [Un lugar para cada cosa y cada cosa en su lugar.](http://www.gestionaobras.com/5s-un-lugar-para-cada-cosa-y-cada-cosa-en-su-lugar/)

Por ello cree una estructura muy básica de directorios y puse las cosas en su lugar, por favor revísala.

Si revisas con cuidado, te darás cuenta que a propósito puse algunos directorios que están vacíos,pero dentro contienen un archivo oculto [.gitkeep](https://developpaper.com/what-is-gitkeep-the-difference-between-gitignore-and-gitkeep/), el cual es empleado para indicarle al control de versiones que mantenga una copia de esos directorios.

En esto consiste precisamente el `Scaffolding.`

## ALERTA | TAREAS

>Pensé que ya habías asimilado la buena práctica de nunca trabajar sobre la rama máster, con tristeza veo que no.

## Por que nunca trabajar sobre la rama master:

La rama master nos permite siempre tener un espacio donde se encuentra el código del proyecto que ha sido aprobado y completamente limpio.

La ramificación en proyectos de git nos permite crear tantas ramas como sean necesarias para cada incidencia o funcionalidad del proyecto, las ramas entre otras características nos permite las multitareas y el trabajo en equipo.

# Workflow

El flujo de trabajo a emplear en este repositorio es [WunderFlow](https://wunderflow.wunder.io/).

## Branches

Siguiendo el flujo de trabajo WunderFlow contaremos con 3 ramas principales:

- **develop**: Rama de desarrollo.
- **staging**: Rama de testing.
- **master**: Rama de produccion.

Las ramas secundarias se nombrarán así:

- **feature/[ticket number]--[short description]**: Todas las ramas de desarrollo relacionadas a una tarea, comenzarán con la palabra feature seguido del número de ticket y una descripcion corta. Con ello se obtendrá un mejor control y seguimiento de la tarea.

- **hotfix/[ticket number]--[short description]**: un hotfix es una tarea que, como su nombre lo indica, es un arreglo rápido que quedara fuera de los realeases normales y solo debe ser usado en casos especiales.

### Branching

Siguiendo el flujo de WunderFlow, todas las ramas deberán iniciar de **master** como base, nunca de ninguna de las otras ramas principales. Si se da el caso que apenas inicia el proyecto, la rama **master** solamente contendrá el commit inicial, por lo qué, en esta única ocasión, las ramas iniciarán a partir de **develop**

### Merge Strategy

La estrategia de merge es individual para cada rama feature haciendo un merge por cada rama principal.

### Conflicts Resolution

Para resolver los conflictos que puedan existir entre ramas, al momento de hacer un merge deberán de ser resueltos por el encargado de hacer los merges ó, en su defecto, si se les indica, creando una rama pr/[branch to merge]/[ticket number].

**Ejemplo:**

Existe un conflicto a la hora de hacer un merge de un feature a develop

    git checkout develop
    git checkout -b pr/develop/NS-01
    git merge feature/NS-01-initial-commit

Posteriormente a esto, se resuelven los conflictos, se prueba el código y se genera un pull request de pr/develop/NS-01 a develop de esta forma se arreglan los conflictos sin ensuciar la rama `develop` principal.


>Ya te lo había puesto en algún otro archivo README, cópialo aquí para que nunca lo olvides e investiga los tipos de estrategias de ramificación que se pueden emplear con Git y pon en este documento las ligas de lo que investigaste.

ADICIONALMENTE:

## SASS

SASS es un lenguaje de hoja de estilo que se compila en CSS. Le permite usar variables, reglas anidadas, mixins, funciones y más, todo con una sintaxis totalmente compatible con CSS. SASS ayuda a mantener bien organizadas las hojas de estilo grandes y facilita compartir diseños dentro y entre proyectos.


## LESS

LESS CSS es un lenguaje de hojas de estilo CSS y funciona como un lenguaje de programación, permitiendo el uso de variables, funciones, operaciones aritmeticas, entre otras, para acelerar y enriquecer los estilos en un sitio web.

LESS CSS no reemplaza a CSS, de hecho el resultado final es una hoja de estilos css completamente funcional y compatible, simplemente ofrece mejoras en el área de desarrollo, por lo que usarlo se vuelve recomendable si quieres ahorrar tiempo de desarrollo, utilizar caracteristicas avanzadas de estilos y para ahorrarte trabajo, de allí su nombre: less css (menos css).