<p align="left">
	<img src="https://telegra.ph/file/c09a3d241eef1856b910c.jpg" width="35%" style="margin-left: auto;margin-right: auto;display: block;">
</p>
<h1 align="left">Haruno Bot</h1>

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/FadliDarmawan/natsukawa)

[![Run on Repl.it](https://repl.it/badge/github/FadliDarmawan/natsukawa)](https://repl.it/github/FadliDarmawan/natsukawa)

# Natsukawa
Natsukawa bot adalah versi simple dari Haruno Bot, Natsukawa dan Haruno bot bergerak di bahasa Nodejs dan menggunakan base Nurutomo/wabot-aq.
Natsukawa bot dapat dijalankan pada: replit, heroku, termux, RDP/VPS/windows, dan mungkin lainnya.

Natsukawa saya rancang untuk hanya fitur yang common use atau sering terpakai seperti downloader, brainly, translate dll.

# Termux
```
apt install ffmpeg
apt install imagemagick
apt install nodejs
apt install git
git clone https://github.com/FadliDarmawan/natsukawa
cd natsukawa
npm i
node . (option)
````

# RDP/VPS/Windows
* Unduh & Instal Git [`Klik Disini`](https://git-scm.com/downloads)
* Unduh & Instal NodeJS [`Klik Disini`](https://nodejs.org/en/download)
* Unduh & Instal FFmpeg [`Klik Disini`](https://ffmpeg.org/download.html) (**Jangan Lupa Tambahkan FFmpeg ke variabel lingkungan PATH**)
* Unduh & Instal ImageMagick [`Klik Disini`](https://imagemagick.org/script/download.php)
```
git clone https://github.com/FadliDarmawan/natsukawa
cd natsukawa
npm i
node . (option)
```
# Replit
[![Run on Repl.it](https://repl.it/badge/github/FadliDarmawan/natsukawa)](https://repl.it/github/FadliDarmawan/natsukawa)
* Klik button
* Buka console
```
npm i
node . (option)
```
# Heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/FadliDarmawan/natsukawa)

*install buildpack
* heroku/nodejs
* https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.git
* https://github.com/DuckyTeam/heroku-buildpack-imagemagick.git

# Option

## Arguments `node . [--options] [<session name>]`

#### Contoh: `node . --self --restrict --autoread`

### `--self`

Aktifkan mode self (Mengabaikan yang lain)

### `--prefix <prefixes>`

* `prefixes` dipisahkan oleh masing-masing karakter
Setel awalan

### `--server`

Digunakan untuk [heroku](https://heroku.com/) atau pindai melalui situs web

### `--db <json-server-url>`

Gunakan db eksternal alih-alih db lokal, 
Contoh Server `https://json-server.nurutomo.repl.co/`
Code: `https://repl.it/@Nurutomo/json-server`

`node . --db 'https://json-server.nurutomo.repl.co/'`

Server harus memiliki spesifikasi seperti ini

#### GET

```http
GET /
Accept: application/json
```

#### POST

```http
POST /
Content-Type: application/json

{
 data: {}
}
```

### `--big-qr`

Jika qr unicode kecil tidak mendukung

### `--restrict`

Mengaktifkan plugin terbatas (yang dapat menyebabkan nomor Anda **diblokir** jika digunakan terlalu sering)

* Administrasi Grup `add, kick, promote, demote`

### `--img`

Aktifkan pemeriksa gambar melalui terminal

### `--autoread`

Jika diaktifkan, semua pesan masuk akan ditandai sebagai telah dibaca

### `--nyimak`

Tidak ada bot, cukup cetak pesan yang diterima dan tambahkan pengguna ke database

### `--test`

**Development** Testing Mode

### `--trace`

```js
conn.logger.level = 'trace'
```

### `--debug`

```js
conn.logger.level = 'debug'
```
