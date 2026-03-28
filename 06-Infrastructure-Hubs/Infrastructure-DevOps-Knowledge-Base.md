# Infrastructure DevOps Knowledge Base

> Pusat pembelajaran untuk mengubah software dari kode yang berjalan lokal menjadi layanan yang dapat dibangun, dikirim, dijalankan, dipantau, dan dioperasikan secara andal di lingkungan nyata.

## 1. Identitas Hub
- **Nama:** Infrastructure-DevOps-Knowledge-Base
- **Fokus Utama:** containerization, CI/CD, Infrastructure as Code, cloud deployment, runtime operations, observability, secrets handling, release automation, delivery reliability
- **Status di Learning Matrix:** pilar utama `RAK-06 Infrastructure Hubs`
- **Peran Umum:** build and release automation, environment provisioning, deployment systems, runtime operations, production readiness
- **Persona Utama:** Platform Delivery Architect & DevOps Operations Strategist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `LAB`, `VISUALIZE`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
Infrastructure dan DevOps penting dipelajari karena software yang bagus tetap tidak bernilai jika tidak bisa dikirim, dijalankan, dan dioperasikan secara andal di lingkungan nyata.

Hub ini relevan ketika kita ingin memahami:
- bagaimana build dan deployment dibuat reproducible,
- bagaimana pipeline menggantikan ritual manual yang rapuh,
- bagaimana environment diprovision secara sadar,
- dan bagaimana operations menjaga sistem tetap sehat setelah rilis.

Di dalam Learning Matrix, infrastructure/devops bukan sekadar kumpulan tools. Ia adalah disiplin delivery dan operasi yang membuat software benar-benar hidup.

## 3. Core DNA

### Reproducible Delivery
Build dan deploy harus bisa diulang dengan hasil yang dapat dipercaya.
Jika rilis hanya bergantung pada memori manusia, sistem sedang menabung risiko.

### Automation over Manual Ritual
Semakin penting suatu langkah, semakin tidak sehat jika ia dikerjakan secara manual.
Automation bukan kemewahan, tetapi cara menjaga konsistensi.

### Environment as a Designed System
Local, staging, dan production bukan tempat ajaib yang berdiri sendiri.
Masing-masing adalah environment yang harus dirancang, dipahami, dan dijaga drift-nya.

### Infrastructure as Code
Provisioning tidak boleh hidup hanya di kepala orang atau perintah terminal yang tak terdokumentasi.
Infra harus punya bentuk yang bisa ditinjau, diuji, dan diulang.

### Operations as Continuous Responsibility
Deployment bukan garis akhir.
Monitoring, rollback, secrets, cost, incident awareness, dan runtime safety adalah bagian dari arsitektur delivery itu sendiri.

## 4. The How
Cara berpikir infrastructure/devops bertumpu pada satu prinsip besar: **ubah delivery software menjadi sistem yang dapat diulang, diamati, dan dioperasikan dengan disiplin**.

Mental model penting di hub ini adalah:
- code lahir di repository,
- build menghasilkan artefak,
- pipeline memvalidasi dan mengirim artefak,
- infra menyediakan tempat hidup,
- runtime menjalankan layanan,
- observability memberi mata,
- dan operations menjaga sistem tetap sehat setelah rilis.

## 5. Kekuatan Utama
- Membuat delivery lebih aman dan dapat diulang.
- Mengurangi ketergantungan pada deploy manual.
- Menjembatani codebase dengan production reality.
- Sangat relevan untuk scaling tim dan sistem.
- Membantu menjaga reliability, security, dan release cadence.
- Menjadi fondasi untuk operasi software modern.

## 6. Trade-offs dan Kelemahan
- Mudah berubah menjadi tool-chasing tanpa pemahaman prinsip.
- Pipeline dan infra bisa terlalu rumit untuk kebutuhan kecil.
- Automasi yang buruk dapat mempercepat kerusakan, bukan mencegahnya.
- Biaya cloud dan operasional bisa membengkak jika tanpa disiplin.
- Tidak menggantikan kebutuhan akan arsitektur aplikasi dan system design yang sehat.

