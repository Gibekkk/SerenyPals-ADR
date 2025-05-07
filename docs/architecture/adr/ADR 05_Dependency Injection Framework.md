---
status: Proposed
date: 2025-07-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 05: Dependency Injection Framework

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami memerlukan dependencies agar lebih efektif. Oleh sebab itu, aplikasi kami memerlukan sebuah cara untuk memasukkan dependencies ke dalam aplikasi kami. Namun, karena keterbatasan waktu dan keahlian, pilihan kami sangat sedikit.

## Decision

* Kami tidak menggunakan dependency injection, dan melakukan import secara manual. Kami memilih mekanisme ini karena beberapa alasan, yaitu:
    * Kami tidak memiliki keahlian ataupun pengalaman dalam menggunakan dependency injection
    * Kami tidak memiliki waktu yang cukup untuk mulai mempelajari cara menggunakan dependency injection

## Alternative Options
1. GetIt
  * Pros:
    * Lebih mudah melakukan scalable di update masa depan
  * Cons:
    * Lebih rumit dan kompleks
    * Memakan banyak waktu dan usaha untuk menginisialisasi aplikasi di pembangunan awal

### Consequences

* Baik, karena jika tidak menggunakan dependency injection, pembangunan aplikasi di awal lebih mudah dan struktur lebih sederhana untuk dipelajari
* Buruk, karena jika tidak menggunakan dependency injection, ketika ingin melakukan penambahan scaling aplikasi, dependency perlu diinisialisasi satu per satu secara manual

