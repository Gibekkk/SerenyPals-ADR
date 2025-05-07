---
title: 'ADR 02: State Management Approach'

---

---
status: Accepted
date: 2025-06-05
deciders: Tiffany
consulted: ChatGPT, Kasmir Syariati
informed: Gilbert, Valentino
---
# ADR 02: State Management Approach

## Context

Dalam mengembangkan aplikasi FrontEnd dari SerenyPals, kami perlu menentukan State Management yang akan digunakan dalam mengembangkan aplikasi ini. Karena keterbatasan waktu pengembangan dan keterbatasan ilmu dalam pemilihan State Management yang tersedia, kami perlu menyesuaikan dengan State yang kami ketahui saja.

## Decision

* State Management yang kami gunakan dalam pengembangan aplikasi ini adalah BLoC (Business Logic Managemet). Kami memilih State ini karena beberapa alasan:
  * Sudah pernah digunakan dalam project sebelumnya
  * Memiliki penggunaan yang cukup sederhana bagi para pemula

## Alternative Options
1. RiverPod
  * Pros:
    * Banyak tutorial mengenai cara menggunakan RiverPod yang tersedia
  * Cons:
    * Memiliki banyak class yang rumit untuk digunakan
    * Cukup sulit untuk dipelajari para pemula 

### Consequences

* Baik, karena dalam BloC, lapisan UI dan logika bisnis dipisah dan memungkinkan untuk pengembangan yang lebih terstruktur dan mudah dimengerti
* Buruk, karena dalam BloC yang lapisan UI dan logika bisnis yang dikembangkan secara terpisah membuat struktur file menjadi sangat panjang dan kompleks 