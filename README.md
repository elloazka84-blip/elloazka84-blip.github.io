# GitHub Pages CalFin

Folder ini siap di-upload ke GitHub Pages untuk dipakai sebagai URL privacy policy Google Play
dan verifikasi `app-ads.txt` AdMob.

## Opsi Paling Mudah

1. Buat repo publik baru di GitHub:
   - paling ideal: `<username>.github.io`
2. Upload seluruh isi folder ini ke root repo.
3. Di GitHub, buka `Settings` > `Pages`.
4. Pada `Build and deployment`, pilih:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
5. Tunggu GitHub Pages aktif.

## URL yang Dipakai

Jika repo bernama `<username>.github.io`:
- `https://<username>.github.io/privacy-policy/`
- `https://<username>.github.io/app-ads.txt`

Jika repo biasa, misalnya `calfin-pages`:
- `https://<username>.github.io/calfin-pages/privacy-policy/`

URL di atas yang dipaste ke field `Privacy policy URL` di Google Play Console.

## Catatan Penting Untuk AdMob

- Agar verifikasi `app-ads.txt` paling aman, gunakan repo GitHub Pages bernama `<username>.github.io`.
- Dengan struktur itu, `app-ads.txt` akan berada di root host dan bisa dicrawl AdMob.
- Jika Anda memakai repo biasa seperti `calfin-pages` atau `calfin-privacy-policy`, privacy policy tetap bisa hidup,
  tetapi `app-ads.txt` tidak berada di root host GitHub Pages.

## Isi Folder

- `index.html`: redirect ringan ke halaman privacy policy
- `privacy-policy/index.html`: halaman kebijakan privasi CalFin
- `app-ads.txt`: file verifikasi AdMob untuk publisher CalFin
- `.nojekyll`: memastikan file statis dipublish apa adanya
