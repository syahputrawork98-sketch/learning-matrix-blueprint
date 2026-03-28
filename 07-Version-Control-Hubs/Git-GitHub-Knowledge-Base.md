# Git GitHub Knowledge Base

> Pusat pembelajaran untuk memahami sejarah kode sebagai aset tim, mengelola kolaborasi asinkron dengan disiplin, dan menjaga integrasi perubahan agar tetap aman, dapat ditinjau, dan dapat ditelusuri.

## 1. Identitas Hub
- **Nama:** Git-GitHub-Knowledge-Base
- **Fokus Utama:** git internals, snapshots and DAG thinking, branching strategies, merge and rebase discipline, pull requests, code review, collaboration governance, repository history hygiene
- **Status di Learning Matrix:** pilar utama `RAK-07 Version-Control-Hubs`
- **Peran Umum:** version control literacy, asynchronous collaboration, review discipline, branch governance, commit and merge safety
- **Persona Utama:** Version Control Architect & Collaboration Governance Strategist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `LAB`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
Git dan GitHub penting dipelajari karena software modern dibangun secara kolaboratif, dan kualitas kolaborasi sangat ditentukan oleh kualitas sejarah perubahan yang disimpan serta governance integrasi yang dipakai tim.

Hub ini relevan ketika kita ingin memahami:
- bagaimana perubahan dicatat dengan rapi,
- bagaimana branch dipakai sebagai jalur kerja sementara,
- bagaimana pull request dan review menjadi mekanisme validasi,
- dan bagaimana riwayat kode dijaga tetap bisa dibaca, ditelusuri, dan dipulihkan.

Di dalam Learning Matrix, Git/GitHub bukan sekadar alat penyimpanan versi. Ia adalah sistem koordinasi kerja engineering.

## 3. Core DNA

### History as a First-Class Asset
Riwayat kode bukan sampingan.
Ia adalah memori tim tentang:
- apa yang berubah,
- kapan berubah,
- kenapa berubah,
- dan siapa yang mengubahnya.

### Snapshot and DAG Thinking
Git lebih sehat dipahami sebagai graph snapshot daripada tombol save.
Pemahaman ini membantu menjelaskan:
- branch,
- merge,
- rebase,
- conflict resolution,
- dan history inspection.

### Branches as Collaboration Lanes
Branch adalah jalur kerja sementara untuk memisahkan eksperimen, development, dan integrasi.
Ia bukan tempat bersembunyi selamanya.

### Review before Integration
Pull request dan code review penting karena perubahan sebaiknya masuk lewat proses yang:
- terlihat,
- bisa dikomentari,
- bisa divalidasi,
- dan bisa dipertanggungjawabkan.

### Governance over Repository Chaos
Version control yang sehat butuh aturan:
- ukuran PR,
- naming branch,
- commit discipline,
- review policy,
- merge policy,
- dan perlindungan branch utama.

## 4. The How
Cara berpikir Git/GitHub bertumpu pada satu prinsip besar: **kelola perubahan software sebagai sejarah kolaboratif yang tertib, bukan sebagai tumpukan revisi tanpa memori**.

Mental model penting di hub ini adalah:
- developer membuat perubahan lokal,
- Git mencatatnya sebagai sejarah yang terstruktur,
- branch memberi ruang kerja terpisah,
- pull request memberi ruang review dan validasi,
- dan governance menjaga integrasi tetap sehat saat tim bertumbuh.

## 5. Kekuatan Utama
- Menjaga kolaborasi tetap tertib.
- Membantu tim meninjau perubahan dengan lebih sehat.
- Memudahkan rollback, tracing, dan history inspection.
- Mengurangi chaos saat banyak developer bekerja paralel.
- Menjadi fondasi penting untuk release discipline dan delivery confidence.
- Relevan untuk semua codebase yang tumbuh serius.

## 6. Trade-offs dan Kelemahan
- Git bisa terasa membingungkan jika dipelajari hanya sebagai daftar perintah.
- Policy yang terlalu kaku bisa memperlambat alur kerja.
- Rebase, force push, dan merge strategy yang salah bisa merusak history.
- Tooling kolaborasi tidak otomatis menghasilkan budaya review yang sehat.
- Tidak menggantikan kebutuhan akan CI/CD dan deployment discipline.

