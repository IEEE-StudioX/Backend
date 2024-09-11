# Laravel API V11

This project is a backend API built using Laravel. It contains user authentication routes, profile management, and more.

## installation

```
 clone https://github.com/IEEE-StudioX/Backend.git
 cd Backend
```

```
    composer install
```
```
    php artisan migrate --seed
```
```
    php artisan key:generate
```
```
    php artisan key:generate
```


**Test the Project With Postman**:
 `http://127.0.0.1:8000/api`

## Backend: Laravel API
### Login Routes

| Type | URL | Accepts |
|------|------|---------|
| POST | `/api/register` | `name`, `email`, `password`, `password_confirmation` |
| POST | `/api/login` | `email`, `password` |
| POST | `/api/logout` | Add the Token |
| POST | `/api/forgot-password` | `email` |

### Profile Routes

| Method | URL | Description | Accepts |
|--------|-----|-------------|---------|
| POST | `/api/profile/update-name` | Update User Names | `name` |
| POST | `/api/profile/update-password` | Update User Password | `old_password`, `password`, `password_confirmation` |



### Libraries and Technologies

#### Core Technologies
- Laravel
- Laravel Sunctum 
- Laravel Spite Permsions 

### Project Folder Structure

```plaintext
app/                     # Core application code including controllers, models, and services
├── Http/                # Controllers, middleware, and form requests
│   ├── Controllers/     # All API controllers for handling requests
│   └── Middleware/      # Middleware for handling requests like auth checks
├── Models/              # Eloquent models
bootstrap/               # Laravel bootstrap files
config/                  # Application configuration files (e.g., database, auth, services)
database/                # Migrations, seeds, and factories
├── migrations/          # Database table migrations
├── seeds/               # Database seeders for populating tables
public/                  # Publicly accessible files (e.g., assets, index.php)
resources/               # Blade templates, language files, and raw assets (CSS, JS, images)
routes/                  # Route definitions (web.php, api.php)
storage/                 # Logs, compiled Blade templates, file-based cache
tests/                   # Unit and feature tests
vendor/                  # Composer dependencies
```

## Backend Developed By:
- [Ibrahim Elshorbagy](https://github.com/ibrahim-elshorbagy)
- [Amera Mahmoud](https://github.com/Ameramahmoud22)
