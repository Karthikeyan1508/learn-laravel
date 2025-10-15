# Laravel Application Setup Guide

This document provides step-by-step instructions for setting up and running a Laravel application on your local machine. It follows the standard Laravel installation process and assumes no prior setup.

---

## 1. Overview

Laravel is a modern PHP framework designed for simplicity, scalability, and developer productivity.
This guide will help you:

* Install Laravel and its dependencies
* Create a new Laravel project
* Understand the project structure
* Run the development server

---

## 2. Prerequisites

Before starting, ensure you have the following installed on your system:

* PHP (version 8.1 or higher)
* Composer (dependency manager for PHP)
* Node.js and npm (for frontend assets)
* Git (recommended for version control)

To verify installation:

```bash
php -v
composer -V
node -v
npm -v
git --version
```

For a graphical PHP management experience, you may use [Laravel Herd](https://herd.laravel.com/).

---

## 3. Install Laravel

Visit the [official Laravel installation guide](https://laravel.com/docs/installation) and follow the instructions for your operating system.

If you already have PHP and Composer installed, you can install the Laravel installer globally using:

```bash
composer global require laravel/installer
```

After installation, restart your terminal session to ensure all commands are available globally.

Verify installation:

```bash
laravel -v
```

---

## 4. Create a New Laravel Application

Once Laravel is installed, create a new project using the following command:

```bash
laravel new chirper
```

During setup, select the following options when prompted:

| Option            | Selection |
| ----------------- | --------- |
| Starter Kit       | None      |
| Testing Framework | Default   |
| Database          | SQLite    |
| Run npm install   | Yes       |

After installation completes, navigate into the project directory:

```bash
cd chirper
```

---

## 5. Set Up Your Editor

You can use any text editor or IDE. Popular choices include:

* **VS Code** – Lightweight with excellent Laravel support through official extensions.
* **Cursor** – A VS Code variant with AI-assisted capabilities.
* **PHPStorm** – Full-featured IDE with Laravel integration via the Laravel Idea plugin.

Install a Laravel extension in your editor for syntax highlighting, Blade support, and route navigation.

---

## 6. Explore the Project Structure

A newly created Laravel project includes several key directories:

| Directory          | Description                                                          |
| ------------------ | -------------------------------------------------------------------- |
| `app/`             | Contains core application code such as models and controllers.       |
| `resources/views/` | Contains Blade templates used for rendering HTML views.              |
| `routes/`          | Defines application routes that map URLs to actions.                 |
| `database/`        | Contains database migrations, seeders, and the SQLite database file. |

---

## 7. Run the Application

To start the development server, run:

```bash
composer run dev
```

This command initializes the Laravel development server and the Vite server for frontend assets.

Once running, open the application in your browser:

```
http://localhost:8000
```

If the Laravel welcome page appears, your setup is complete.

---

## 8. Next Steps

After confirming the application is running, you can proceed to:

* Create your first route and Blade view.
* Define application logic within controllers.
* Explore database migrations and Eloquent ORM.

---

## 9. Quick Reference

| Step            | Command                                     |
| --------------- | ------------------------------------------- |
| Install Laravel | `composer global require laravel/installer` |
| Create project  | `laravel new chirper`                       |
| Enter directory | `cd chirper`                                |
| Start server    | `composer run dev`                          |
| Access app      | `http://localhost:8000`                     |

---
