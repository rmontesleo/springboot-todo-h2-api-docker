# Springboot TODO API with H2 as Database and Docker (springboot-todo-h2-api-docker)

This is CRUD (Create Read Update Delete) application using Java with Springboot and save the data in a H2 database.
This is an basic sample to start using the mentioned tools. After create the API, this will be move to a container.

I hope this project helps you to build something big, something better.

## Install the application

### Prerequisite

- Have installed Java 17 or above
- Have installed Maven 3.8.5 or above
- You cand use your favorite IDE or Text Editor . This project was tested with IntelliJ IDEA and VSCode
- git 2.25.1 or above
- Have Installed some browser like Chrome, Firefox or Microsoft Edge


### Clonning the project

The project is hosted on GitHub, on the repository [springboot-todo-h2-api-docker](https://github.com/rmontesleo/springboot-todo-h2-api-docker)

```bash
git clone https://github.com/rmontesleo/springboot-todo-h2-api-docker.git
```

Go to the folder project
```bash
cd springboot-todo-h2-api-docker
```

## Run the project


### Build the jar with maven
```bash
springboot-todo-h2-api-docker $  mvn clean package
```

### Run the jar
```bash
springboot-todo-h2-api-docker $  java -jar target/springboot-todo-h2-api.jar
```


## Operate the project

The project is a REST API, with two endponts

- [Users](http://localhost:8080/api/todoapp/users) : With the operations to Signup, login, get all users and get user by id.
- [Todos](http://localhost:8080/api/todoapp/todos) : Whith the CRUD TODO operations for a register user


### Test with Swagger

Open the URL http://localhost:8080/api/todoapp/swagger-ui/index.html in your browser

More details of how test/execute the api go to [TEST API](DOCS/TEST_API.md)


### Test the data base.

The H2 dependency also generate a web console to execute queries to your database. You can open the console in http://localhost:8080/api/todoapp/h2-console/login.jsp .  This console is open when you run with VSCode or IntelliJ IDEA

Mode details of how test/execute operations on the database [TEST DATABASE](DOCS/TEST_DATABASE.md)


## Next steps

- [rmontesleo/springboot-todo-h2-api-jib](https://github.com/rmontesleo/springboot-todo-h2-api-jib) : The API using jib to create the containers

## Previous steps
- [rmontesleo/springboot-todo-h2-api](https://github.com/rmontesleo/springboot-todo-h2-api) : The Basic version of the API


## Other resources to see



## Project Licence

The project uses the MIT license. You can check [here](LICENSE)


## Additional information

Some additional documents where added to get more information, details of some topic or solutions of some issues.

- [CONFIGURATION](DOCS/CONFIGURATION.md) : Configuration JAVA_HOME, MVN_HOME and other related configurations

- [TEST API](DOCS/TEST_API.md) : Details of how operate you api with Swagger and curl

- [TEST Database](DOCS/TEST_DATABASE.md) : Details of how operate you database

- [Container Operations](DOCS/BUILD_CONTAINER.md): Create the image, run container, tag the image, push to Docker Hub.

- [Using Compose](DOCS/COMPOSE.md): Configurations and commands to execute the compose.

- [REFERENCES](DOCS/REFERENCES.md) : With information of the topics used in this project like Java 8, Swagger, Cors, Lombox, Records, etc.

- [SOLVING ERRORS](DOCS/SOLVING_ERRORS.md) : Solutions to some errors, issues, presented in this project