## 7. Use Case Prioritas
Git/GitHub paling cocok untuk:
- team-based development
- asynchronous collaboration
- code review workflows
- branch and merge discipline
- repository history management
- open-source style contribution flow
- maintainable engineering governance

Hub ini kurang ideal jika fokus utamanya adalah:
- skrip personal sekali pakai yang hampir tidak punya lifecycle kolaboratif
- diskusi murni tentang deployment dan infra
- pembahasan desain aplikasi atau desain internal software tanpa konteks kolaborasi perubahan

## 8. Kapan Dipilih
Pilih hub ini ketika:
- tim mulai bekerja paralel di codebase yang sama,
- PR dan review mulai menjadi kebiasaan,
- konflik merge mulai sering muncul,
- history repo mulai sulit dibaca,
- dan Anda ingin membangun kolaborasi engineering yang lebih aman dan rapi.

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke hub ini ketika:
- project masih sangat kecil dan belum kolaboratif,
- problem utama masih di dasar coding atau struktur aplikasi,
- Anda sedang membahas pipeline deployment, bukan history governance,
- atau belum ada tekanan nyata pada branch, merge, atau review discipline.

## 10. Posisi di Learning Matrix
Git/GitHub paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  relevan ke semua language hubs yang menghasilkan codebase kolaboratif

- **Execution Hubs:**
  relevan secara tidak langsung karena perubahan pada runtime-facing code tetap masuk melalui history dan review discipline yang sama

- **Digital UI Hubs:**
  relevan untuk PR hygiene, UI refactor review, feature branch discipline, dan collaboration pada codebases frontend

- **Storage Hubs:**
  relevan untuk migration review, schema change discipline, dan koordinasi perubahan storage lintas tim

- **Architecture Hubs:**
  `Application-Architecture-Hub`, `Repository-Architecture-Hub`, `Design-Patterns-Library`

- **Infrastructure Hubs:**
  `Infrastructure-DevOps-Knowledge-Base`

- **Version Control Hubs:**
  hub ini sendiri menjadi pusat pembelajaran sejarah kode, integrasi perubahan, dan collaboration governance

- **AI Orchestration Hubs:**
  relevan untuk PR review assistance, commit hygiene review, merge strategy guidance, dan repository history analysis

- **Security Identity Hubs:**
  relevan untuk access control ke repository, branch protection, maintainer policy, dan auditability of changes

## 11. Jalur Belajar Praktis
Contoh jalur belajar Git/GitHub di dalam Learning Matrix:

### Jalur Product Change Governance
`Application-Architecture-Hub -> Repository-Architecture-Hub -> Git-GitHub-Knowledge-Base`

### Jalur Frontend Collaboration Discipline
`TypeScript -> JavaScript-TS-Frontend-Hub -> Git-GitHub-Knowledge-Base`

### Jalur Backend Delivery Coordination
`Golang -> Server-Runtime-Knowledge-Base -> Git-GitHub-Knowledge-Base -> Infrastructure-DevOps-Knowledge-Base`

### Jalur Repository-to-Release Hygiene
`Repository-Architecture-Hub -> Git-GitHub-Knowledge-Base -> Infrastructure-DevOps-Knowledge-Base`

## 12. Repository dan Workspace Terkait
Node Git/GitHub di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis Git/GitHub di dalam Learning Matrix.

- **Workspace Kolektif Version Control:**
  `07-Version-Control-Hubs`
  Perannya adalah menjadi area kerja version control yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman Git/GitHub:**
  `07-Version-Control-Hubs/Git-GitHub-Knowledge-Base`
  Perannya adalah menjadi workspace khusus untuk membedah version control dan collaboration governance lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace Git/GitHub Perlu Dipisah
Workspace Git/GitHub perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace Git/GitHub boleh:
- menyimpan Git internals notes,
- menyimpan branch and merge labs,
- menyimpan rebase and conflict simulations,
- menyimpan PR review conventions,
- menyimpan commit message standards,
- menyimpan hooks and policy experiments,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di Git/GitHub Workspace
Untuk pendalaman Git/GitHub, struktur awal yang disarankan untuk workspace turunannya adalah 8 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: Git Foundations and Mental Models
Fokus:
- snapshots,
- blobs, trees, dan commits,
- DAG thinking,
- HEAD,
- refs,
- dan model internal Git yang benar-benar penting.

