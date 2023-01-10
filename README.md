# Share Your Codes
App for publishing and sharing code snippets, like Carbon.

## Table of contents
- [Running on localhost](#🚀-running-on-localhost)
- [Features](#✨-features)

## 🚀 Running on localhost
Before getting started, make sure that you have installed:
- PHP 7.4.21;
- Node.js 17.7.1;
- Composer 2.4.4
- MySQL
- NPM 8.5.2

First of all:
```
    git clone ${insert repository}
```

### Initializing server
1. From root directory, move to server directory:
```
    cd share_your_codes_server
```

2. Install dependencies:
```
    componser install
```

3. Create a .env file from the .env.example file and setup your database:
```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_db
    DB_USERNAME=your_username
    DB_PASSWORD=your_password
```

4. Generate an app key :
```
    php artisan key:generate
```

5. Run the migrations: 
```
    php artisan migrate
```

6. Init server:
```
    php artisan serve --port=3000
```

### Initializing client
1. Install dependencies:
```
    npm install
```

2. Init client:
```
    npm run serve
```

## ✨ Features
- Sign up, sign in and sign out with JWT;
- Create, read, update and delete projects;
- Share code snippets on social medias, like twitter or whatsapp;