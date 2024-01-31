# Installation

## Clone the repo
```bash
git clone github.com/bayuawe/laravellunar.git example-app
```
This will create a shallow clone of the repo, from there you would just need to remove the `.git`folder and reinitialise it to make it your own.

```bash
cd exampleapp
rm -rf .git
```

Then install composer dependencies
```bash
composer install
```

## Configure the Laravel app
Copy the `.env.example` file to `.env` and make sure the details match to your install.

```bash
cp .env.example .env
```
All the relevant configuration files should be present in the repo.

## Migrate and seed
Run the migrations
```bash
php artisan migrate
```

Install Lunar
```bash
php artisan lunar:install
```

Seed the demo data.
```bash
php artisan db:seed
```

Link the storage directory
```bash
php artisan storage:link
```

# Finished 🚀
You are now installed!

- You can access the storefront at `http://<yoursite>`
- You can access the admin hub at `http://<yoursite>/hub`
