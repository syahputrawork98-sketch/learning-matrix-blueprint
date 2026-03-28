# MongoDB Knowledge Base

> Pusat pembelajaran untuk memahami penyimpanan document-oriented yang menekankan fleksibilitas bentuk data, object-shaped persistence, agregasi, dan skalabilitas horizontal untuk sistem yang tidak cocok dipaksa ke model relasional yang kaku.

## 1. Identitas Hub
- **Nama:** MongoDB-Knowledge-Base
- **Fokus Utama:** document-oriented storage, BSON documents, flexible schema, aggregation pipeline, indexing, replica sets, sharding, object-shaped persistence
- **Status di Learning Matrix:** pilar utama `RAK-04 Storage Hubs`
- **Peran Umum:** content-heavy storage, polymorphic data persistence, event and log-like data, flexible product data, rapidly evolving application data models
- **Persona Utama:** MongoDB Data Modeling Architect & Document Systems Specialist
- **Mode AI yang Relevan:** `DISCUSS`, `BLUEPRINT`, `SOURCE_SYNC`, `DRAFT`, `LAB`, `VISUALIZE`, `CURATE`, `SYNC`, `REVIEW`, `EXECUTE`

## 2. The Why
MongoDB penting dipelajari karena tidak semua data cocok disusun sebagai tabel relasional dengan struktur yang kaku dan relasi yang sangat eksplisit.

Hub ini relevan ketika kita ingin memahami:
- bagaimana data yang bentuknya berubah-ubah tetap bisa disimpan secara produktif,
- bagaimana objek aplikasi dapat dipetakan lebih langsung ke storage,
- bagaimana agregasi dapat membentuk informasi tanpa harus berpikir selalu dalam relasi tabel,
- dan mengapa fleksibilitas skema kadang lebih penting daripada keketatan relasional.

Di dalam Learning Matrix, MongoDB bukan pengganti universal untuk storage lain. Ia adalah jalur document-oriented untuk data yang lebih polymorphic, hierarkis, dan cepat berubah.

## 3. Core DNA

### Document-Centric Thinking
MongoDB menyimpan data sebagai dokumen, bukan baris tabel yang terpisah kaku.
Artinya, satu unit data sering kali mencerminkan bentuk objek aplikasi secara lebih langsung.

### Flexible Schema
MongoDB memungkinkan struktur data berubah lebih bebas.
Ini sangat berguna untuk:
- MVP,
- domain yang cepat berubah,
- katalog produk yang tidak seragam,
- dan data yang bentuknya tidak selalu identik antar entitas.

### Embedding over Excessive Joins
MongoDB sering lebih sehat ketika relasi lokal yang dekat disimpan sebagai embedded documents, bukan selalu dipisah menjadi struktur yang saling tergantung.

### Aggregation as Data Shaping
Aggregation pipeline adalah salah satu DNA utama MongoDB.
Ia memungkinkan transformasi, filtering, grouping, dan shaping data secara kuat di dalam database.

### Scale-Oriented Design
MongoDB sangat terkait dengan pemikiran:
- replica sets,
- sharding,
- distribution,
- dan skala horizontal
sebagai bagian dari arsitektur penyimpanan.

## 4. The How
Cara berpikir MongoDB bertumpu pada satu prinsip besar: **simpan data dalam bentuk yang dekat dengan kebutuhan aplikasi, lalu bentuk kembali data itu sesuai alur baca dan analisis yang nyata**.

Mental model penting di MongoDB adalah:
- bentuk dokumen harus mengikuti pola akses,
- embedding dan referencing harus dipilih secara sadar,
- schema flexibility harus tetap dijaga dengan disiplin,
- dan agregasi bukan sekadar fitur tambahan, melainkan alat utama untuk membentuk informasi.

## 5. Kekuatan Utama
- Sangat cocok untuk data yang bentuknya fleksibel dan cepat berubah.
- Memetakan objek aplikasi ke storage dengan lebih alami.
- Kuat untuk content-heavy systems dan katalog polymorphic.
- Aggregation pipeline memberi kemampuan shaping data yang kuat.
- Relevan untuk sistem yang perlu bertumbuh secara horizontal.

## 6. Trade-offs dan Kelemahan
- Fleksibilitas schema bisa berubah menjadi kekacauan jika tanpa disiplin.
- Integritas data antar dokumen tidak seketat model relasional.
- Embedding yang salah dapat membuat dokumen membengkak atau update menjadi mahal.
- Query dan indexing tetap perlu desain yang matang.
- Tidak semua problem data cocok diselesaikan secara document-oriented.

## 7. Use Case Prioritas
MongoDB paling cocok untuk:
- CMS and content platforms
- product catalogs with polymorphic attributes
- event or activity data
- log-like storage
- rapidly evolving application schemas
- document-centric APIs
- flexible internal products

