# Design Patterns Library

> Pusat pembelajaran untuk memahami pola desain, prinsip desain software, dan struktur internal kode agar sistem tetap dapat dirawat saat kompleksitasnya bertumbuh.

## 1. Identitas Hub
- **Nama:** Design-Patterns-Library
- **Fokus Utama:** software design principles, SOLID, GoF patterns, clean architecture, dependency inversion, composition, internal code structure across major languages
- **Status di Learning Matrix:** pilar utama `RAK-05 Architecture Hubs`
- **Peran Umum:** internal software design, pattern literacy, maintainability thinking, abstraction discipline, code-level architecture
- **Persona Utama:** Software Design Patterns Architect & Internal Structure Strategist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `LAB`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
Design patterns penting dipelajari karena banyak codebase rusak bukan karena teknologinya salah, tetapi karena struktur internalnya tumbuh tanpa prinsip, tanpa kosakata bersama, dan tanpa batas abstraksi yang sehat.

Hub ini relevan ketika kita ingin memahami:
- bagaimana mencegah logic berubah menjadi spaghetti code,
- bagaimana tim bisa berdiskusi tentang solusi desain dengan bahasa yang sama,
- bagaimana dependency seharusnya diarahkan,
- dan bagaimana pola desain membantu software bertahan terhadap perubahan.

Di dalam Learning Matrix, design patterns bukan kumpulan trik wawancara. Ia adalah pustaka mental untuk membentuk software yang lebih dapat dirawat.

## 3. Core DNA

### Principles before Patterns
Pola desain yang sehat lahir dari prinsip yang sehat.
Karena itu pembahasan pattern harus bertumpu pada:
- separation of concerns,
- single responsibility,
- dependency inversion,
- composition over inheritance,
- dan batas abstraksi yang jelas.

### Patterns as Shared Vocabulary
Pattern memberi tim bahasa bersama.
Dengan kosakata ini, diskusi kompleks bisa dipadatkan menjadi istilah yang punya bentuk arsitektural yang dikenali bersama.

### Dependency Discipline
Salah satu DNA utama hub ini adalah disiplin arah dependency.
Komponen inti tidak boleh bocor ke detail implementasi yang seharusnya bisa diganti.

### Trade-off Awareness
Pattern bukan mantra suci.
Setiap pola membawa:
- manfaat,
- cost,
- kompleksitas,
- dan risiko over-engineering.

### Cross-Language Design Thinking
Pattern perlu dipahami lintas bahasa.
Implementasinya bisa berbeda di:
- TypeScript,
- Go,
- Python,
- Rust,
- atau JavaScript,
tetapi inti masalah rekayasanya sering sama.

## 4. The How
Cara berpikir design patterns bertumpu pada satu prinsip besar: **gunakan abstraksi secukupnya untuk menahan perubahan, bukan untuk memamerkan kerumitan**.

Mental model penting di hub ini adalah:
- mulai dari masalah desain,
- pahami tekanan perubahan yang ingin ditahan,
- pilih prinsip lebih dulu,
- gunakan pattern hanya jika memang membantu,
- dan nilai setiap abstraksi dari dampaknya terhadap keterbacaan, fleksibilitas, dan maintenance cost.

## 5. Kekuatan Utama
- Membantu tim punya kosakata desain yang sama.
- Menjaga struktur internal software tetap terbaca saat skala bertambah.
- Membantu mengelola perubahan melalui abstraksi yang sadar.
- Relevan lintas bahasa dan lintas domain.
- Menjadi jembatan kuat ke clean architecture, dependency injection, dan modular design.
- Sangat berguna untuk review code dan refactor besar.

## 6. Trade-offs dan Kelemahan
- Mudah disalahgunakan menjadi over-engineering.
- Pola yang benar di konteks salah tetap menjadi beban.
- Abstraksi berlebihan dapat memperlambat pengembangan sederhana.
- Tim bisa menghafal nama pattern tanpa memahami problem yang diselesaikannya.
- Tidak menggantikan kebutuhan akan application architecture, repository design, atau system design.

