# System Design Architect Hub

> Pusat pembelajaran untuk memahami arsitektur sistem tingkat makro, distribusi beban, batas layanan, strategi skalabilitas, dan trade-off operasional ketika software tumbuh melampaui satu proses atau satu mesin.

## 1. Identitas Hub
- **Nama:** System-Design-Architect-Hub
- **Fokus Utama:** distributed systems, system topology, service boundaries, scalability, availability, caching strategy, messaging, event-driven architecture, load balancing, failure-aware system design
- **Status di Learning Matrix:** pilar utama `RAK-05 Architecture Hubs`
- **Peran Umum:** macro system architecture, service decomposition, scaling strategy, resilience planning, traffic handling, distributed trade-off analysis
- **Persona Utama:** Distributed Systems Architect & Scalability Strategy Specialist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `VISUALIZE`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
System design penting dipelajari karena software yang sehat di level kode atau aplikasi tetap bisa runtuh ketika dipaksa melayani trafik, beban, dependensi, dan kebutuhan availability yang jauh lebih besar daripada kemampuan satu mesin tunggal.

Hub ini relevan ketika kita ingin memahami:
- kapan monolith masih cukup dan kapan tidak,
- bagaimana sistem dibagi tanpa memecahnya secara sembrono,
- bagaimana load, latency, failure, dan consistency memengaruhi desain,
- dan mengapa skalabilitas sejati adalah masalah trade-off, bukan sekadar menambah server.

Di dalam Learning Matrix, system design bukan sekadar kumpulan diagram high-level. Ia adalah disiplin untuk memahami bagaimana aplikasi benar-benar hidup di bawah beban, ketidakpastian, dan distribusi sumber daya.

## 3. Core DNA

### Load and Scale Awareness
System design selalu dimulai dari pertanyaan:
- beban datang dari mana,
- bottleneck ada di mana,
- dan apa yang sebenarnya harus diskalakan.

### Boundaries beyond Code
Di level ini, batas tidak lagi hanya antara module atau package.
Batas berubah menjadi:
- service boundaries,
- data ownership,
- communication paths,
- dan operational blast radius.

### Failure as a First-Class Reality
Kegagalan bukan edge case.
Network failure, timeout, retry storms, stale cache, queue lag, dan partial outage adalah realitas yang harus dipikirkan sejak desain.

### Trade-offs over Absolutes
System design sehat lahir dari kesadaran trade-off:
- consistency vs availability,
- latency vs durability,
- simplicity vs scale,
- synchronous clarity vs asynchronous resilience.

### Architecture under Operations
Desain sistem tidak berhenti di diagram.
Ia menyatu dengan:
- observability,
- deployment topology,
- rollout strategy,
- disaster recovery,
- dan operational discipline.

## 4. The How
Cara berpikir system design bertumpu pada satu prinsip besar: **rancang sistem sesuai tekanan nyata yang harus ia tanggung, lalu kelola trade-off-nya dengan sadar**.

Mental model penting di hub ini adalah:
- mulai dari kebutuhan bisnis dan traffic shape,
- petakan bottleneck utama,
- tentukan data ownership dan service boundaries,
- pilih komunikasi sinkron atau asinkron secara sadar,
- rancang cache dan storage sesuai pola beban,
- dan siapkan sistem untuk gagal secara terkendali, bukan runtuh total.

## 5. Kekuatan Utama
- Membantu melihat sistem sebagai jaringan komponen, bukan hanya aplikasi tunggal.
- Sangat kuat untuk memahami scalability dan availability.
- Menjernihkan kapan cache, queue, shard, replica, atau service split benar-benar dibutuhkan.
- Membantu tim menilai trade-off sebelum membangun terlalu jauh.
- Menjadi jembatan kuat antara storage, infrastructure, runtime, dan application boundaries.
- Sangat relevan untuk software yang mulai tumbuh besar atau mission-critical.

## 6. Trade-offs dan Kelemahan
- Mudah berubah menjadi terlalu abstrak jika tidak dibumi-kan ke traffic dan use case nyata.
- Bisa memicu over-engineering jika microservices dijadikan default.
- Diagram sistem yang rapi tidak menjamin desain operasional yang sehat.
- Fokus terlalu cepat ke distribusi bisa merusak tim yang belum siap secara delivery discipline.
- Tidak menggantikan kebutuhan akan application architecture atau desain internal software yang baik.

