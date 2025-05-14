---
status: Proposed
date: 2025-07-05
deciders: Tiffany
consulted: ChatGPT
informed: Gilbert, Valentino
---
# ADR 10: Testing Strategy & CI/CD Pipeline

## Context

Dalam mengembangkan aplikasi Frontend dari SerenyPals, kami perlu mengembangkan environment aplikasi yang aman. Oleh karena itu, perlu diterapkan testing dan auto build dalam pembangunan aplikasi. Namun, karena keterbatasan waktu dan keterampilan, kami tidak memiliki banyak pilihan.

## Decision

* Kami tidak menggunakan pipeline. Kami tidak menggunakan pipeline karena beberapa alasan, yaitu:
    * Keterbatasan waktu dalam implementasi dan setup environment untuk testing dan auto build
    * Kami sudah menerapkan error handling, dan dengan segala keterbatasan sudah cukup membantu dalam testing error, dan kami melakukan testing fitur secara manual untuk mengidentifikasi tingkat keberhasilan dengan lebih akurat pada fitur tersebut
    * Kami tidak memerlukan publish aplikasi untuk sementara, dan tidak memerlukan fitur auto build dan fitur publish
 
## Alternative Options
1. Github Action
  * Pros:
    * Memiliki fitur unit testing
    * Memiliki fitur auto publish dan auto build
  * Cons:
    * Memerlukan waktu yang lebih lama untuk disetup
    * Workflow yang cukup lambat untuk mendapatkan hasil build

### Consequences

* Baik, karena jika tidak menggunakan pipeline, kami dapat menghemat waktu belajar dan pemahaman penggunaan pipeline, dan melakukan testing fitur secara manual dan lebih akurat
* Buruk, karena jika tidak menggunakan pipeline, kami akan kesulitan jika aplikasi suatu saat perlu dipublish dan dibuat menjadi lebih besar lagi dengan version control
