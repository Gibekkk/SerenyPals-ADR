---
status: Proposed
date: 2025-07-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 09: Error Handling & Monitoring

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami perlu mengembangkan environment aplikasi yang aman. Namun, bug dan error kerap terjadi. Jadi, kami perlu menentukan mekanisme dalam menangani error dan melakukan monitoring terhadap aplikasi. Namun, karena keterbatasan waktu dan keahlian, pilihan kami pun terbatas dalam hal ini.

## Decision

* Kami menggunakan Sentry. Kami memilih mekanisme ini karena beberapa alasan, yaitu:
    * Mekanisme ini memungkinkan kami untuk memonitor error pada aplikasi secara realtime
    * Mekanisme ini lebih menghemat waktu karena untuk mengimplementasikan cukup mudah dan sederhana

## Alternative Options
1. Custom Logging
  * Pros:
    * Lebih fleksibel dan mudah untuk dibuat sesuai kebutuhan error
  * Cons:
    * Memerlukan implementasi yang lebih sulit dari segi frontend dan backend
    * Memakan lebih banyak waktu untuk diimplementasikan karena membutuhkan catch error pada berbagai jenis tingkatan error

### Consequences

* Baik, karena jika menggunakan Sentry, aplikasi kami lebih mudah untuk dimonitor dan diperbaiki secara langsung melalui dashboard Sentry, dan mudah untuk diimplementasikan
* Buruk, karena jika menggunakan Sentry, kami belum sepenuhnya paham menggunakan sistem dashboard dan cara yang paling efektif dalam penggunaannya, memungkinkan waktu dan tenaga yang lebih banyak digunakan dalam proses pemahaman