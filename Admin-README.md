# sushi-admin

> sushi-admin this code is from sushi e-learning system with model integration
> we use ReactJS library for dom manipulation and for client side rendering
> this project support japanese language and english

## System Design

> our pattern inspired from MVP(Model View Presenter) pattern, but we don't have model class instead we use javascript Object to represent the data

## Concept

* Domain - domain or entities is the specific Object Model in our Application
* UseCase - the specific task in domain that we execute in Presenter
* View - the view is our Component Class Page JS don't have concept of interface so our view directly inject to our
  Presenter
* Presenter - all custom logic before we execute the use-case are here

## Folder Structure

we use flat directory structure as possible

* pages - all Class Page store here
* components - all our custom component not in sushi-component are here
* domain - all use-cases are here

## Modules

* BasePage - all Page are extend to this class all common functionality of all pages are here.
* AppContext - we use this class for global state
* Functions - all other custom function is in src folder

## Technologies Used

- react - version 18.1.0 - for dom manipulation -> [repository](https://github.com/facebook/react)
- i18next - version 21.9.1 - use for translation -> [repository](https://github.com/i18next/i18next)
- papaparse - version 5.3.2 - use for CSV export -> [repository](https://github.com/mholt/PapaParse)
- react-router-dom - version 6.3.0 - use for routing -> [repository](https://github.com/remix-run/react-router)
- nginx - version 1.21.1 - for deployment -> [repository](https://github.com/nginx/nginx)
- docker - version 20.10.14 - use in deployment [repository](https://github.com/docker)

## Recommended Hardware

* ubuntu 18
* minimum of 25gb storage
* minimum of 1gb ram
* minimum of 1 CPU

## Maintenance

to deploy this system in production we use nginx in docker environment
first build the code 
```
yarn build
```
after code is built you can use git to push your build folder to your repository
```
# add all changes
git add .
# commit your release
git commit -m "publish"
# push to the repository
git push
```
after you login to your server you can pull your changes 
```
# goto your project folder
cd sushi-admin
# pull your changes
git pull
# run docker
docker-compose up
```

## Troubleshooting and debugging
* clear cache - clear cache your browser if the changes from the server not reflected
* check API - if there's the system is not responding check the API if its running


## Installation

first clone this package

```
git clone https://repository.git
```

then goto the folder

```
cd sushi-admin
```

install all dependency

```
yarn install
```

run all local link

```
yarn run link
```

start local development

```
yarn start
```

## reference

* [ReactJS Docs](https://reactjs.org/docs/getting-started.html)

