# Table of contents
1. [Project Abstract](#introduction)
2. [Team Roles](#team)
3. [Project](#bookmarks) 
    1. [Backlog](#backlog)
    3. [API](#api)
    4. [CI/CD](#ci_cd)
    5. [Code Quality](#quality)
    6. [Production Environment](#prod_env)
    7. [Deployments](#deploy)
4. [Repositories](#reps) 
    1. [We_Deliver-Backend](#weDel-back)
    2. [We_Deliver-Frontend-Rider](#weDel-frider)
    3. [We_Deliver-Frontend-Admin](#weDel-fadmin)
    4. [DrinkUp-Backend](#drink-back)
    5. [DrinkUp-Frontend](#drink-front)

## Project Abstract <a name="introduction"></a>
The *WeDeliver* application is a riders platform with the main objective of providing an infrastructure that allows stores to use it for the deliveries of their products.

The client side application is a drinks store, *DrinkUp*, that delivers their items using the *WeDeliver* platform.


## Team Roles <a name="team"></a>
The team has 5 elements:
- **Rui Fernandes** - Team Leader, Developer
- **Inês Leite** - Product Owner, Developer
- **Orlando Macedo** - QA Engineer, Developer
- **Óscar Fernandez** - QA Engineer, Developer
- **Pedro Marques** - DevOps Master, Developer

## Project <a name="bookmarks"></a>

### Backlog <a name="backlog"></a>
The Backlog management tool we are using is PivotalTracker for the [*WeDeliver* platform](https://www.pivotaltracker.com/n/projects/2500281) and for the [*DrinkUp* platform](https://www.pivotaltracker.com/n/projects/2500453) using Pivotal Workflow, passing through all the stages ("Write stories", "Prioritize stories", "Estimate stories", "Start stories", "Finish and deliver stories", "Test stories", "Accept or reject stories" and "Stories move to the Done panel").

### API <a name="api"></a>
We have 2 sets of API's, one for *WeDeliver* and another for *DrinkUp*. The first one has 4 groups of API's, for the customer and riders and for the orders and admin page. *DrinkUp* has 3 groups of API's for the users, the items and the orders.

[Swagger for *WeDeliver*](https://webmarket-314811.oa.r.appspot.com/swagger-ui/index.html?configUrl=%2Fapi-docs%2Fswagger-config#/)

[Swagger for *DrinkUp*](http://drinkup-316817.oa.r.appspot.com/swagger-ui/index.html?configUrl=/api-docs/swagger-config)

### CI/CD <a name="ci_cd"></a>
In order to continually test our deployments, each backend-related repositories for both WeDeliver and DrinkUp apps have CI/CD scripts executed on push.  

*WeDeliver* Backend
[CD](https://github.com/Tqs-project/We_Deliver-Backend/blob/dev/.github/workflows/build-cd.yaml)
[CI](https://github.com/Tqs-project/We_Deliver-Backend/blob/dev/.github/workflows/build-ci.yml)

*DrinkUp* Backend
[CD](https://github.com/Tqs-project/DrinkUp-Backend/blob/main/.github/workflows/build-cd.yaml)
[CI](https://github.com/Tqs-project/DrinkUp-Backend/blob/main/.github/workflows/build-ci.yml)

Furthermore, the rider flutter app repository also has a CI script.
*WeDeliver* MobileApp
[CI](https://github.com/Tqs-project/We_Deliver-MobileApp-Rider/blob/dev/.github/workflows/build.yml)

### Code Quality <a name="quality"></a>
In regards to static code analysis, we're using SonarCloud.
[SonarCloud Dashbord](https://sonarcloud.io/organizations/tqs-project-1/projects)

### Production Environment <a name="prod_env"></a>


### Deployments <a name="deploy"></a>
Our App is Continuously being deployed into the GoogleCloud Platform.

The *WeDeliver* admin frontend is deployed on **[https://wedeliveradmin.herokuapp.com/](https://wedeliveradmin.herokuapp.com/)** and *DrinkUp* client frontend is on **[https://drinkupstore.herokuapp.com/](https://drinkupstore.herokuapp.com/)**. Both were deployed with Heroku.

The *WeDeliver* rider app has an apk on this repo.

**Existing users:**
- Clients for *DrinkUp*:
    -  username: aux | password: aux
-  Riders for *WeDeliver*:
    -  username: Pedro | password: 1234


## Repositories <a name="reps"></a>
This project has two main applications: *WeDeliver* and *DrinkUp*. Each of them has a backend and a frontend. *WeDeliver* has two frontends, the riders application, which is in Flutter, and the admin application, which is in AngularJS. The *DrinkUp* frontend is also in AngularJS.

Giving that the project has several parts, we separated them by the following repositories:

### We_Deliver-Backend <a name="weDel-back"></a>
Has all the deliveries platform, *WeDeliver*, backend: the tables' models, it's repositories, the services and controllers for the API's and the tests for each.

Repo link: [here](https://github.com/Tqs-project/We_Deliver-Backend)

### We_Deliver-Frontend-Rider <a name="weDel-frider"></a>
Has the code for the Flutter app of the *WeDeliver* platform for the Riders. 

Repo link: [here](https://github.com/Tqs-project/We_Deliver-Frontend-Rider)

### We_Deliver-Frontend-Admin <a name="weDel-fadmin"></a>
Has the code for the AngularJS application of the *WeDeliver* platform for the admin.

Repo link: [here](https://github.com/Tqs-project/We_Deliver-MobileApp-Rider)

### DrinkUp-Backend <a name="drink-back"></a>
Has the code for the backtend of the *DrinkUp* store: the tables' models, it's repositories, the services and controllers for the API's and the tests for each.

Repo link: [here](https://github.com/Tqs-project/DrinkUp-Backend)

### DrinkUp-Frontend <a name="drink-front"></a>
Has the code for the frontend of the *DrinkUp* store.

Repo link: [here](https://github.com/Tqs-project/DrinkUp-Frontend)
