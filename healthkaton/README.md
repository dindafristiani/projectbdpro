## Tentang SIDESPIN

Sistem Informasi Desa Pintar (SIDESPIN) merupakan sistem yang digagas untuk mempercepat pembangunanan teknologi di daerah-daerah dengan potensi desa, salah satunya dalam hal digitalisasi desa. dan menyajikan informasi secara riil, seperti geografi desa, demografi penduduk desa dan lain sebagainya.

SIDESPIN dibangun menggunakan beberapa teknologi berikut:

- Framework [Laravel](https://laravel.com/) dan [Vue.JS](https://vuejs.org/).
- Authentication menggunakan [Laravel UI](https://github.com/laravel/ui).
- Design website menggunakan Framework [Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/introduction/) v5.
- Template CMS menggunakan [AdminLTE 3](https://adminlte.io/).
- Hak akses dan Level User menggunakan [Spatie Laravel Permission](https://github.com/spatie/laravel-permission).
- Manipulasi gambar pada website menggunakan [Image Intervension](http://image.intervention.io/).
- Data table menggunakan [Yajra DataTables](https://datatables.yajrabox.com/).

### Instalasi
Instal [Composer](https://getcomposer.org/) pada Sistem Operasi agar perintah artisan dapat dijalankan. Masuk ke folder <i>root</i> aplikasi dan jalankan perintah instal pada terminal untuk download vendor yang dibutuhkan.

```javascript
//Download vendor untuk aplikasi
composer install
```

Jalankan perintah berikut untuk <i>copy</i> file `.env`, atau bisa juga <i>copy</i> secara manual. Sesuaikan pengaturan <i>database</i> dengan lokal sistem anda pada file `.env` ini.

```javascript
cp .env.example .env
```

Jalankan perintah artisan untuk generate enkripsi kunci keamanan aplikasi.

```javascript
//Generate key baru
php artisan key:generate
```

Jalankan perintah artisan migration dan seeder pada terminal untuk membuat <i>database</i> dan pengguna.

```javascript
//Generate database baru dan user default
php artisan migrate --seed

```

Jalankan artisan serve pada terminal untuk jalankan server default laravel.

```javascript
//Local server default laravel
php artisan serve

```

### User Default Akses

```javascript
//Email login
superadmin@email.com

//Pass login
12345678
```