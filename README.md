# Kuiz Bahasa Arab Tingkatan 3 (اِخْتِبَار اللُّغَة العَرَبِيَّة)

Kuiz interaktif berasaskan web untuk mata pelajaran **Bahasa Arab KSSM Tingkatan 3**.
Murid boleh menguji penguasaan **kosa kata**, **tarakib** (susunan ayat) dan **jenis ayat**
mengikut lima tema Tingkatan 3, dengan maklum balas serta-merta bagi setiap soalan.

![Bahasa](https://img.shields.io/badge/bahasa-Melayu%20%2B%20Arab-0d5249)
![HTML](https://img.shields.io/badge/dibina%20dengan-HTML%20%2B%20CSS%20%2B%20JS-c98a16)

## Ciri-ciri

- 18 soalan aneka pilihan merentas 5 tema Tingkatan 3
- Soalan dan pilihan jawapan **diacak** setiap kali main
- Maklum balas serta-merta + penjelasan ringkas (betul/salah)
- Skor langsung, bar kemajuan dan cincin peratusan keputusan
- **Semakan jawapan** penuh di akhir kuiz
- Boleh dikawal guna **papan kekunci** (A–D untuk jawab, Enter untuk teruskan)
- Reka bentuk responsif (sesuai telefon) + sokongan teks Arab (khat Amiri)

## Cara menggunakan

Buka sahaja `index.html` dalam mana-mana pelayar — tiada pemasangan diperlukan.

## Cara menerbitkan di GitHub Pages

1. Cipta repositori baharu di GitHub (contoh: `kuiz-bahasa-arab`).
2. Muat naik fail `index.html` (dan `README.md`) ke repositori tersebut.
3. Pergi ke **Settings → Pages**.
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`, kemudian **Save**.
5. Tunggu seketika, pautan kuiz anda akan muncul:
   `https://NAMA-PENGGUNA.github.io/kuiz-bahasa-arab/`

## Menambah atau mengubah soalan

Semua soalan disimpan dalam array `BANK` di dalam `index.html`. Setiap soalan:

```js
{
  tag:"Kosa Kata",                 // kategori (dipaparkan di atas soalan)
  prompt:"Apakah maksud ini?",     // arahan soalan
  stim:"المِطْرَقَة",               // (pilihan) teks Arab besar
  type:"ms",                       // "ms" = pilihan Melayu, "ar" = pilihan Arab
  opts:["Gergaji","Tukul","Paku","Pemutar skru"],
  a:1,                             // indeks jawapan betul (mula dari 0)
  why:"Penjelasan ringkas..."      // boleh guna <span class='ar'>...</span>
}
```

Tambah sahaja objek baharu ke dalam array untuk menambah soalan.

## Tema yang diliputi

1. Menyebarkan Salam & Akhlak — إفشاء السلام
2. Buat Sendiri & Kemahiran — اصنع بنفسك
3. Lalu Lintas & Jalan Raya — من بيتك إلى المدرسة
4. Alam Sekitar & Kebersihan — معا للحي الأنظف
5. Resipi & Memasak — وصفة الطعام

---

Dibina untuk kegunaan pengajaran dan pembelajaran Bahasa Arab KSSM Tingkatan 3.