## 7. Use Case Prioritas
Design patterns paling cocok untuk:
- growing codebases
- reusable internal architecture
- clean separation of logic
- dependency-heavy systems
- service and module refactors
- framework-agnostic software design
- lintas bahasa yang tetap butuh prinsip serupa

Hub ini kurang ideal jika fokus utamanya adalah:
- project kecil yang belum punya tekanan desain berarti
- eksplorasi ide sekali pakai
- diskusi workflow bisnis di level aplikasi
- topologi distribusi sistem dan cloud-scale architecture

## 8. Kapan Dipilih
Pilih hub ini ketika:
- codebase mulai sulit dirawat,
- dependency mulai saling mencengkeram,
- logic inti bercampur dengan detail implementasi,
- tim perlu bahasa desain bersama,
- atau Anda sedang melakukan refactor struktural di level software.

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke hub ini ketika:
- problem utama masih di pemetaan produk dan workflow,
- repository belum punya struktur dasar yang bisa ditopang,
- project masih sangat kecil,
- atau tantangan utama ada di skala sistem, bukan desain internal software.

## 10. Posisi di Learning Matrix
Design patterns paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  `TypeScript-Knowledge-Base`, `Golang-Knowledge-Base`, `Python-Knowledge-Base`, `Rust-Knowledge-Base`, `JavaScript-Knowledge-Base`

- **Execution Hubs:**
  relevan secara tidak langsung karena pola desain sering muncul di software yang hidup di browser atau server runtimes

- **Digital UI Hubs:**
  relevan untuk component composition, state handling abstractions, UI service boundaries, dan frontend maintainability

- **Storage Hubs:**
  relevan untuk repository pattern, data access abstractions, unit of work thinking, dan persistence isolation

- **Architecture Hubs:**
  `Application-Architecture-Hub`, `Repository-Architecture-Hub`, `System-Design-Architect-Hub`

- **Infrastructure Hubs:**
  relevan ketika abstractions menyentuh config, delivery boundaries, adapters, dan runtime integration

- **Version Control Hubs:**
  relevan untuk refactor discipline, shared conventions, dan menjaga perubahan desain tetap dapat ditinjau

- **AI Orchestration Hubs:**
  sangat relevan untuk pattern review, refactor support, dependency reasoning, dan architecture critique

- **Security Identity Hubs:**
  relevan ketika boundary internal software memengaruhi auth, policy enforcement, dan trust-sensitive flows

## 11. Jalur Belajar Praktis
Contoh jalur belajar design patterns di dalam Learning Matrix:

### Jalur Internal Software Design
`Repository-Architecture-Hub -> Design-Patterns-Library -> System-Design-Architect-Hub`

### Jalur Type-Safe Application Refinement
`TypeScript -> Application-Architecture-Hub -> Design-Patterns-Library`

### Jalur Backend Refactor Discipline
`Golang -> Server Runtime -> PostgreSQL -> Design-Patterns-Library`

### Jalur Systems-Aware Code Design
`Rust -> Repository-Architecture-Hub -> Design-Patterns-Library -> System Design`

## 12. Repository dan Workspace Terkait
Node Design Patterns di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis design patterns di dalam Learning Matrix.

- **Workspace Kolektif Arsitektur:**
  `05-Architecture-Hubs`
  Perannya adalah menjadi area kerja arsitektur yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman Design Patterns:**
  `05-Architecture-Hubs/Design-Patterns-Library`
  Perannya adalah menjadi workspace khusus untuk membedah pola desain jauh lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace Design Patterns Perlu Dipisah
Workspace design patterns perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace design patterns boleh:
- menyimpan katalog pattern,
- menyimpan prinsip desain dan anti-pattern,
- menyimpan implementasi lintas bahasa,
- menyimpan refactor examples,
- menyimpan clean architecture studies,
- menyimpan dependency inversion labs,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di Design Patterns Workspace
Untuk pendalaman design patterns, struktur awal yang disarankan untuk workspace turunannya adalah 8 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: Design Principles and Mental Models
Fokus:
- SOLID,
- composition over inheritance,
- separation of concerns,
- dependency direction,
- dan prinsip dasar desain software.

