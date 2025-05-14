---
status: Proposed
date: 2025-07-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 08: Offline Support & Caching

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami perlu mengatur mekanisme yang akan digunakan ketika aplikasi diakses secara offline, dan pengelolaan cache agar transfer data tidak selalu terjadi. Namun, karena keterbatasan waktu dan keahlian, kami tidak menerapkan konsep ini di seluruh layar, namun di layar yang perlu saja.

## Decision

* Kami menggunakan mekanisme Offline First. Kami memilih mekanisme ini karena beberapa alasan, yaitu:
    * Mekanisme ini membuat aplikasi kami lebih interaktif sejak dibuka karena tidak memerlukan loading yang terlalu lama di luar layar aplikasi utama
    * Memudahkan akses ke aplikasi tanpa memerlukan jaringan

## Alternative Options
1. Online First
  * Pros:
    * Lebih aman dan memberikan waktu bagi sistem untuk mempersiapkan data sebelum load layar aplikasi
  * Cons:
    * Memerlukan loading yang lebih lama di luar layar konten
    * Memakan lebih banyak data untuk mendownload kembali gambar setiap kali aplikasi dibuka kembali

### Consequences

* Baik, karena jika menggunakan Offline First, aplikasi kami lebih mudah untuk diakses, dan memungkinkan user untuk langsung menggunakan fitur offline ketika jaringan buruk tanpa perlu menunggu load yang lama
* Buruk, karena jika menggunakan Offline First, aplikasi tidak akan terload secara sepenuhnya ketika ingin diakses, dan sinkronisasi menjadi sedikit lebih lambat ketika aplikasi dibuka setelah ditinggalkan cukup lama