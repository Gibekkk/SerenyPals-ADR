---
title: 'ADR 01: App Architecture Pattern'

---

---
status: Accepted
date: 2025-06-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 01: App Architecture Pattern

## Context

Dalam mengembangkan aplikasi FrontEnd dari SerenyPals, kami perlu menentukan pola arsitektur yang akan digunakan dalam mengembangkan aplikasi ini. Karena keterbatasan waktu pengembangan dan keterbatasan ilmu dalam pemilihan pola yang tersedia, kami perlu menyesuaikan dengan pola yang kami ketahui saja. Juga karena menggunakan Flutter dalam pengembangan, maka kami perlu menyesuaikan pola yang akan kami gunakan dengan techstack tersebut.

## Decision

* Pola yang kami gunakan dalam pengembangan aplikasi ini adalah pola MVVM atau Model-View-ViewModel. Kami memilih pola ini karena beberapa alasan:
  * Menghemat waktu pengembangan karena tidak perlu mengembangkan controller dan dapat secara langsung menggunakan dan memanipulasi data di dalam tampilan
  * Sesuai dengan Flutter dan dapat bekerja dengan baik dalam penggunaan tools eksternal

## Alternative Options
1. MVC
  * Pros:
    * Struktur yang sangat rapi dan kompleks sehingga pengembangan lebih terstruktur
  * Cons:
    * Memerlukan banyak waktu untuk inisialisasi aplikasi

### Consequences

* Baik, karena dalam MVVM pengembangan tidak memerlukan banyak waktu untuk memanipulasi data secara terpisah dan mendukung banyak tools external
* Buruk, karena dalam MVVM struktur aplikasi terlihat tidak rapi karena pemrosesan data yang tertumpuk di dalam pemrosesan tampilan, dan seringkali menyebabkan beberapa kesalahan dalam manipulasi data
