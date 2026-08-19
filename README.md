# Biosteenyc — Ilm-fan va Ijodkorlik uygʻunligi

Live demo: https://biosteenyc.github.io

## Umumiy ma'lumot
Biosteenyc — bu Abdulhakim Xayitboyev (tahallusi: Biosteenyc) ning shaxsiy veb-sayti va portfoliysi. Sayt ilm-fan, dasturlash, mobil ilovalar, UstaMakon loyihasi hamda shoirlik ijodini birlashtiradi.

Sayt yagona fayldan (index.html) tashkil topgan, statik SPA uslubida yozilgan va GitHub Pages orqali joylashtirilgan.

## Asosiy sahifalar va funksionallik
- Asosiy (Home / Asosiy)
  - Profil kartochkasi, qisqacha bio va tezkor tugmalar (GitHub, YouTube, CV).
  - Teglar (hashtags) bilan shaxsiy brend ko'rsatilgan.

- Ijod (Poetry / Ijod)
  - 3D WebGL kitob (Three.js orqali) — sichqoncha yoki barmoq bilan aylantirish va sahifalarni varoqlash.
  - Kategoriyalar bo'yicha sheʼr filterlari.
  - YouTube kanali reklama bannerni o'z ichiga olgan.

- Ilm (Projects & Practice / Ilm)
  - UstaMakon loyihasi: mobil-desktop integratsiya, yuklab olish tugmalari (Windows, Linux, Google Play).
  - Amaliyot bo'limi: PDF taqdimotlarni ochish uchun PDF.js modal viewer mavjud (Amaliyot 2025, 2026 misollari).

- Umumiy xususiyatlar
  - To'liq ko'p tillilik (uz_latn, uz_cyrl, uz_afg(RTL), tg_cyrl, ky_cyrl) — tarjimalar index.html ichidagi `translations` obyekti orqali boshqariladi.
  - Kun/tungi rejim (theme toggle) — Tailwind dark mode orqali ishlaydi.
  - Material-like kartalar va yumshoq animatsiyalar (GSAP, CSS transitions).
  - FontAwesome, Google Fonts ishlatilgan.

## Texnologiyalar
- HTML (bitta fayl: index.html)
- Tailwind CSS (CDN)
- Three.js (r128) — 3D kitob
- GSAP — animatsiyalar
- PDF.js — PDF viewer
- FontAwesome — ikonlar
- Google Fonts

## Fayl tuzilmasi
Reponing asosiy mazmuni:
- index.html — butun sayt va barcha kontent (poeziya ma'lumotlari, tarjimalar, 3D kitob va PDF viewer logikasi) shu faylda joylashgan.
- Ba'zi PDF va CV fayllar raw.githubusercontent.com orqali bog'langan (gh-pages branch yoki release assets).

> Eslatma: sayt kontenti (she'rlar) `index.html` ichidagi `rawPoetryDatabase` massivida saqlangan. Tarjimalar `translations` obyektida.

## Lokalda ishga tushirish
Statik sayt bo'lgani uchun, fayllarni shunchaki brauzerda ochish mumkin, lekin baʼzi brauzerlarda CORS yoki font yuklanishi muammosi bo'lishi mumkin. Quyidagi usullar tavsiya etiladi:

1) Oddiy HTTP server (Python 3):

```bash
git clone https://github.com/biosteenyc/BIOSTEENYC.github.io.git
cd BIOSTEENYC.github.io
python3 -m http.server 8000
# brauzerda: http://localhost:8000
```

2) npm http-server (agar mavjud bo'lsa):

```bash
npx http-server -c-1
# yoki
npm i -g http-server
http-server
```

3) GitHub Pages orqali avtomatik: bu repo allaqachon `gh-pages` yoki repo-nomi.github.io orqali joylashtirilgan.

## Qanday qilib mazmunni yangilash mumkin
- She'rlarni tahrirlash / qo'shish: index.html ichidagi `rawPoetryDatabase` massiviga yangi obyekt qo'shing yoki mavjud obyektning `lines` massivini yangilang.
- Tarjimalarni yangilash: `translations` obyektida kerakli til kalitiga yangi `data-i18n` kalitlari va qiymatlarini qo'shing.
- CV yoki PDF fayllarni yangilash: `CV Yuklash` va `openPDFViewer` funksiyasidagi URL manzillarni mos faylga yo'naltiring.
- 3D kitob sahifalari va sahifa ichidagi stylarni o'zgartirish uchun Three.js sahnasi va `rawPoetryDatabase` dan kelayotgan mazmunni sinxronlashtiring.

## Rivojlantiruvchilar uchun tez qadamlar
- index.html fayli katta va bir faylda hamma narsani o'z ichiga oladi — komponentizatsiya uchun faylni bo'lish, CSS va JS ajratish tavsiya etiladi.
- Ustunliklar: CDN-lar ishlatilgan (Tailwind, FontAwesome, Three.js, GSAP, PDF.js) — offline yoki o'chirilgan CDN uchun lokal nusxalar kerak bo'lishi mumkin.
- Three.js versiyasi r128; agar yangilash rejalashtirilsa, API o'zgarishlarini tekshiring.

## Muallif va kontakt
- Muallif: Abdulhakim Xayitboyev (Biosteenyc)
- Telefon: +998 - (33) - 349 - 09 - 30
- Telegram: Biosteenyc
- GitHub: https://github.com/biosteenyc
- YouTube: https://youtube.com/@biosteenyc

## Litsenziya
Repo ichida hozircha LICENSE fayli ko'rinmaydi. Agar siz ruxsat bergan bo'lsangiz, MIT yoki boshqa mos litsenziyani qo'shishni tavsiya qilaman.
