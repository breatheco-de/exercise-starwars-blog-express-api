# Exercise starwars blog express api


Es recomendado desarrollar este proyecto en conjunto con el [StarWars Blog Reading List](https://github.com/breatheco-de/exercise-starwars-blog-reading-list), eventualmente ese front-end se integrará con la API que vas a desarrollar en este proyecto y tendrás una aplicación completamente funcional con front-end y back-end.

Hoy vamos a construir una API para administrar un blog (El StarWars Blog), los usuarios de este blog van a poder listar planetas, personajes, y agregar o eliminar favoritos.

Para permitir que los usuarios hagan todo esto, debemos seguir los siguientes pasos:

1. Comienza por modelar la base de datos: crea una base de datos y las tablas necesarias para almacenar esa información, es posible que ya lo hayas hecho en el proyecto StarWars DataModeling en [node/express](https://github.com/breatheco-de/starwars-data-model-typeorm-node).
2. Crea tus endpoints utilizando Express.
3. Prueba constantemente tus endpoints con [Postman](https://www.postman.com/).

## 🌱 Cómo comenzar este proyecto

No clones este repositorio porque vamos a usar una plantilla diferente.

Recomendamos abrir el `express.js template` usando un entorno de desarrollo como [Codespaces](https://4geeks.com/es/lesson/tutorial-de-github-codespaces) (recomendado). Alternativamente, puedes clonarlo en tu computadora local usando el comando `git clone`.

Estos son los repositorios que necesitas abrir o clonar:

```text

https://github.com/4GeeksAcademy/expressjs-rest-hello
```

> ⚠ Si trabajas localmente debes tener una base de datos y Node.js pero si usas Codespaces o Gitpod ya viene todo instalado.

**👉 Por favor sigue estos pasos sobre** [cómo comenzar un proyecto de programación](https://4geeks.com/es/lesson/como-comenzar-un-proyecto-de-codificacion).

> 💡 Importante: Recuerda guardar y subir tu código a GitHub creando un nuevo repositorio, actualizando el remoto (`git remote set-url origin <your new url>`) y subiendo el código a tu nuevo repositorio usando los comandos `add`, `commit` y `push` desde la terminal de git.

## 📝 Instrucciones

Crea una API conectada a una base de datos e implemente los siguientes endpoints (muy similares a SWAPI.dev or SWAPI.tech):

- `[GET] /people` Recuperar todos los registros de people de la base de datos usando Express.
- `[GET] /people/:people_id` Mostrar la información de un solo personaje según su id, utilizando parámetros de ruta en Express.
- `[GET] /planets` Recuperar todos los registros de planets de la base de datos.
- `[GET] /planets/:planet_id` Mostrar la información de un solo planeta según su id.
Además, crea los siguientes endpoints para gestionar usuarios y sus favoritos:

- `[GET] /users` Recuperar todos los usuarios del blog desde la base de datos.
- `[GET] /users/favorites` Recuperar todos los favoritos que pertenecen al usuario actual.
- `[POST] /favorite/planet/:planet_id` Añadir un nuevo planet favorito al usuario actual, donde :planet_id representa el ID del planeta que se añadirá.
- `[POST] /favorite/people/:people_id` Añadir un nuevo people favorito al usuario actual, donde :people_id representa el ID del personaje que se añadirá.
- `[DELETE] /favorite/planet/:planet_id` Eliminar un planet favorito del usuario actual utilizando su id.
- `[DELETE] /favorite/people/:people_id` Eliminar un people favorito del usuario actual utilizando su id.

- Tu API actual no cuenta con un sistema de autenticación implementado aún. Por lo tanto, la única forma de crear usuarios es directamente en la base de datos. Usa herramientas como un panel de administración o un gestor de bases de datos para añadir usuarios de forma manual.

> Nota: Aquí hay un ejemplo en Postman: https://documenter.getpostman.com/view/2432393/TzRSgnTS#a4174b48-3fc8-46e3-bf82-19a08107666f

## 📖 Fundamentos

Este ejercicio te permitirá practicar las siguientes habilidades y conceptos:

1. Construcción de APIs utilizando el standard REST (a.k.a: RESTful APIs).
2. Construir una base de datos utilizando el **ORM** llamado [TypeORM](https://typeorm.io/).
3. Utilizar y entender sistemas de migraciones de bases de datos con las migraciones nativas de TypeORM.

## 😎 Te sientes con confianza?

Los siguientes requerimientos no son necesarios para completar el proyecto satisfactoriamente, pero puedes desarrollarlos para continuar tu aprendizaje si te sientes con suficiente confianza.

`+4` Crea endpoints para agregar (POST), modificar (PUT) y eliminar (DELETE) `planets` y `people`. De esta manera, toda la base de datos va a poder ser administrada vía API en vez de depender del admin.

Este y otros proyectos son usados para [aprender a programar](https://4geeksacademy.com/es/aprender-a-programar/aprender-a-programar-desde-cero) por parte de los alumnos de 4Geeks Academy [Coding Bootcamp](https://4geeksacademy.com/us/coding-bootcamp) realizado por [Alejandro Sánchez](https://twitter.com/alesanchezr) y muchos otros contribuyentes. Conoce más sobre nuestros [Cursos de Programación](https://4geeksacademy.com/es/curso-de-programacion-desde-cero?lang=es) para convertirte en [Full Stack Developer](https://4geeksacademy.com/es/coding-bootcamps/desarrollador-full-stack/?lang=es), o nuestro [Data Science Bootcamp](https://4geeksacademy.com/es/coding-bootcamps/curso-datascience-machine-learning).