Hub ini kurang ideal jika fokus utamanya adalah:
- strict transactional truth
- relational reporting-heavy systems
- hot ephemeral caching workloads
- graph-native relationship traversal

## 8. Kapan Dipilih
Pilih MongoDB ketika:
- bentuk data Anda cepat berubah,
- struktur antar entitas tidak selalu seragam,
- Anda ingin memetakan objek aplikasi lebih langsung ke storage,
- aggregations dan document shaping penting,
- atau Anda membutuhkan jalur scale-out yang lebih natural untuk document data.

## 9. Kapan Tidak Dipilih
Tunda fokus utama ke MongoDB ketika:
- integritas relasional sangat penting,
- transaksi kompleks adalah inti bisnis,
- data Anda sebenarnya lebih cocok sebagai cache atau transient state,
- atau problem Anda lebih natural dimodelkan sebagai graph.

## 10. Posisi di Learning Matrix
MongoDB paling kuat terhubung ke hub berikut:

- **Language Hubs:**
  `JavaScript-Knowledge-Base`, `TypeScript-Knowledge-Base`, `Python-Knowledge-Base`, `Golang-Knowledge-Base`

- **Execution Hubs:**
  `Server-Runtime-Knowledge-Base`

- **Digital UI Hubs:**
  relevan untuk product UIs, content-heavy apps, dashboards, dan systems yang membaca data berbentuk objek atau dokumen

- **Architecture Hubs:**
  `Application-Architecture-Hub`, `System-Design-Architect-Hub`

- **Infrastructure Hubs:**
  sangat relevan untuk replica sets, sharding, managed clusters, backups, monitoring, dan operational scale

- **Version Control Hubs:**
  relevan untuk schema evolution discipline, migration approaches, dan collection-level change management

- **AI Orchestration Hubs:**
  relevan untuk data shaping assistance, aggregation drafting, document modeling review, dan query reasoning

- **Security Identity Hubs:**
  relevan untuk auth-sensitive data, access control, role boundaries, and document-level exposure risks

## 11. Jalur Belajar Praktis
Contoh jalur belajar MongoDB di dalam Learning Matrix:

### Jalur Flexible Product Data
`TypeScript -> Server Runtime -> MongoDB -> Application Architecture`

### Jalur Content and CMS Builder
`JavaScript -> Server Runtime -> MongoDB -> Repository Architecture -> Infrastructure`

### Jalur Data-Shaping Backend
`Python -> Server Runtime -> MongoDB -> System Design`

### Jalur Operational Document Services
`Golang -> Server Runtime -> MongoDB -> Infrastructure -> Security`

## 12. Repository dan Workspace Terkait
Node MongoDB di dalam ekosistem ini terhubung ke beberapa layer repository yang berbeda:

- **Blueprint Induk:**
  `learning-matrix-blueprint`
  Perannya adalah menjelaskan posisi strategis MongoDB di dalam Learning Matrix.

- **Workspace Kolektif Storage:**
  `04-Storage-Hubs`
  Perannya adalah menjadi area kerja storage yang dapat berkembang setelah blueprint matang.

- **Workspace Pendalaman MongoDB:**
  `04-Storage-Hubs/MongoDB-Knowledge-Base`
  Perannya adalah menjadi workspace khusus untuk membedah MongoDB jauh lebih dalam daripada dokumen blueprint ini.

## 13. Mengapa Workspace MongoDB Perlu Dipisah
Workspace MongoDB perlu dipisah dari `learning-matrix-blueprint` karena kebutuhan keduanya berbeda.

`learning-matrix-blueprint` harus tetap:
- ringkas secara strategis,
- fokus pada hubungan antar hub,
- dan stabil sebagai peta induk.

Sementara workspace MongoDB boleh:
- menyimpan data modeling labs,
- menyimpan aggregation experiments,
- menyimpan indexing proofs,
- menyimpan embedding vs referencing studies,
- menyimpan sharding and replica notes,
- dan dibuka hanya saat memang dibutuhkan untuk pendalaman.

## 14. Struktur Rak Internal di MongoDB Workspace
Untuk pendalaman MongoDB, struktur awal yang disarankan untuk workspace turunannya adalah 7 rak utama. Jumlah rak ini dapat berkembang atau menyusut mengikuti kebutuhan domain dan bentuk workspace nyatanya:

### RAK-01: History and Landscape
Fokus:
- sejarah NoSQL,
- posisi MongoDB di industri,
- document model,
- dan alasan MongoDB dipilih untuk data yang fleksibel.