### RAK-02: Local History and Change Craft
Fokus:
- staging,
- commits,
- amending,
- diff literacy,
- log reading,
- dan local history hygiene.

### RAK-03: Branching, Merging, and Rebasing
Fokus:
- branch strategy,
- merge mechanics,
- rebase discipline,
- conflict resolution,
- dan history shaping.

### RAK-04: Remote Collaboration and GitHub Flow
Fokus:
- remotes,
- fetch, pull, dan push,
- PR flow,
- branch protection,
- maintainer flow,
- dan async collaboration model.

### RAK-05: Code Review and Governance
Fokus:
- PR quality,
- review etiquette,
- gatekeeper policy,
- approval model,
- merge policy,
- dan collaboration hygiene.

### RAK-06: Commit Discipline and Repository Hygiene
Fokus:
- conventional commits,
- atomic changes,
- commit slicing,
- stale branches,
- cleanup discipline,
- dan readable history.

### RAK-07: Recovery, Safety, and Troubleshooting
Fokus:
- reflog,
- reset dan revert,
- detached HEAD,
- recovery flows,
- force push risks,
- dan safety discipline.

### RAK-08: Bridge to Repository, Delivery, and Team Operations
Fokus:
- hubungan ke repository architecture,
- hubungan ke CI/CD dan infra flow,
- hubungan ke team workflow,
- dan hubungan ke security and access governance.

Sub-rak yang layak untuk Git/GitHub saat ini:

#### Sub-Rak: Git/GitHub to Repository Architecture
Fokus:
- bagaimana bentuk codebase memengaruhi cara perubahan dipecah, ditinjau, dan diintegrasikan.

#### Sub-Rak: Git/GitHub to Infrastructure-DevOps
Fokus:
- bagaimana branch, PR, tag, dan release flow terhubung ke pipeline delivery dan deployment discipline.

#### Sub-Rak: Git/GitHub to Team Review Governance
Fokus:
- code review,
- maintainer policy,
- ownership,
- dan governance kolaborasi asinkron.

#### Sub-Rak: Git/GitHub to Security and Access Control
Fokus:
- repository access,
- branch protection,
- auditability,
- dan boundary keamanan di level kolaborasi kode.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `Git-GitHub-Knowledge-Base` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi Git/GitHub di dalam Learning Matrix.
- Workspace turunannya menjelaskan praktik version control dan collaboration secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning Git/GitHub di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Lain
- **Dibanding Repository-Architecture-Hub:** repository architecture membahas bentuk codebase, sedangkan Git/GitHub membahas sejarah perubahan dan governance integrasi codebase itu.
- **Dibanding Infrastructure-DevOps-Knowledge-Base:** Git/GitHub membahas collaboration dan history flow, sedangkan infrastructure/devops membahas build, deploy, dan operations flow.
- **Dibanding Application-Architecture-Hub:** application architecture membahas bentuk aplikasi, sedangkan Git/GitHub membahas bagaimana perubahan terhadap bentuk itu dikelola bersama.

## 17. Pitfalls
- Menganggap Git hanya tombol save.
- God PR yang terlalu besar.
- Rebase buta-buta pada branch bersama.
- Force push tanpa disiplin.
- Stale branches menumpuk.
- Commit history tidak bermakna.
- Review jadi formalitas tanpa kualitas nyata.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `05-Architecture-Hubs/Repository-Architecture-Hub`
- `06-Infrastructure-Hubs/Infrastructure-DevOps-Knowledge-Base`
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `09-Security-Identity-Hubs`

Dokumen ini terutama berada pada level:
- primary version control path
- collaboration and history governance
- review and integration discipline

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `06-Infrastructure-Hubs/Infrastructure-DevOps-Knowledge-Base`
- `05-Architecture-Hubs/Repository-Architecture-Hub`
- `09-Security-Identity-Hubs`
- dan language atau runtime hub yang paling dekat dengan codebase yang sedang dikelola