## 7. Use Case Prioritas
System design paling cocok untuk:
- high-traffic applications
- growing backend platforms
- distributed services
- API ecosystems
- event-driven systems
- caching and queue-heavy architectures
- availability-sensitive and latency-sensitive systems

Hub ini kurang ideal jika fokus utamanya adalah:
- aplikasi kecil yang masih sehat sebagai monolith sederhana
- diskusi folder structure atau code-level abstractions
- workflow aplikasi internal yang belum punya tekanan skala berarti
- eksplorasi teknis yang belum punya kebutuhan sistem nyata

## 8. Kapan Dipilih
Pilih hub ini ketika:
- satu aplikasi mulai tidak cukup menjelaskan seluruh sistem,
- traffic, latency, atau availability mulai menjadi concern nyata,
- ada kebutuhan service boundaries yang lebih tegas,
- sistem mulai bergantung pada cache, queue, replica, atau load balancing,
- atau Anda perlu memikirkan sistem dalam kondisi gagal dan bertumbuh.

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke hub ini ketika:
- masalah utama Anda masih di pemetaan actor, workflow, atau feature breakdown,
- codebase belum punya struktur dasar yang sehat,
- problem sebenarnya belum membenarkan distribusi sistem,
- atau tim masih butuh monolith yang rapi sebelum melompat ke arsitektur makro.

## 10. Posisi di Learning Matrix
System design paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  relevan lintas bahasa karena system design hidup di level topologi dan trade-off, bukan di level sintaks

- **Execution Hubs:**
  `Server-Runtime-Knowledge-Base`

- **Digital UI Hubs:**
  relevan secara tidak langsung melalui frontend-backend boundaries, latency impact, realtime delivery, dan user-facing system behavior

- **Storage Hubs:**
  `PostgreSQL-Knowledge-Base`, `Redis-Knowledge-Base`, `MongoDB-Knowledge-Base`, `Neo4j-Knowledge-Base`

- **Architecture Hubs:**
  `Application-Architecture-Hub`, `Repository-Architecture-Hub`, `Design-Patterns-Library`

- **Infrastructure Hubs:**
  sangat kuat karena system design bertemu langsung dengan deployment, compute, network, observability, and runtime operations

- **Version Control Hubs:**
  relevan untuk ADR, topology changes, service contracts, dan migration discipline saat sistem berevolusi

- **AI Orchestration Hubs:**
  relevan untuk architecture critique, bottleneck analysis, trade-off simulation, dan system decomposition assistance

- **Security Identity Hubs:**
  sangat relevan untuk trust boundaries, auth propagation, policy distribution, secrets management, dan attack surface thinking

## 11. Jalur Belajar Praktis
Contoh jalur belajar system design di dalam Learning Matrix:

### Jalur Backend Scalability
`Server Runtime -> PostgreSQL -> Redis -> System-Design-Architect-Hub`

### Jalur Product-to-Platform Growth
`Application-Architecture-Hub -> Repository-Architecture-Hub -> System-Design-Architect-Hub`

### Jalur Event-Driven Systems
`Golang -> Server Runtime -> Redis -> System-Design-Architect-Hub -> Infrastructure`

### Jalur Full-Stack System Awareness
`TypeScript -> JavaScript-TS-Frontend-Hub -> Application-Architecture-Hub -> System-Design-Architect-Hub`

## 12. Repository dan Workspace Terkait
Node System Design di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis system design di dalam Learning Matrix.

- **Workspace Kolektif Arsitektur:**
  `05-Architecture-Hubs`
  Perannya adalah menjadi area kerja arsitektur yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman System Design:**
  `05-Architecture-Hubs/System-Design-Architect-Hub`
  Perannya adalah menjadi workspace khusus untuk membedah system design jauh lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace System Design Perlu Dipisah
Workspace system design perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace system design boleh:
- menyimpan case studies,
- menyimpan topology diagrams,
- menyimpan load and bottleneck reasoning,
- menyimpan caching and messaging labs,
- menyimpan failure mode explorations,
- menyimpan architecture trade-off notes,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di System Design Workspace
Untuk pendalaman system design, struktur awal yang disarankan untuk workspace turunannya adalah 8 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: Load, Scale, and Problem Framing
Fokus:
- traffic shape,
- bottleneck identification,
- scalability goals,
- latency targets,
- dan kapan sebuah sistem benar-benar butuh desain makro yang lebih serius.

