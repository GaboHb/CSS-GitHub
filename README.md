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

Gabriel, por favor indica aquí que tutoriales estás siguiendo, gracias.

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

Cuando aprendas algo, utilízalo constantemente si no, lo vas a olvidar. Por ello, de tarea añade aquí el porqué no trabajar nunca sobre la rama máster.

>Ya te lo había puesto en algún otro archivo README, cópialo aquí para que nunca lo olvides e investiga los tipos de estrategias de ramificación que se pueden emplear con Git y pon en este documento las ligas de lo que investigaste.

ADICIONALMENTE:

* Investigar que son SASS y LESS e implementa el uso de SASS en todos tus archivos .css
* Corrige todos tus .html para que carguen los .css generados correctamente.

`¡SUERTE!`
