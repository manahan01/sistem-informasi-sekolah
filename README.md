# Project
 Aplikasi back-end sistem informasi penilaian sekolah menggunakan framework laravel dan mongoDB.

# Instalasi
1. Buka direktori project di terminal anda.
2. Ketik command : copy .env.example .env (copas di terminal).
3. Ketik command dibawah ini:
	- composer install
	- php artisan optimize:clear
	- php artisan key:generate
4. Periksa kembali setting mongoDB apa sudah sesuai atau belum:
  - Periksa providers di config/app.php (Jenssegers\Mongodb\MongodbServiceProvider::class,)
  - Periksa database mongoDB apakah sudah terdaftar di config/database.php 
  - Periksa environment (.env) apakah sudah menggunakan database mongoDB
5. Instal dan lakukan regis pada postman desktop
6. Ketik command dibawah ini:
    - php artisan migrate (migrasi database)
    - php artisan db:seed
    - php artisan serve
7. Terakhir, masukkan request api http://127.0.0.1:8000/api/{sesuai-action-yang-tertera} dan methodnya.
