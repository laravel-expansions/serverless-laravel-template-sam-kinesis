# Serverless Laravel Template for SAM (with Kinesis)

## Technologies

- **[Laravel 8.x](https://github.com/laravel/framework/tree/8.x) - Framefork**
- **[bref](https://github.com/brefphp/bref) - PHP Runtime + Composer Package**
- **[laravel-expansions/serverless-function](https://github.com/laravel-expansions/serverless-function) - Serverless Function Expansion**

## Setup

### 1. Clone this repository
```
git clone https://github.com/laravel-expansions/serverless-laravel-template-sam-kinesis.git
```

and move laravel directory
```
cd laravel
```


### 2. Install composer packages
Pre installed additional packages
- bref/bref
- bref/laravel-bridge
- laravel-expansions/serverless-function
```
composer insttall
```

### 3. Create .env
```
cp .env.example .env && php artisan key:generate
```

## Deploy

Run SAM CLI commands
```
sam build && sam deploy --guided
```
