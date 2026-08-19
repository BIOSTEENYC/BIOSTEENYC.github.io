# Abdulhakim Xayitboyev — Biosteenyc
Ilm‑fan va ijodkorlik uygʻunligi — shaxsiy portfoliom va loyihalarim jamlanmasi.

[Live demo — biosteenyc.github.io](https://biosteenyc.github.io)  
[CV (PDF)](https://raw.githubusercontent.com/biosteenyc/BIOSTEENYC.github.io/gh-pages/Abdulhakim%20Xayitboyev%20Rezume.pdf) • [YouTube](https://youtube.com/@biosteenyc) • [Telegram: Biosteenyc](https://t.me/biosteenyc)

---

[![Website](https://img.shields.io/website?url=https%3A%2F%2Fbiosteenyc.github.io&style=for-the-badge&color=7c3aed)](https://biosteenyc.github.io) [![GitHub stars](https://img.shields.io/github/stars/biosteenyc/BIOSTEENYC.github.io?style=for-the-badge&color=00696f)](https://github.com/biosteenyc/BIOSTEENYC.github.io/stargazers) [![Followers](https://img.shields.io/github/followers/biosteenyc?style=for-the-badge)](https://github.com/biosteenyc)

## Qisqacha (TL;DR)
Men — Abdulhakim (Biosteenyc). Dasturchi, mobil ilova muallifi va havaskor shoirman. Kod va sheʼrlarni bir joyga toʻplab, interaktiv portfolio va amaliyot materiallarini yarataman. Bu repo — mening jamoat sahifam (GitHub Pages) va portfoliomning markazi.

---

## Loyihalar (tanlangan)
- Biosteenyc — personal website & portfolio  
  - Live: https://biosteenyc.github.io  
  - Texnologiyalar: HTML, Tailwind CSS (CDN), Three.js (3D kitob), GSAP, PDF.js, FontAwesome.  
  - Xususiyatlar: 3D WebGL kitob bilan sheʼr varoqlash, ko‘p tillik (lotin/kiril/RTL/tg/ky), CV yuklash, YouTube banner.

- UstaMakon — tizim optimizatsiyasi va diagnostika ilovasi  
  - Repo: https://github.com/biosteenyc/ustamakon  
  - Qisqacha: Mobil qurilmadan desktop (Windows/Linux) ilovasiga ulanib, tezkor optimizatsiya va diagnostika amallarini bajaradi.  
  - Texnologiyalar: Flutter (Dart), Supabase (maʼlumotlar), QR skanerlash, AppImage / .exe distributivlar.  
  - Qoʻllash: mobil + desktop kombinatsiyasi; Supabase URL/ANON_KEY bilan sozlash talab etiladi.

- Abdulhakim Sheʼrlari (poetry dataset & reader)  
  - Repo: https://github.com/biosteenyc/abdulhakim_sherlari  
  - Qisqacha: Sheʼrlar toʻplami, 3D kitobga integratsiya qilingan material. Index.html ichida `rawPoetryDatabase` orqali saqlanadi.

- Amaliyot taqdimotlari (PDF viewer)  
  - Saytda PDF.js yordamida interaktiv ko‘rinish (Amaliyot 2025 / 2026).

---

## Texnik stack (asosiy)
- Frontend: HTML, Tailwind CSS, Google Fonts, FontAwesome  
- 3D & animatsiya: Three.js (r128), GSAP  
- PDF viewer: PDF.js  
- Mobile/Desktop app: Flutter (Dart), video_player, mobile_scanner, qr_flutter  
- Backend / DB: Supabase (used by UstaMakon)  
- CI / automation: GitHub Actions (oddiy CI workflow mavjud)

---

## Lokalda tez ishga tushirish
Statik portfolio (shu repo) uchun:
```bash
git clone https://github.com/biosteenyc/BIOSTEENYC.github.io.git
cd BIOSTEENYC.github.io
python3 -m http.server 8000
# oching: http://localhost:8000
