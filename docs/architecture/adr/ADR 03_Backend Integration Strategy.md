---
status: Accepted
date: 2025-06-05
deciders: Tiffany
consulted: Gilbert
informed: Gilbert, Valentino
---
# ADR 03: Backend Integration Strategy

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami perlu menerima data melalui Backend. Oleh sebab itu, kami perlu menentukan metode yang akan kami gunakan untuk mengintegrasikan Frontend dan Backend aplikasi kami. Karena keterbatasan waktu pengembangan dan keterbatasan ilmu dalam pemilihan metode integrasi yang tersedia, kami perlu menyesuaikan dengan metode yang kami ketahui saja.

## Decision

* Metode Backend Integration yang kami gunakan dalam pengembangan aplikasi ini adalah RESTful API. Kami memilih metode ini karena beberapa alasan:
  * Sudah pernah digunakan dalam project sebelumnya
  * Memiliki penggunaan dan cara integrasi yang sederhana dengan frontend

## Alternative Options
1. Firebase
  * Pros:
    * Memikiki fitur hosting gratis yang bisa digunakan secara online
  * Cons:
    * Membutuhkan waktu yang cukup lama untuk mempelajari penggunaan versi terbaru
    * Tutorial untuk menggunakan versi terbaru sangat sedikit 

### Consequences

* Baik, karena dalam RESTful API, integrasi backend ke frontend hanya menggunakan link dengan payload dan response yang sederhana dan efektif
* Buruk, karena dalam RESTful API, setiap kali frontend ingin mengambil data atau mengirimkan data ke backend, perlu dibuat request baru dan bisa saja memberatkan server bila suatu proses memerlukan banyak request dalam waktu yang sama