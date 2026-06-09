# Twitter Clone

A simplified Twitter-inspired social media web application built with Laravel and MySQL. This project demonstrates the implementation of core social networking features such as user authentication, posting content, user profiles, likes, and follower relationships.

## Features

### Authentication

* User registration
* User login
* User logout
* Session-based authentication

### Posts

* Create new posts
* View posts on the home timeline
* View individual post details
* Reply/comment on posts

### Social Features

* Like and unlike posts asynchronously (AJAX)
* Follow and unfollow other users
* View follower and following information

### Profile Management

* View user profiles
* Edit profile information
* Update username, display name, email, and bio

## Technology Stack

### Backend

* PHP
* Laravel

### Frontend

* Blade Template Engine
* Bootstrap
* JavaScript
* AJAX

### Database

* MySQL

## Project Structure

```text
app/
├── Http/Controllers/
│   ├── HomeController.php
│   ├── PostsController.php
│   ├── ProfileController.php
│   ├── LikeController.php
│   ├── FollowController.php
│   ├── SignInController.php
│   └── SignUpController.php
│
├── Models/
│   ├── User.php
│   ├── Post.php
│   ├── Like.php
│   └── Follow.php
│
resources/views/
├── home.blade.php
├── profile/
├── post/
├── login/
└── register/
```

## Installation

### Prerequisites

* PHP 8.1+
* Composer
* MySQL

### Clone Repository

```bash
git clone <repository-url>
cd <project-folder>
```

### Install Dependencies

```bash
composer install
```

### Environment Configuration

Copy the environment file:

```bash
cp .env.example .env
```

Configure your MySQL database credentials inside `.env`.

Example:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=twitter_clone
DB_USERNAME=root
DB_PASSWORD=
```

### Generate Application Key

```bash
php artisan key:generate
```

### Run Database Migration

```bash
php artisan migrate
```

### Start Development Server

```bash
php artisan serve
```

The application will be available at:

```text
http://localhost:8000
```

## Learning Objectives

This project was developed to practice:

* Laravel MVC architecture
* Authentication and authorization
* Eloquent ORM relationships
* CRUD operations
* AJAX interactions
* Relational database design
* Social media application fundamentals


## License

This project was created for educational and learning purposes.

