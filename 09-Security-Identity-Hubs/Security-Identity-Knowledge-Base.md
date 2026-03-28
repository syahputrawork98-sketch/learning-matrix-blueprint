# Security Identity Knowledge Base

> Pusat pembelajaran untuk memahami bagaimana sistem melindungi identitas, menjaga integritas data, mengendalikan akses, dan membangun boundary kepercayaan yang sehat di seluruh aplikasi dan layanan.

## 1. Identitas Hub
- **Nama:** Security-Identity-Knowledge-Base
- **Fokus Utama:** authentication, authorization, cryptography fundamentals, secrets handling, application security, OWASP-style risk mitigation, identity governance, trust boundary design
- **Status di Learning Matrix:** pilar utama `RAK-09 Security-Identity-Hubs`
- **Peran Umum:** identity and access modeling, application security posture, secrets discipline, defense-in-depth, trust-aware software design
- **Persona Utama:** Application Security Architect & Identity Governance Strategist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `LAB`, `VISUALIZE`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
Security dan identity penting dipelajari karena software yang bernilai selalu menarik risiko, dan satu boundary yang bocor dapat merusak seluruh nilai sistem, data, dan kepercayaan pengguna.

Hub ini relevan ketika kita ingin memahami:
- bagaimana identitas diverifikasi,
- bagaimana akses dibatasi,
- bagaimana rahasia dan data sensitif dijaga,
- dan bagaimana aplikasi membangun postur pertahanan yang sehat terhadap ancaman yang berulang.

Di dalam Learning Matrix, security/identity bukan fitur tambahan. Ia adalah fondasi kepercayaan yang membuat software layak dipakai di dunia nyata.

## 3. Core DNA

### Trust Boundary Thinking
Keamanan dimulai dari pertanyaan:
- siapa dipercaya,
- dalam konteks apa,
- untuk tindakan apa,
- dan di batas mana kepercayaan harus diuji ulang.

### Identity before Privilege
Sebelum memberi akses, sistem harus tahu:
- siapa pengguna atau layanan itu,
- bagaimana identitasnya diverifikasi,
- dan bagaimana session atau token dikelola.

### Authorization as Architecture
Akses tidak boleh jadi `if-else` acak di seluruh codebase.
Model izin adalah bagian dari arsitektur aplikasi dan sistem.

### Secrets and Cryptographic Discipline
Hashing, encryption, signing, key rotation, dan secrets handling harus dipahami sebagai praktik disiplin, bukan sihir hitam.

### AppSec as Continuous Posture
Security bukan checklist sekali jadi.
XSS, CSRF, SQLi, SSRF, token abuse, misconfiguration, dan data leakage harus dipahami sebagai ancaman yang perlu dijaga terus-menerus.

## 4. The How
Cara berpikir security/identity bertumpu pada satu prinsip besar: **kelola kepercayaan, akses, dan risiko secara sadar di seluruh jalur aplikasi**.

Mental model penting di hub ini adalah:
- sistem menerima request dari aktor tertentu,
- identitas harus diverifikasi,
- izin harus dinilai,
- data sensitif harus dilindungi,
- boundary harus dijaga di setiap titik penting,
- dan audit serta mitigasi harus mendukung respons saat sesuatu gagal.

## 5. Kekuatan Utama
- Membantu sistem menjaga trust dan data integrity.
- Membuat auth dan permission lebih arsitektural, bukan tambal sulam.
- Menurunkan risiko celah umum di level aplikasi.
- Menjadi jembatan penting ke runtime, storage, infrastructure, dan architecture.
- Sangat relevan untuk software yang menangani user, data, dan layanan nyata.
- Membentuk pola pikir defense-in-depth yang sehat.

## 6. Trade-offs dan Kelemahan
- Mudah berubah menjadi paranoia abstrak tanpa prioritas risiko yang jelas.
- Security posture yang buruk sering tersembunyi di balik flow yang tampak normal.
- Tooling auth dan security bisa terasa kompleks dan berat.
- Over-hardening di tempat yang salah dapat menghambat delivery.
- Tidak menggantikan kebutuhan akan discipline infra dan system design.

