# Exercise StarWars Blog Express API

It is recommended to develop this project together with the [StarWars Blog Reading List](https://github.com/breatheco-de/exercise-starwars-blog-reading-list). Eventually, that front-end will integrate with the API you will develop in this project, and you will have a fully functional application with both front-end and back-end.

Today we are going to build an API to manage a blog (The StarWars Blog). Users of this blog will be able to list planets, characters, and add or remove favorites.

To allow users to do all this, we must follow these steps:

1. Start by modeling the database: create a database and the necessary tables to store that information. You may have already done this in the StarWars DataModeling project in [node/express](https://github.com/breatheco-de/starwars-data-model-typeorm-node).
2. Create your endpoints using Express.
3. Constantly test your endpoints with [Postman](https://www.postman.com/).

## 🌱 How to start this project

Do not clone this repository because we are going to use a different template.

We recommend opening the `express.js template` using a development environment like [Codespaces](https://4geeks.com/es/lesson/tutorial-de-github-codespaces) (recommended). Alternatively, you can clone it on your local computer using the `git clone` command.

These are the repositories you need to open or clone:

```text
https://github.com/4GeeksAcademy/expressjs-rest-hello
```

> ⚠ If you work locally, you must have a database and Node.js, but if you use Codespaces or Gitpod, everything is already installed.

**👉 Please follow these steps on** [how to start a coding project](https://4geeks.com/es/lesson/como-comenzar-un-proyecto-de-codificacion).

> 💡 Important: Remember to save and upload your code to GitHub by creating a new repository, updating the remote (`git remote set-url origin <your new url>`), and uploading the code to your new repository using the `add`, `commit`, and `push` commands from the git terminal.

## 📝 Instructions

Create an API connected to a database and implement the following endpoints (very similar to SWAPI.dev or SWAPI.tech):

- `[GET] /people` Retrieve all people records from the database using Express.
- `[GET] /people/:people_id` Show the information of a single character by its id, using route parameters in Express.
- `[GET] /planets` Retrieve all planet records from the database.
- `[GET] /planets/:planet_id` Show the information of a single planet by its id.

Additionally, create the following endpoints to manage users and their favorites:

- `[GET] /users` Retrieve all blog users from the database.
- `[GET] /users/favorites` Retrieve all favorites that belong to the current user.
- `[POST] /favorite/planet/:planet_id` Add a new favorite planet to the current user, where :planet_id represents the ID of the planet to be added.
- `[POST] /favorite/people/:people_id` Add a new favorite character to the current user, where :people_id represents the ID of the character to be added.
- `[DELETE] /favorite/planet/:planet_id` Remove a favorite planet from the current user using its id.
- `[DELETE] /favorite/people/:people_id` Remove a favorite character from the current user using its id.

- Your current API does not have an authentication system implemented yet. Therefore, the only way to create users is directly in the database. Use tools like an admin panel or a database manager to manually add users.

> Note: Here is an example in Postman: https://documenter.getpostman.com/view/2432393/TzRSgnTS#a4174b48-3fc8-46e3-bf82-19a08107666f

## 📖 Fundamentals

This exercise will allow you to practice the following skills and concepts:

1. Building APIs using the REST standard (a.k.a: RESTful APIs).
2. Building a database using the **ORM** called [TypeORM](https://typeorm.io/).
3. Using and understanding database migration systems with TypeORM's native migrations.

## 😎 Feeling confident?

The following requirements are not necessary to complete the project successfully, but you can develop them to continue your learning if you feel confident enough.

`+4` Create endpoints to add (POST), modify (PUT), and delete (DELETE) `planets` and `people`. This way, the entire database can be managed via API instead of relying on the admin.

This and other projects are used to [learn to code](https://4geeksacademy.com/es/aprender-a-programar/aprender-a-programar-desde-cero) by students of 4Geeks Academy [Coding Bootcamp](https://4geeksacademy.com/us/coding-bootcamp) conducted by [Alejandro Sánchez](https://twitter.com/alesanchezr) and many other contributors. Learn more about our [Programming Courses](https://4geeksacademy.com/es/curso-de-programacion-desde-cero?lang=es) to become a [Full Stack Developer](https://4geeksacademy.com/es/coding-bootcamps/desarrollador-full-stack/?lang=es), or our [Data Science Bootcamp](https://4geeksacademy.com/es/coding-bootcamps/curso-datascience-machine-learning).
