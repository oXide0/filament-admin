# Laravel Filament Demo (Produkty & Kategórie)

## Požiadavky

- PHP 8.4+
- Composer
- Node.js (kvôli buildovaniu assetov)

## Inštalácia

1. Klonuj projekt a nainštaluj závislosti:
   ```
   git clone ...
   cd ...
   composer install
   cp .env.example .env
   php artisan key:generate
   ```

2. Nastav .env (DB prístup, APP_URL)

3. Migrácie:
   ```
   php artisan migrate
   ```

4. Buildni frontendy (ak treba):
   ```
   npm install && npm run build
   ```

5. Admin credentials:
    ```
   php artisan db:seed
   ```   
   Credentials:
    ```
   test@example.com
   password
   ```

6. Spusti server:
   ```
   php artisan serve
   ```

7. Admin rozhranie je na [http://localhost:8000/admin](http://localhost:8000/admin)

## Bonusy

- SoftDeletes pri produktoch a kategóriách
- Prepínanie aktivity priamo v tabuľke
- Výber kategórií iba z aktívnych
- Admin rozhranie v slovenčine
- Časová zóna Europe/Bratislava