### RAK-02: Document Modeling Foundations
Fokus:
- BSON structure,
- collections,
- schema thinking,
- embedding vs referencing,
- dan fondasi model dokumen yang sehat.

### RAK-03: Querying and Aggregation
Fokus:
- filters,
- projections,
- updates,
- aggregation pipeline,
- stages,
- dan data shaping yang kuat di MongoDB.

### RAK-04: Indexing and Access Patterns
Fokus:
- indexing strategies,
- compound indexes,
- access patterns,
- query planning,
- dan performa pada document workloads.

### RAK-05: Application Patterns and Flexibility Trade-offs
Fokus:
- schema evolution,
- polymorphic collections,
- read-heavy and write-heavy trade-offs,
- dan bagaimana fleksibilitas tetap dijaga dengan disiplin.

### RAK-06: Internal Mechanics and Scale
Fokus:
- WiredTiger basics,
- journaling,
- replica sets,
- sharding,
- elections,
- dan skala operasional MongoDB.

### RAK-07: Language and System Bridges
Fokus:
- bagaimana MongoDB dipakai dari bahasa-bahasa utama,
- hubungan MongoDB dengan server runtime,
- hubungan MongoDB dengan system design, infrastructure, dan security,
- serta kapan MongoDB diposisikan sebagai primary document store.

Sub-rak yang layak untuk MongoDB saat ini:

#### Sub-Rak: MongoDB to JavaScript and TypeScript
Fokus:
- MongoDB dalam ekosistem JS/TS,
- hubungan object-shaped data dengan backend dan full-stack application design,
- serta alasan MongoDB terasa alami di jalur document-centric apps.

#### Sub-Rak: MongoDB to Python
Fokus:
- MongoDB dalam workflow Python,
- relasi ke data tools, flexible APIs, dan backend pragmatis.

#### Sub-Rak: MongoDB to Golang
Fokus:
- MongoDB dalam service Go,
- relasi ke backend yang butuh document flexibility tanpa meninggalkan performance discipline.

#### Sub-Rak: MongoDB to System Architecture
Fokus:
- peran MongoDB dalam application architecture,
- infrastructure scaling,
- dan system design untuk document-oriented systems.

## 15. Aturan Sinkronisasi Blueprint dan Workspace
Agar `learning-matrix-blueprint` dan `MongoDB-Knowledge-Base` tetap sinkron, gunakan aturan berikut:

- Dokumen blueprint ini menjelaskan posisi MongoDB di dalam Learning Matrix.
- Workspace MongoDB menjelaskan isi MongoDB secara rinci.
- Jika struktur rak internal berubah, positioning strategis di blueprint harus tetap dijaga.
- Jika positioning MongoDB di matrix berubah, workspace turunannya harus diperbarui agar tetap selaras.
- Blueprint tidak perlu menyalin isi teknis workspace secara mendalam.
- Workspace tidak boleh kehilangan tautan balik ke blueprint induknya.

## 16. Perbandingan Singkat dengan Node Storage Lain
- **Dibanding PostgreSQL:** MongoDB lebih fleksibel untuk document-oriented modeling, sementara PostgreSQL lebih kuat untuk integritas relasional dan transaksi ketat.
- **Dibanding Redis:** MongoDB lebih cocok untuk document persistence yang lebih tahan lama, sementara Redis lebih cocok untuk in-memory transient workloads.
- **Dibanding Neo4j:** MongoDB unggul untuk object-shaped documents, sementara Neo4j lebih cocok untuk relationship traversal yang graph-native.

## 17. Pitfalls
- Menganggap schema flexibility berarti schema boleh liar.
- Embedding berlebihan tanpa memikirkan update cost.
- Full collection scans karena indexing buruk.
- Aggregation pipelines yang kuat tetapi tidak dipahami performanya.
- Memakai MongoDB untuk problem yang sebenarnya lebih relasional atau graph-native.

## 18. Hub Connections
Dokumen ini terutama terhubung ke:
- `02-Execution-Hubs/Server-Runtime-Knowledge-Base`
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `06-Infrastructure-Hubs`
- `09-Security-Identity-Hubs`

Dokumen ini terutama berada pada level:
- primary storage path
- document-oriented flexibility and scale
- object-shaped persistence design

## 19. Next Steps
Setelah dokumen ini, pembaca sebaiknya lanjut ke:
- `02-Execution-Hubs/Server-Runtime-Knowledge-Base`
- `05-Architecture-Hubs/Application-Architecture-Hub`
- `05-Architecture-Hubs/System-Design-Architect-Hub`
- `06-Infrastructure-Hubs`
- lalu bandingkan dengan:
  - `PostgreSQL-Knowledge-Base`
  - `Redis-Knowledge-Base`
  - `Neo4j-Knowledge-Base`
