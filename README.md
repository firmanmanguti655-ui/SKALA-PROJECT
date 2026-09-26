# Web Peta Wisata Rancabali

Website informasi dan peta digital destinasi wisata Rancabali berdasarkan proposal proyek.

## Destinasi awal
- Kawah Putih
- Situ Patenggang

## Fitur MVP
- Beranda dan daftar wisata
- Pencarian wisata
- Detail wisata
- Peta digital dan koordinat
- Link Google Maps
- Login admin
- Dashboard admin
- CRUD data wisata

## Teknologi
- Laravel / PHP
- MySQL
- Blade, HTML, CSS, JavaScript
- Leaflet + OpenStreetMap untuk peta

## Instalasi
```bash
git clone <URL-REPOSITORY>
cd web-peta-wisata-rancabali
composer install
copy .env.example .env
php artisan key:generate
```

Buat database MySQL, lalu isi `.env`:
```env
DB_DATABASE=wisata_rancabali
DB_USERNAME=root
DB_PASSWORD=
```

Jalankan:
```bash
php artisan migrate --seed
php artisan serve
```

Buka `http://127.0.0.1:8000`.

### Akun admin demo
- Email: `admin@rancabali.test`
- Password: `password`

## Struktur
- `app/Models` — model database
- `app/Http/Controllers` — controller pengunjung/admin
- `database/migrations` — struktur tabel
- `database/seeders` — data awal Kawah Putih dan Situ Patenggang
- `resources/views` — tampilan Blade
- `routes/web.php` — routing
- `public/css` — stylesheet
- `public/js` — JavaScript peta
- `docs` — dokumentasi proyek

## Catatan
Repository ini mengikuti scope proposal. Fitur pembayaran, booking hotel, marketplace, aplikasi mobile native, dan transaksi keuangan tidak termasuk MVP.
