# sushi-api

> sushi-api this code is from sushi e-learning system with model integration
> this code is the backend of the project
> the core functionality of this platform is more on database manipulation or CRUD (Create,Read,Update,Delete)
> we use Nodejs to run this API

## System Design

> we use schema base to shape the data before we insert into database
> the concept is inspired in Parse Platform and Mongoose

## Concept

* Domain - domain or entities is the specific Object Model in our Application
* UseCase - the specific task in domain that we execute
* Routers - all endpoint of our API are here

## Folder Structure

we use flat directory structure as possible

* adapters - all library we use are here
* controllers - all costume functionality of the API are here
* domain - all use-cases are here

## Modules

* Auth - this class handle the user authentication and authorization
* Config - this class handle the configuration of our backend API

## Technologies Used

- nodejs - version 16.16.0 - the runtime environment to run JavaScript as backend API
- express - version 4.18.1 - the framework we in routing and to parse JSON data
- mongodb - version 4.8.0 - the database we use

## Installation

first clone this package

```
git clone https://repository.git
```

then goto the folder

```
cd sushi-api
```

install all dependency

```
npm install
```


start local development

```
npm start
```

## reference

* [NodeJS Docs](https://nodejs.org/en/docs/)

