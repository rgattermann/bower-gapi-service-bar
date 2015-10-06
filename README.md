# Grupo API Service Bar

> Application Header bar with Notifications, Contracted Applications and User Configuration

![services-bar](http://s23.postimg.org/tbzd2mo3v/bar.gif)

## Mirrors

* Development instance at: [lost-panther]()
* QA(homolog) instance at: [internal only]()

## Developing at gapi-service-bar

> gapi-service-bar is a AngularJS Application built to make easier to change application accesses and user configuration of the GAPI Customers.

> More about on the [Wiki](https://github.com/grupoapi/gapi-service-bar/wiki) page.

### Configuring development environment

#### Step 1: installing tools

* install git: [git-scm](http://git-scm.com/)
* install NodeJS: [nodejs.org](http://nodejs.org)

#### Step 2: preparing repository

Clone repository:
```
git clone https:/github.com/grupoapi/gapi-service-bar
```

Install dependency packages
``` sh
cd gapi-service-bar
npm install
bower install
```

### Step 3: build it to generate 'demo' dependencies

To build Just type:
``` sh
gulp
```

### Step 4: How to get fun

``` sh
gulp dev
```

**Browse it** : ```localhost:7777/```

### Adding to your project

Firstly you must have bower already installed to run this command:
```sh
bower install gapi-service-bar --save
```

Add it to your AngularJS Module as AngularJS dependency:
``` javascript
angular.module('yourProject', ['gapiServiceBar'];
```

Include the directive on your HTML:
``` html
<gapi-service-bar></gapi-service-bar>
```
--
### Customization

To cover all functionalities peacefully you must observe the following [angularjs broadcast](https://docs.angularjs.org/api/ng/type/$rootScope.Scope) events:

* **GAPI-SERVICE-BAR-LOGOUT**  - When logout.
* **GAPI-SERVICE-BAR-ISLOADING**  - When the Service Bar is loading, it passes an boolean.

--

### Development style guide

The project pattern follows is based on consolidated best practices. That means:
* there is a Continuous Integration system;
* there is a static code analysis tool;
* the repository flow is simple: [Git flow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow) do the job;
* JSLint and JSHint checks are part of the build process;
