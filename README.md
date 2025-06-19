
# Node PostgreSQL typeORM

## Tech Stack

**Server:** Node, Express

**DataBase:** postgreSQL, typeOrm


## Run Locally

Clone the project

```bash
  git clone https://github.com/RameshPrabakar/node-typescript-typeorm
```

Go to the project directory

```bash
  cd node-typescript-typeorm
```

Install dependencies

```bash
  npm install
```

Start the tsc

```bash
  npm run watch
```

Start the server

```bash
  npm run dev
```


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`PORT`

`TOKEN_SECRET`

`REFRESH_TOKEN_SECRET`



## Documentation
`typeORM Configuration`
```
{
    "description": "TypeORM configuration file for a Node.js project using PostgreSQL as the database. This configuration specifies connection details, enables automatic schema synchronization, logging, and sets up paths for entities and CLI operations.",
    "fields": {
        "type": "Specifies the database type. Here, 'postgres' indicates PostgreSQL.",
        "host": "The hostname of the database server. 'localhost' refers to the local machine.",
        "port": "The port number on which the database server is running. Default for PostgreSQL is 5432.",
        "username": "The username used to connect to the database.",
        "password": "The password used to connect to the database.",
        "database": "The name of the database to connect to.",
        "synchronize": "If true, TypeORM will automatically synchronize the database schema with the entities each time the application runs. Not recommended for production.",
        "logging": "Enables logging of database queries and errors.",
        "entities": "An array of paths to the compiled entity files. Here, it points to all JavaScript files in the 'dist/entity' directory.",
        "migrations": "An array specifying migration files. Empty in this configuration.",
        "subscribers": "An array specifying subscriber files. Empty in this configuration.",
        "cli": {
            "entitiesDir": "Specifies the directory where new entity files will be created when using the TypeORM CLI."
        }
    }
}
```

## API Reference

#### Create user

```http
  POST /user/create
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `firstName`      | `string` | **Required**. Your API key |
| `lastName`      | `string` | **Required**. Your API key |
| `email`      | `string` | **Required**. Your API key |
| `password`      | `string` | **Required**. Your API key |
| `phoneNumber`      | `number` | **Required**. Your API key |

#### login user

```http
  POST /user/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `phoneNumber`      | `number` | **Required**. Your API key |
| `password`      | `string` | **Required**. Your API key |


#### Get all users

```http
  GET /user/list
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `uuid` | **Required**. Your API key |
| `firstName` | `string` | **Required**. Your API key |
| `lastName` | `string` | **Required**. Your API key |
| `email` | `string` | **Required**. Your API key |
| `password` | `string` | **Required**. Your API key |
| `profileImage` | `string` | **Required**. Your API key |
| `isActive` | `boolean` | **Required**. Your API key |
| `phoneNumber` | `number` | **Required**. Your API key |
| `tocken` | `string` | **Required**. Your API key |
| `refreshToken` | `string` | **Required**. Your API key |

A postman collection has been added for better understanding.


## Author

- [@RameshPrabhakar](https://www.github.com/RameshPrabakar)

