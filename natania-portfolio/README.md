# Natania Portfolio

Website portofolio pribadi dengan gaya playful dan modern, memakai palet pastel pink, biru, dan ungu.

## Struktur folder

```text
natania-portfolio/
├── index.html
├── style.css
├── script.js
└── README.md
```

## Cara menjalankan di VS Code

1. Ekstrak ZIP ini ke folder yang mudah ditemukan.
2. Buka VS Code.
3. Pilih **File → Open Folder...**, lalu pilih folder `natania-portfolio`.
4. Buka `index.html`.
5. Jika ekstensi **Live Server** sudah terpasang, klik kanan `index.html` lalu pilih **Open with Live Server**.
6. Website akan terbuka di browser. Setelah mengubah kode, simpan dengan **Ctrl + S** lalu muat ulang browser bila perlu.

Alternatif: klik dua kali `index.html` di File Explorer untuk membukanya langsung di browser. Live Server lebih nyaman untuk proses pengembangan.

## Cara mengganti placeholder foto

Saat ini foto masih berupa placeholder desain, jadi tidak ada file foto yang perlu disiapkan.

Untuk menambahkan foto sendiri:
1. Buat folder bernama `assets` di dalam folder proyek.
2. Salin foto ke folder `assets`, misalnya dengan nama `foto-natania.jpeg`.
3. Di `index.html`, cari blok `<div class="photo-placeholder"> ... </div>`.
4. Ganti seluruh blok itu dengan:

```html
<div class="photo-placeholder">
  <img
    src="assets/foto-natania.jpeg"
    alt="Foto profil Natania"
    class="profile-photo"
  >
</div>
```

5. Tambahkan aturan berikut ke bagian paling bawah `style.css`:

```css
.profile-photo {
  display: block;
  width: 100%;
  height: 330px;
  object-fit: cover;
  border-radius: 19px;
}
```

Pastikan ejaan nama file dan ekstensi pada `src` sama persis dengan nama file sebenarnya. `.jpeg` dan `.jpg` sama-sama bisa digunakan, selama nama di kode sesuai.

## Konten yang bisa disunting

- Data diri ada di bagian **About me** dalam `index.html`.
- Area **What I can do** adalah contoh area belajar yang bisa disesuaikan dengan kemampuan nyata.
- **Achievement** berisi proyek portofolio ini dan tempat untuk menambahkan pencapaian yang sudah benar-benar dimiliki.
- Email dan LinkedIn sudah diisi sesuai detail yang diberikan.
- Warna, ukuran, layout, dan responsivitas diatur dalam `style.css`.
- Menu mobile, animasi saat scroll, dan tahun footer diatur dalam `script.js`.

## Catatan

- Email menggunakan tautan `mailto:`. Saat diklik, perangkat akan membuka aplikasi email yang dikonfigurasi.
- Tautan LinkedIn akan terbuka di tab baru.
- Google Fonts memerlukan koneksi internet untuk memuat font pilihan; jika offline, website tetap berjalan dengan font cadangan.
- Website ini belum dipublikasikan ke internet. Untuk dibuka orang lain melalui tautan publik, perlu layanan hosting seperti GitHub Pages.
