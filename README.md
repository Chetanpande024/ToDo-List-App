# ToDo List App

Todo list web app built with [ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-3.1),
[ReactJS](https://reactjs.org/) and "EntityFrameworkCore InMemory" Database.

## Technologies
-   Backend
    -   [ASP NET Core](https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-3.1): Cross-platform framework to build web apps
    -   EntityFrameworkCore InMemory Database: Microsoft EntityFrameworkCore InMemory Database
-   Tests
        -   [xUnit](https://xunit.net/): Unit testing tool for the .NET
        -   [Fluent Assertions](https://fluentassertions.com/): Fluent API for asserting the results of unit tests
        -   [Moq](https://github.com/moq/moq): Mocking framework for .NET
-   Frontend
    -   [ReactJS](https://reactjs.org/): JavaScript library for building user interfaces
    -   [Typescript](https://www.typescriptlang.org/): Typed superset of JavaScript
    -   [React Router DOM](https://reacttraining.com/react-router/web/guides/quick-start): Declarative routing for React
-   [Docker](https://www.docker.com/): Platform to build, run, and share applications with containers.

# Getting started

### Download ToDo-List.zip file and extract it.

Then use Package Manager Console/VS Code Terminal/Powershell to change directory to extract folder 'ToDo-List'

```
cd ToDo-List
```

### Run without docker

Requires

-   [SQL SERVER](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
-   [.NET Core 3.1 SDK](https://dotnet.microsoft.com/download)
-   [NodeJS](https://nodejs.org/en/)

**Run the Web Api**

First, restore dependencies

```bash
$ dotnet restore
```

To run the tests

```
$ dotnet test
```

Then, run the project with with

```bash
$ dotnet run --project src/TodoList.WebApi
```

**Run the React app**

Change directory to '..\ToDo-List\src\todo-list-spa' folder

```
cd ToDo-List\src\todo-list-spa
```

```bash
# Install dependencies
$ npm install

# Starting the project
$ npm start
```
ASP.NET Core API will be available in `http://localhost:5000`
ReactJS app will be available in `http://localhost:3000`

### Run with docker

Requires

-   [Docker](https://docs.docker.com/get-docker/)
-   [Docker compose](https://docs.docker.com/compose/install/)

Run the following command to start backend and frontend

```
docker-compose up -d
```
ASP.NET Core API will be available in `http://localhost:5000`
ReactJS app will be available in `http://localhost:3000`

To stop the application run

```
docker-compose down
```