### RAK-02: Creational Patterns
Fokus:
- factory,
- abstract factory,
- builder,
- singleton,
- dan pola penciptaan objek atau komponen.

### RAK-03: Structural Patterns
Fokus:
- adapter,
- facade,
- decorator,
- composite,
- proxy,
- dan pola pembentukan struktur internal software.

### RAK-04: Behavioral Patterns
Fokus:
- strategy,
- observer,
- command,
- state,
- chain of responsibility,
- dan pola perilaku yang membantu mengelola variasi logika.

### RAK-05: Clean Architecture and Dependency Design
Fokus:
- dependency rule,
- ports and adapters,
- use cases,
- domain isolation,
- dependency injection,
- dan arsitektur software yang lebih tahan perubahan.

### RAK-06: Anti-Patterns and Over-Engineering
Fokus:
- rigidity,
- needless abstraction,
- accidental complexity,
- God object,
- service soup,
- dan kegagalan desain internal yang umum.

### RAK-07: Cross-Language Implementations
Fokus:
- bagaimana pattern dipraktikkan di TypeScript,
- Go,
- Python,
- Rust,
- dan JavaScript,
- serta perbedaan gaya implementasinya.

### RAK-08: Bridge to Application, Repository, and System Architecture
Fokus:
- hubungan design patterns dengan application architecture,
- hubungan ke repository shape,
- hubungan ke storage adapters dan infrastructure boundaries,
- dan batas kapan software-level design harus naik menjadi system-level architecture.

Sub-rak yang layak untuk design patterns saat ini:

#### Sub-Rak: Design Patterns to TypeScript and JavaScript
Fokus:
- pattern di ekosistem JS/TS,
- composition, services, frontend abstractions, dan backend modularity.

#### Sub-Rak: Design Patterns to Golang
Fokus:
- interface-driven design,
- dependency inversion pragmatis,
- dan pattern dalam service Go yang struktural tetapi tetap ringan.

#### Sub-Rak: Design Patterns to Python
Fokus:
- pragmatic abstractions,
- dynamic language trade-offs,
- dan pattern yang tetap sehat di Pythonic codebases.

#### Sub-Rak: Design Patterns to Rust
Fokus:
- ownership-aware design,
- trait-based abstractions,
- dan batas pattern klasik saat masuk ke dunia Rust.

#### Sub-Rak: Design Patterns to Architecture Boundaries
Fokus:
- bagaimana software design internal terhubung ke application, repository, storage, dan system architecture.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `Design-Patterns-Library` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi design patterns di dalam Learning Matrix.
- Workspace turunannya menjelaskan pattern dan prinsip desain secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning design patterns di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Architecture Lain
- **Dibanding Application-Architecture-Hub:** design patterns bekerja di level struktur internal software, sedangkan application architecture bekerja di level role, workflow, dan modul aplikasi.
- **Dibanding Repository-Architecture-Hub:** design patterns membahas desain internal kode, sedangkan repository architecture membahas bentuk codebase dan governance.
- **Dibanding System-Design-Architect-Hub:** design patterns hidup di level software internals, sedangkan system design hidup di level topologi layanan, distribusi beban, dan availability.

## 17. Pitfalls
- Menghafal nama pattern tanpa memahami problem yang diselesaikannya.
- Menciptakan abstraksi berlebihan demi terlihat arsitektural.
- Memakai pattern klasik pada konteks yang tidak membutuhkannya.
- Menyamakan design pattern dengan kualitas otomatis.
- Mengabaikan cost maintenance dari setiap lapisan abstraksi.
- Memakai clean architecture sebagai slogan tanpa discipline boundary yang nyata.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `05-Architecture-Hubs/Repository-Architecture-Hub`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `04-Storage-Hubs`
- `06-Infrastructure-Hubs`

Dokumen ini terutama berada pada level:
- primary architecture path
- internal software design and maintainability
- pattern literacy and abstraction discipline

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `04-Storage-Hubs`
- `06-Infrastructure-Hubs`
- dan language hub yang paling relevan dengan implementasi pattern yang ingin didalami