### RAK-02: Service Boundaries and Topology
Fokus:
- monolith vs modular monolith vs microservices,
- service decomposition,
- API gateway,
- ownership boundaries,
- dan topology mapping.

### RAK-03: Data, Consistency, and Ownership
Fokus:
- data ownership,
- transactional boundaries,
- replication,
- sharding,
- CAP-style trade-offs,
- dan consistency choices di level sistem.

### RAK-04: Caching, Messaging, and Asynchronous Flows
Fokus:
- caching strategy,
- queues,
- streams,
- event-driven architecture,
- retries,
- idempotency,
- dan asynchronous design trade-offs.

### RAK-05: Availability, Resilience, and Failure Modes
Fokus:
- SPOF,
- failover,
- circuit breakers,
- graceful degradation,
- timeout budgets,
- disaster thinking,
- dan resilience patterns di level sistem.

### RAK-06: Observability and Operational Design
Fokus:
- logging,
- metrics,
- tracing,
- alerting,
- SLO-minded thinking,
- dan operasi sistem yang bisa dipantau dan dipelihara.

### RAK-07: Delivery, Migration, and Evolution Strategy
Fokus:
- monolith decomposition,
- migration path,
- strangler thinking,
- rollout sequencing,
- compatibility strategy,
- dan evolusi arsitektur sistem tanpa merusak delivery.

### RAK-08: Bridge to Application, Storage, Runtime, and Infrastructure
Fokus:
- hubungan system design dengan application architecture,
- hubungan ke storage choices,
- hubungan ke server runtime dan infra topology,
- dan batas kapan code-level concerns harus naik ke system-level concerns.

Sub-rak yang layak untuk system design saat ini:

#### Sub-Rak: System Design to Storage Strategy
Fokus:
- bagaimana pilihan PostgreSQL, Redis, MongoDB, atau Neo4j memengaruhi topologi sistem.

#### Sub-Rak: System Design to Runtime and Services
Fokus:
- bagaimana runtime server, process model, dan service shape saling memengaruhi.

#### Sub-Rak: System Design to Infrastructure
Fokus:
- bagaimana deployment, networking, compute, observability, dan availability bertemu di level arsitektur sistem.

#### Sub-Rak: System Design to Security Boundaries
Fokus:
- trust zones,
- auth propagation,
- policy enforcement,
- dan blast radius thinking.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `System-Design-Architect-Hub` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi system design di dalam Learning Matrix.
- Workspace turunannya menjelaskan praktik system design secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning system design di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Architecture Lain
- **Dibanding Application-Architecture-Hub:** system design membahas topologi sistem dan distribusi beban, sedangkan application architecture membahas struktur aplikasi, role, dan workflow.
- **Dibanding Repository-Architecture-Hub:** system design hidup di level service topology dan operational architecture, sedangkan repository architecture hidup di level codebase organization.
- **Dibanding Design-Patterns-Library:** system design bekerja di level makro distribusi sistem, sedangkan design patterns bekerja di level software internals.

## 17. Pitfalls
- Memaksa microservices demi hype pada project yang belum membutuhkannya.
- Menggambar diagram bagus tanpa bottleneck analysis yang nyata.
- Mengabaikan failure modes dan observability.
- Menyebar data ownership tanpa discipline yang jelas.
- Mengandalkan cache atau queue tanpa memahami consistency cost.
- Naik terlalu cepat ke distribusi sebelum monolith dasar benar-benar sehat.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `05-Architecture-Hubs/Repository-Architecture-Hub`
- `05-Architecture-Hubs/Design-Patterns-Library`
- `04-Storage-Hubs`
- `06-Infrastructure-Hubs`
- `09-Security-Identity-Hubs`

Dokumen ini terutama berada pada level:
- primary architecture path
- distributed systems and macro topology
- scalability, availability, and failure-aware design

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `06-Infrastructure-Hubs`
- `09-Security-Identity-Hubs`
- `04-Storage-Hubs`
- dan node arsitektur lain yang paling relevan dengan sistem yang sedang dianalisis
