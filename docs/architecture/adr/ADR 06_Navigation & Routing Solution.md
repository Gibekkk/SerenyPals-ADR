---
status: Proposed
date: 2025-06-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 06: Navigation & Routing Solution

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami memerlukan cara untuk melakukan navigasi untuk berpindah dan mengakses aplikasi. Oleh sebab itu, kami perlu menentukan metode untuk melakukan navigasi bagi aplikasi kami. Namun, karena keterbatasan waktu dan keahlian, pilihan kami sangat sedikit.

## Decision

* Kami menggunakan GoRouter. Kami memilih metode ini karena beberapa alasan, yaitu:
    * Lebih mudah menggunakan deep linking untuk notifikasi aplikasi kami
    * Lebih mudah untuk melakukan navigasi dari route yang sudah ditetapkan sebelumnya
    * Struktur aplikasi lebih rapi dan terstruktur

## Alternative Options
1. Navigator default Flutter
  * Pros:
    * Lebih mudah dipelajari karena lebih sederhana
  * Cons:
    * Perlu mendefinisikan route berulang-ulang di setiap layar untuk lokasi tujuan
    * Sulit melakukan deep linking

### Consequences

* Baik, karena jika menggunakan GoRouter, navigasi aplikasi kami jadi lebih terstruktur dan deep linking untuk notifikasi kami lebih mudah untuk dibuat
* Buruk, karena jika menggunakan GoRouter, kami perlu untuk belajar mengenai cara penggunaan GoRouter, dan perlu membangun routing terlebih dahulu yang membuat inisialisasi aplikasi menjadi lebih panjang