## 7. Use Case Prioritas
Security/identity paling cocok untuk:
- auth-heavy applications
- role-based systems
- APIs with user or service identity
- SaaS products
- admin systems
- systems handling sensitive data
- applications that need stronger AppSec posture

Hub ini kurang ideal jika fokus utamanya adalah:
- eksperimen kecil yang belum menyentuh identity atau data sensitif
- diskusi murni tentang deployment infra tanpa konteks keamanan aplikasi
- topik keamanan jaringan fisik atau hardening device di luar software boundary

## 8. Kapan Dipilih
Pilih hub ini ketika:
- aplikasi mulai punya user identities, roles, atau sessions,
- data sensitif mulai masuk sistem,
- auth dan permission mulai terasa rumit,
- tim butuh threat awareness yang lebih nyata,
- dan Anda ingin membangun boundary keamanan sebagai bagian dari arsitektur.

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke hub ini ketika:
- aplikasi masih sangat dini dan belum menyentuh identity atau trust boundaries,
- masalah utama masih di feature definition atau repo structure,
- Anda sedang membahas hardening infra tingkat spesifik tanpa konteks aplikasi,
- atau sistem belum punya kebutuhan keamanan yang melampaui dasar minimum.

## 10. Posisi di Learning Matrix
Security/identity paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  relevan ke semua language hubs yang menangani input, session, secrets, access, dan data boundary

- **Execution Hubs:**
  `Browser-Runtime-Knowledge-Base`, `Server-Runtime-Knowledge-Base`

- **Digital UI Hubs:**
  relevan untuk auth UX, session flows, trusted client boundaries, dan UI exposure risks

- **Storage Hubs:**
  `PostgreSQL-Knowledge-Base`, `Redis-Knowledge-Base`, `MongoDB-Knowledge-Base`, `Neo4j-Knowledge-Base`

- **Architecture Hubs:**
  `Application-Architecture-Hub`, `System-Design-Architect-Hub`, dan pada batas tertentu `Repository-Architecture-Hub`

- **Infrastructure Hubs:**
  `Infrastructure-DevOps-Knowledge-Base`

- **Version Control Hubs:**
  `Git-GitHub-Knowledge-Base`

- **AI Orchestration Hubs:**
  relevan untuk threat modeling assistance, auth flow review, policy drafting, dan security critique

- **Security Identity Hubs:**
  hub ini sendiri menjadi pusat pembelajaran trust, access, secrets, dan AppSec posture

## 11. Jalur Belajar Praktis
Contoh jalur belajar security/identity di dalam Learning Matrix:

### Jalur Frontend Trust Boundary Awareness
`Browser-Runtime-Knowledge-Base -> JavaScript-TS-Frontend-Hub -> Security-Identity-Knowledge-Base`

### Jalur Backend Access and Data Protection
`Server-Runtime-Knowledge-Base -> PostgreSQL -> Security-Identity-Knowledge-Base`

### Jalur Architecture-to-Security Discipline
`Application-Architecture-Hub -> Security-Identity-Knowledge-Base -> Infrastructure-DevOps-Knowledge-Base`

### Jalur Delivery and Access Governance
`Git-GitHub-Knowledge-Base -> Infrastructure-DevOps-Knowledge-Base -> Security-Identity-Knowledge-Base`

## 12. Repository dan Workspace Terkait
Node Security/Identity di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis security/identity di dalam Learning Matrix.

- **Workspace Kolektif Security:**
  `09-Security-Identity-Hubs`
  Perannya adalah menjadi area kerja security yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman Security/Identity:**
  `09-Security-Identity-Hubs/Security-Identity-Knowledge-Base`
  Perannya adalah menjadi workspace khusus untuk membedah praktik security dan identity lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace Security-Identity Perlu Dipisah
Workspace security/identity perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace security/identity boleh:
- menyimpan auth and session labs,
- menyimpan OAuth and OIDC notes,
- menyimpan JWT and token studies,
- menyimpan OWASP case breakdowns,
- menyimpan secrets management patterns,
- menyimpan permission matrix experiments,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di Security-Identity Workspace
Untuk pendalaman security/identity, struktur awal yang disarankan untuk workspace turunannya adalah 8 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: Security Foundations and Threat Models
Fokus:
- CIA triad,
- trust boundaries,
- threat modeling,
- zero trust mindset,
- dan attack surface basics.

