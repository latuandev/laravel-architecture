# README #
This is the source code architecture of Laravel version 10.x, utilizing the Repository pattern and Docker.

---

## Note for GIT
* Please help apply GitFlow for this repository (https://danielkummer.github.io/git-flow-cheatsheet).
* Example:
  - Name for any features -> `feature/xxx-yyy`. Ex: `feature/implement-login-ui`
  - Name for any bugs -> `bugfix/xxx-yyy`. Ex: `bugfix/wrong-message-when-login`

* When creating a title for a pull request or a commit message, please ensure that both the title and message are meaningful, and include a description if necessary. Capitalize the first letter and avoid using special characters.
* Example:
  - Implement the authentication feature

---

## Tech stacks
- PHP 8.2.x
- Laravel 10.x

## Your machine's prerequisites
- Docker
- Docker compose
- Node.js 20.18.x or other Node.js version

## Getting started
### Setting environment
```
cp .env.example .env
```

### Installation
```
docker-compose build
```

### Running
```
docker-compose up
```

- Host: http://localhost:8000

### Steps build
_Make sure the laravel-app service is running_

#### Start bash shell
```
docker exec -it laravel-app sh
```

#### Installation PHP's dependencies
```
composer install
```

#### Generation APP_KEY
```
php artisan key:generate
```

#### Migration DB
```
php artisan migrate
```

#### Exit bash shell
```
exit
```

### To use pre-commit
_Make sure you have Node.js installed on your machine_

#### Installation Node's modules. _(This is necessary to use pre-commit and more)_
```
npm install
```

---

## Author
* Name: Tuan Le
* Email: latuan.dev@gmail.com
