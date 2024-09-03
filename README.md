# vrom
This is a template for initiating this project using Laravel and Jetstream

## Project Setup
### 1. Initiate Project
```shell
composer create-project laravel/laravel:^9.0 vrom
```

### 2. Navigate to the Project Directory
```shell
cd vrom
composer require laravel/jetstream:^2.0
php artisan jetstream:install livewire
npm install
npm run build
```

### 3. Specify the Database Name in the `.env` File and Create it in the Target Database
### 4. Migrate Database
```shell
php artisan migrate
```

### 5. Copy Jetstream Files to Enable Customization
```shell
php artisan vendor:publish --tag=jetstream-views
```

### 6. You Can Now Launch the Project

## Project Build
### 1. Make Migrations
#### create table
To create a new migration for a table, use the following command:
```shell
php artisan make:migration create_examples_table --create="examples"
```

#### edit table 
To create a migration for modifying an existing table, use:
```shell
php artisan make:migration add_feature_field_to_example_table --table="examples"
```

#### run migration
To apply the migrations and update the database schema, execute:
```shell
php artisan migrate
```
