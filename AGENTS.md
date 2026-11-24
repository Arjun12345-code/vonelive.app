# CODING AGENT RULES - BOLOUUPGO.APP

Projek ini akan dipakai untuk Wordpress Elementor HTML Element dan Site Custom CSS untuk boloupgo.app. Oleh karena itu, projek ini WAJIB mengikuti konfigurasi ini:

- Setiap page adalah HTML.
- Setiap HTML page punya Javascripnya sendiri dan WAJIB INTERNAL JAVASCRIPT di akhir <body>.
- Untuk design WAJIB pakai CSS EXTERNAL (style.css), TIDAK BOLEH CSS INTERNAL dan INLINE.
- Saat membuat Header (Nav) dan Footer, WAJIB DIBUAT HTML TERPISAH (header.html dan footer.html). Jangan satukan dengan HTML PAGE.
- Custom Font wajib dari Google Font via CSS @import.
- Mengikuti Aturan Detail dibawah ini.

## Aturan Penulisan Konten
- Jangan pernah mengubah copywriting yang diberikan user.
- Jangan menambahkan atau mengurangi apapun yang diberikan user.
- Copywriting harus 100% tepat karena sudah disesuaikan untuk SEO.

## Aturan Projek
- Pastikan struktur projeknya rapih, assets ditempatkan di tempatnya.
- Semua page HTML dan CSS ada di root (`boloupgo.app/`), jangan masukkan ke dalam sub-folder.

## Aturan HTML
- Setiap Page = 1 Full HTML Standalone.
- Wajib mengikuti best-practice SEMANTIC HTML agar SEO-nya bagus.
- Wajib mengisi semua ALT IMAGE dengan isi sesuai dengan konteksnya.
- Tidak boleh mengimport Custom Font di HTML karena Custom Font Wajib di CSS.
- Tiap Link Internal untuk pindah antar page wajib "/<slug-page>" dengan mengikuti prinsip href Wordpress Elementor Page dan slugnya harus sesuai dengan nama page .html yang dibuat.
- Untuk External Link open in new tab (`target="_blank" rel="noopener noreferrer"`).
- Header dan Footer dipisah, dengan membuat `header.html` dan `footer.html`.

## Aturan CSS
- CSS masuk ke Global CSS Elementor yang berlaku sitewide (`style.css`).
- CSS hanya ada 1 dan UNTUK SEMUA PAGE termasuk Header dan Footer.
- Pastikan mengikuti best-practice CSS dengan mendefinisikan variabel berulang dengan `:root { --<property-css> }`.
- Saat menggunakan Custom Font wajib mengimport dari CSS menggunakan CSS `@import`.
- Pastikan Mobile-First Responsive Breakpoint.

## Aturan JS
- Semua TAG script JS harus inline di dalam body TAG HTML (di akhir sebelum `</body>`).
- Menerapkan Internal JS.
- Tidak ada file .js terpisah.
- Dilarang menaruh script di dalam head.

# Aturan Accessibility dan Performa
- Semua img wajib ada alt dan ada isinya sesuai konteksnya.
- loading="lazy" untuk semua gambar di bawah fold.
- Semua img wajib ada attribute width dan height untuk mencegah layout shift (CLS).
- Gunakan rel="preload" untuk stylesheet kritis bila diperlukan.

## List Link & Informasi Utama boloupgo.app