## 7. Use Case Prioritas
Infrastructure/devops paling cocok untuk:
- containerized services
- CI/CD pipelines
- cloud deployment
- staging and production delivery
- IaC workflows
- release automation
- environment management
- operational readiness

Hub ini kurang ideal jika fokus utamanya adalah:
- project sekali pakai yang tidak punya lifecycle operasional berarti
- diskusi murni tentang feature design
- code-level design tanpa kebutuhan delivery nyata
- sistem yang masih terlalu kecil untuk membawa banyak kompleksitas infra sekaligus

## 8. Kapan Dipilih
Pilih hub ini ketika:
- software perlu dideploy secara konsisten,
- tim mulai butuh pipeline yang bisa dipercaya,
- environment mulai berbeda-beda dan menyulitkan,
- kebutuhan observability, rollback, atau secrets handling mulai muncul,
- dan Anda ingin bergerak dari "bisa jalan" ke "bisa dioperasikan".

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke hub ini ketika:
- aplikasi masih sangat dini dan belum butuh delivery discipline besar,
- problem utama masih di pemetaan product/application structure,
- tim belum butuh automation yang kompleks,
- atau Anda sedang membahas desain software internal, bukan operational delivery.

## 10. Posisi di Learning Matrix
Infrastructure/devops paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  relevan ke semua language hubs yang menghasilkan artefak dan service deployable

- **Execution Hubs:**
  `Server-Runtime-Knowledge-Base`

- **Digital UI Hubs:**
  relevan secara tidak langsung melalui delivery frontend assets, deployment path, CDN concerns, dan release discipline

- **Storage Hubs:**
  `PostgreSQL-Knowledge-Base`, `Redis-Knowledge-Base`, `MongoDB-Knowledge-Base`, `Neo4j-Knowledge-Base`

- **Architecture Hubs:**
  `Repository-Architecture-Hub`, `System-Design-Architect-Hub`, dan pada batas tertentu `Application-Architecture-Hub`

- **Infrastructure Hubs:**
  hub ini sendiri menjadi pusat orkestrasi delivery, runtime environment, dan operasi sistem

- **Version Control Hubs:**
  sangat relevan untuk pipeline triggers, release discipline, config changes, ADRs, dan deployment-safe collaboration

- **AI Orchestration Hubs:**
  relevan untuk pipeline review, IaC drafting, deployment troubleshooting, dan observability assistance

- **Security Identity Hubs:**
  sangat relevan untuk secrets handling, access to cloud resources, runtime trust boundaries, dan operational safety

## 11. Jalur Belajar Praktis
Contoh jalur belajar infrastructure/devops di dalam Learning Matrix:

### Jalur Backend Delivery and Operations
`Golang -> Server Runtime -> PostgreSQL -> System-Design-Architect-Hub -> Infrastructure-DevOps-Knowledge-Base`

### Jalur Codebase-to-Production Discipline
`Repository-Architecture-Hub -> Infrastructure-DevOps-Knowledge-Base -> Security`

### Jalur Runtime and Release Automation
`Python -> Server Runtime -> Redis -> Infrastructure-DevOps-Knowledge-Base`

### Jalur Full Delivery Awareness
`Application-Architecture-Hub -> Repository-Architecture-Hub -> Infrastructure-DevOps-Knowledge-Base`

## 12. Repository dan Workspace Terkait
Node Infrastructure/DevOps di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis infrastructure/devops di dalam Learning Matrix.

- **Workspace Kolektif Infrastruktur:**
  `06-Infrastructure-Hubs`
  Perannya adalah menjadi area kerja infrastruktur yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman Infrastructure/DevOps:**
  `06-Infrastructure-Hubs/Infrastructure-DevOps-Knowledge-Base`
  Perannya adalah menjadi workspace khusus untuk membedah praktik delivery dan operasi lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace Infrastructure/DevOps Perlu Dipisah
