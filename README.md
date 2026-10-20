# Daniel Aldo Pratama: online CV

Static site for GitHub Pages. No build step needed.

```
index.html        halaman depan (pilih CV)
it/index.html     CV Backend Engineer
pilot/index.html  CV Commercial Pilot
.nojekyll         supaya GitHub Pages tidak memproses ulang file
```

## Deploy ke GitHub Pages

1. Buat repo baru bernama persis `rocketflash-net.github.io` (public).
2. Upload isi folder ini ke repo tersebut:
   ```
   git init
   git add .
   git commit -m "Online CV"
   git branch -M main
   git remote add origin https://github.com/rocketflash-net/rocketflash-net.github.io.git
   git push -u origin main
   ```
3. Di repo: Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Tunggu 1–2 menit. Situs tersedia di:
   - `https://rocketflash-net.github.io/` (halaman depan)
   - `https://rocketflash-net.github.io/it/`
   - `https://rocketflash-net.github.io/pilot/`

## Mengedit isi

Semua teks ada langsung di file HTML. Contoh: kalau jam terbang bertambah, cari angka `222` di `pilot/index.html` (dan di `index.html`), lalu ganti.
Tombol "Save as PDF" di tiap halaman mencetak versi CV yang bersih (tanpa navigasi dan tombol).
