---
title: Proyek Pemrograman Website Black Jack
description: Website Game Black Jack menggunakan HTML, CSS, dan Java
author: cotes
date: 2024-04-20 11:33:00 +0800
categories: [Blogging, Demo]
tags: [HTML, Java, Web, Game, Desain, Blackjack]
pin: false
math: true
mermaid: true
image:
  path: /assets/blackjack.jpg
  lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
  alt: Tampilan website game Black Jack pada berbagai perangkat.
---

# 🃏 Proyek Website Game Black Jack
{: .mt-4 .mb-2 }

> Proyek ini membuat game **Black Jack berbasis web** menggunakan kombinasi **HTML, CSS**, dan **Java**, agar dapat dijalankan secara langsung melalui browser dengan pengalaman interaktif yang simpel dan elegan.

---

## 🎯 Tujuan Proyek
Membangun aplikasi permainan **Black Jack** dengan tampilan user-friendly dan logika permainan yang mengikuti aturan standar Black Jack, di mana pemain bermain melawan komputer (dealer).

---

## 🛠️ Teknologi yang Digunakan

| Komponen        | Teknologi             | Fungsi                                 |
|-----------------|-----------------------|----------------------------------------|
| Struktur UI     | `HTML`                | Menyusun elemen halaman                |
| Tampilan Visual | `CSS`                 | Mendesain tata letak dan gaya visual   |
| Logika Game     | `Java` / `JavaScript` | Mengatur aturan & gameplay             |

---

## 🔧 Fitur Utama

- 🎮 **Tombol Aksi**: `Hit`, `Stand`, dan `Restart`
- 🖥️ **Tampilan Kartu**: Kartu pemain & dealer ditampilkan real-time
- 📱 **Responsive Layout**: Tampilan menyesuaikan untuk mobile dan desktop
- 🔁 **Sistem Skor** *(rencana)*: Menyimpan skor kemenangan pengguna

---

## ✅ Checklist Pengembangan

- [x] Struktur UI dasar menggunakan HTML
- [x] Styling responsif dengan CSS
- [x] Logika Black Jack menggunakan Java
- [ ] Tambahan animasi kartu
- [ ] Peringkat skor pemain

---

## 📌 Langkah Pengerjaan

1. Mendesain UI dengan elemen HTML & CSS modern
2. Membuat class Java untuk menangani kartu, skor, dan aturan game
3. Menyambungkan UI dan logika menggunakan JavaScript (jika client-side)
4. Menguji gameplay dan kompatibilitas tampilan di berbagai device

---

## 💬 Catatan Pengembangan

> "Proyek ini sangat cocok untuk belajar logika pemrograman game dasar berbasis web."
{: .prompt-info }

> Gunakan `localStorage` atau `sessionStorage` bila ingin menyimpan skor di sisi klien.
{: .prompt-tip }

> Perhatikan validasi agar pemain tidak bisa menekan `Hit` setelah `Stand`.
{: .prompt-warning }

> Optimalkan penggunaan loop dan DOM event untuk menghindari lag saat interaksi.
{: .prompt-danger }

---

## 📷 Contoh Tampilan Game

![Tampilan Game Black Jack](/assets/blackjack.jpg){: .w-75 .shadow .rounded-10 }

_Tampilan Game Black Jack._

---

## 📎 Repository Kode

🔗 [Lihat di GitHub](https://github.com/muslihkar17/LAB-WEB-15-2024/tree/main/H071231042/TUGAS%205)

---

## 📄 Contoh Kode Java

```java
public class Card {
    private String suit;
    private String value;

    public Card(String value, String suit) {
        this.value = value;
        this.suit = suit;
    }

    public String toString() {
        return value + " of " + suit;
    }
}