### RAK-02: Cryptography, Hashing, and Secrets
Fokus:
- hashing,
- salting,
- encryption,
- signing,
- key management,
- dan secrets discipline.

### RAK-03: Authentication and Identity Flows
Fokus:
- sessions,
- tokens,
- OAuth 2.0,
- OIDC,
- SSO,
- dan identity lifecycle.

### RAK-04: Authorization and Access Control
Fokus:
- RBAC,
- ABAC,
- policy thinking,
- permission boundaries,
- service-to-service authorization,
- dan least privilege.

### RAK-05: Application Security and Common Risks
Fokus:
- OWASP-style risks,
- SQLi,
- XSS,
- CSRF,
- SSRF,
- injection and validation discipline,
- dan session abuse patterns.

### RAK-06: Security Operations inside Applications
Fokus:
- audit logging,
- key rotation,
- session revocation,
- rate limiting,
- anomaly detection,
- dan incident-aware design.

### RAK-07: Identity Providers, Tooling, and Ecosystem
Fokus:
- Auth0,
- Keycloak,
- internal auth services,
- security tooling,
- dan verification or scanning ecosystem.

### RAK-08: Bridge to Runtime, Storage, Architecture, and Infrastructure
Fokus:
- hubungan ke runtime trust boundaries,
- hubungan ke storage protection,
- hubungan ke application architecture,
- hubungan ke infrastructure and delivery,
- dan hubungan ke version control and secrets hygiene.

Sub-rak yang layak untuk security/identity saat ini:

#### Sub-Rak: Security to Browser and Server Runtime
Fokus:
- bagaimana runtime browser dan server membentuk trust boundary yang berbeda.

#### Sub-Rak: Security to Storage and Data Protection
Fokus:
- bagaimana storage choices memengaruhi data protection, token storage, dan secrets discipline.

#### Sub-Rak: Security to Application and System Architecture
Fokus:
- bagaimana role, workflow, service boundaries, dan topology memengaruhi model keamanan.

#### Sub-Rak: Security to Infrastructure and Git Governance
Fokus:
- bagaimana delivery, secrets handling, repository access, dan operational governance memengaruhi security posture.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `Security-Identity-Knowledge-Base` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi security/identity di dalam Learning Matrix.
- Workspace turunannya menjelaskan praktik security dan identity secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning security/identity di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Lain
- **Dibanding Infrastructure-DevOps-Knowledge-Base:** security/identity membahas trust, access, dan AppSec posture, sedangkan infrastructure/devops membahas delivery dan runtime operations.
- **Dibanding Application-Architecture-Hub:** application architecture membahas bentuk aplikasi, sedangkan security/identity membahas bagaimana bentuk itu dilindungi dan dibatasi.
- **Dibanding System-Design-Architect-Hub:** system design membahas topologi dan scale trade-offs, sedangkan security/identity membahas trust and access discipline yang hidup di atasnya.

## 17. Pitfalls
- Security by obscurity.
- Secret leaks.
- Token lifetime yang buruk.
- Auth flow yang tampak jalan tetapi boundary-nya rapuh.
- Role checks yang tersebar tanpa model arsitektural.
- Mengabaikan OWASP-style risks.
- Menganggap security sebagai checklist akhir.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `02-Execution-Hubs/Browser-Runtime-Knowledge-Base`
- `02-Execution-Hubs/Server-Runtime-Knowledge-Base`
- `04-Storage-Hubs`
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `06-Infrastructure-Hubs/Infrastructure-DevOps-Knowledge-Base`
- `07-Version-Control-Hubs/Git-GitHub-Knowledge-Base`

Dokumen ini terutama berada pada level:
- primary security path
- trust, identity, and access discipline
- application security and data protection awareness

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `06-Infrastructure-Hubs/Infrastructure-DevOps-Knowledge-Base`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `04-Storage-Hubs`
- dan node runtime atau aplikasi yang paling relevan dengan threat boundary yang sedang dipelajari
