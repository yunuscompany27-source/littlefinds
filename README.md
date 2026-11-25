# Little Finds (GitHub Pages + Supabase)

## 1. Siapkan Supabase
1. Buat project di supabase.com.
2. Buka SQL Editor, tempel isi `schema.sql`, lalu Run.
3. Authentication > Users > Add user: buat akun admin (email + kata sandi).
4. Jalankan di SQL Editor (ganti emailnya):
   `insert into admins select id from auth.users where email = 'emailkamu@contoh.com';`
5. Project Settings > API: salin Project URL dan anon key ke `config.js`.

## 2. Taruh di GitHub
```
git init
git add .
git commit -m "Little Finds"
git branch -M main
git remote add origin https://github.com/USERNAME/lotus-go.git
git push -u origin main
```
Lalu di repo: Settings > Pages > Source: Deploy from a branch > `main` / root.
Situs aktif di `https://USERNAME.github.io/lotus-go/`.

## 3. Setelah online
Di Supabase: Authentication > URL Configuration, isi Site URL dengan alamat GitHub Pages-mu.