Workspace infrastructure/devops perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace infrastructure/devops boleh:
- menyimpan Docker labs,
- menyimpan CI pipeline examples,
- menyimpan Terraform experiments,
- menyimpan deployment notes,
- menyimpan secrets management patterns,
- menyimpan observability and operations checklists,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di Infrastructure/DevOps Workspace
Untuk pendalaman infrastructure/devops, struktur awal yang disarankan untuk workspace turunannya adalah 8 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: Delivery Mindset and Environment Model
Fokus:
- local vs staging vs production,
- reproducibility,
- environment drift,
- operational lifecycle,
- dan release mindset.

### RAK-02: Containers and Build Artifacts
Fokus:
- Docker,
- image layering,
- multi-stage builds,
- runtime image discipline,
- dan artifact packaging.

### RAK-03: CI and Verification Pipelines
Fokus:
- CI workflows,
- build validation,
- test gates,
- lint or type or test orchestration,
- dan pipeline reliability.

### RAK-04: CD and Release Delivery
Fokus:
- deployment flows,
- rollout strategies,
- rollback thinking,
- release automation,
- dan environment promotion.

### RAK-05: Infrastructure as Code and Provisioning
Fokus:
- Terraform,
- provisioning model,
- reproducible infra,
- state discipline,
- dan cloud resource definition.

### RAK-06: Cloud Runtime and Platform Operations
Fokus:
- VM and container runtime,
- Kubernetes basics,
- networking and runtime topology,
- scaling operations,
- dan platform concerns di lingkungan nyata.

### RAK-07: Secrets, Observability, and Operational Safety
Fokus:
- secrets handling,
- logging,
- metrics,
- tracing,
- alerting,
- cost awareness,
- dan operational safeguards.

### RAK-08: Bridge to Architecture, Runtime, and Security
Fokus:
- hubungan ke repository architecture,
- hubungan ke system design,
- hubungan ke server runtime,
- hubungan ke storage,
- dan hubungan ke security identity.

Sub-rak yang layak untuk infrastructure/devops saat ini:

#### Sub-Rak: Infrastructure to Repository Architecture
Fokus:
- bagaimana bentuk codebase memengaruhi delivery pipelines, config placement, dan scripts organization.

#### Sub-Rak: Infrastructure to System Design
Fokus:
- bagaimana topology sistem memengaruhi deployment model, runtime environments, dan operational strategy.

#### Sub-Rak: Infrastructure to Runtime and Storage
Fokus:
- bagaimana runtime server dan pilihan storage memengaruhi packaging, deployment, dan day-2 operations.

#### Sub-Rak: Infrastructure to Security Identity
Fokus:
- secrets,
- cloud access boundaries,
- operational trust zones,
- dan runtime safety.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `Infrastructure-DevOps-Knowledge-Base` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi infrastructure/devops di dalam Learning Matrix.
- Workspace turunannya menjelaskan praktik infra/devops secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning infrastructure/devops di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Architecture Lain
- **Dibanding Repository-Architecture-Hub:** repository architecture membentuk codebase, sedangkan infrastructure/devops membentuk delivery dan operational path codebase itu.
- **Dibanding System-Design-Architect-Hub:** system design membahas topologi dan trade-off sistem, sedangkan infrastructure/devops membahas bagaimana sistem itu dibangun, diprovision, dideploy, dan dijaga.
- **Dibanding Server-Runtime-Knowledge-Base:** runtime membahas tempat program hidup, sedangkan infrastructure/devops membahas bagaimana tempat hidup itu disiapkan dan dioperasikan.

## 17. Pitfalls
- Deploy manual tanpa reproducibility.
- Secret leakage.
- Pipeline rapuh.
- Tool adoption tanpa prinsip.
- Cloud billing shock.
- Overengineering infra untuk kebutuhan kecil.
- Mengabaikan observability dan rollback path.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `02-Execution-Hubs/Server-Runtime-Knowledge-Base`
- `04-Storage-Hubs`
- `05-Architecture-Hubs/Repository-Architecture-Hub`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `09-Security-Identity-Hubs`

Dokumen ini terutama berada pada level:
- primary infrastructure path
- delivery, deployment, and operations discipline
- production readiness and runtime safety

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `09-Security-Identity-Hubs`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `04-Storage-Hubs`
- dan runtime atau language hub yang paling relevan dengan layanan yang sedang dideploy
