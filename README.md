# 📸 Laravel Social App

A simple social media-style Laravel application built with:

- Laravel 11
- Breeze (for authentication scaffolding)
- Tailwind CSS & Alpine.js (frontend)
- Email verification
- CRUD for posts and profiles
- Follow & like system
- Category filtering for posts

---

## 🚀 Features

- ✅ Authentication (via Laravel Breeze)
- ✅ Email verification
- ✅ Profile management (including profile picture upload)
- ✅ Create, update, delete posts
- ✅ Like/unlike posts
- ✅ Follow/unfollow users
- ✅ Filter posts by category

---

## 🛠️ Tech Stack

- **Backend:** Laravel 11
- **Frontend:** Tailwind CSS, Alpine.js
- **Authentication:** Laravel Breeze
- **Database:** MySQL (or compatible)
- **File Uploads:** Public disk storage (for profile pictures)

---

## 🧱 Database Tables

- `users` – Registered users
- `posts` – Posts created by users
- `categories` – Categories to organize posts
- `follows` – Pivot table for following relationships
- `likes` – Pivot table for post likes

---

## 🖼️ User Functionality

### Authentication
- Register/login
- Email verification required before full access

### Profile
- Edit name, email, bio, and profile image
- Delete account

### Posts
- Create, update, delete own posts
- Assign posts to a category
- View posts by category
- Like/unlike posts

### Social
- Follow/unfollow other users
- See follower/following counts
- View posts from followed users

---

## ⚙️ Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/laravel-social-app.git
cd laravel-social-app

# 2. Install dependencies
composer install
npm install && npm run build

# 3. Environment setup
cp .env.example .env
php artisan key:generate

# 4. Configure your database and mail settings in `.env`

# 5. Run migrations and seeders
php artisan migrate --seed

# 6. Start the server
php artisan serve
