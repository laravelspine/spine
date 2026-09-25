# Spine — Minimal Laravel Consumer

## Overview

Spine adalah aplikasi minimal yang mengonsumi `spine/laravel-spine` package. Berfungsi sebagai proof-of-concept bahwa package dapat diintegrasikan ke aplikasi Laravel biasa.

## Tech Stack

| Layer | Technology |
|-------|------------|
| Framework | Laravel 12 |
| Package | spine/laravel-spine |
| Auth | Laravel Sanctum |
| Database | MySQL |

## Purpose

- Demonstrasi integrasi `spine/laravel-spine` package ke aplikasi Laravel baru
- Konsumen minimal dengan routing, middleware, dan auth yang dikonfigurasi
- Tidak memiliki fitur bisnis (CRM, Customer, dll) — murni untuk testing package

## Features

- ✅ Auth login/logout dengan Sanctum
- ✅ Auth middleware configured
- ✅ API routes prefix `/api/v1`
- ✅ Public content API
- ✅ Menu registry endpoints
- ✅ Translation controller

## Installation

```bash
cd /www/wwwroot/spine.lan
composer install
npm install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan rbac:sync-core
```

## Database

- Host: `127.0.0.1:3306`
- Database: `spine`
- User: `spine`
- Password: `spine_dev_2026`

## GitHub

- Repo: https://github.com/laravelspine/spine (public)
