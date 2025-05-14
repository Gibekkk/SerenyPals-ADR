---
status: Proposed
date: 2025-06-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 04: Local Data Persistence

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami perlu menerima data melalui Backend. Oleh sebab itu, aplikasi perlu terhubung dengan internet untuk mengakses data secara real time. Namun, jika jaringan tidak stabil atau tidak tersedia, aplikasi perlu suatu cara untuk bekerja secara offline meskipun dengan fitur yang terbatas. Maka, kami perlu menentukan mekanisme penyimpanan local agar aplikasi SerenyPals dapat tetap bekerja secara offline. Namun, karena keterbatasan ilmu dan waktu pengembangan, kami perlu menyesuaikan dengan mekanisme yang handal digunakan saja.

## Decision

* Mekanisme Data Storage yang kami gunakan dalam pengembangan aplikasi ini adalah ObjectBox. Kami memilih mekanisme ini karena beberapa alasan:
    * Memiliki performa dan fitur yang jauh lebih bagus dibandingkan SQLite
    * Memiliki resource dan penggunaan penyimpanan yang lebih sedikit
    * Penggunaan yang jauh lebih mudah dibandingkan SQLite

## Alternative Options
1. SQLite
  * Pros:
    * Mensupport penggunaan pada device versi lama
  * Cons:
    * Tidak efektif dan memiliki pemakaian storage yang lebih besar
    * Kode yang lebih panjang dibandingkan ObjectBox

### Consequences

* Baik, karena dalam ObjectBox, pengolahan Data Storage menjadi sangat mudah dan efektif dari segi teknis dan resource dibandingkan SQLite
* Buruk, karena dalam ObjectBox, banyak fitur yang memerlukan device dengan versi yang cukup baru dan tidak dapat bekerja di device versi lama