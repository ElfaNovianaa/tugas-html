# RISK REGISTER - KELENGKAPAN R-07 hingga R-12

## R-07: Keterlambatan Proyek

| Field | Value |
|-------|-------|
| **REF ID** | R-07 |
| **RISK** | Keterlambatan Proyek (gagal memenuhi milestone yang sudah ditetapkan) |
| **RISK OWNER** | Giovan Lado |
| **RISK TRIGGER** | Estimasi waktu yang salah di awal proyek atau tim teknis kewalahan menghadapi isu integrasi yang kompleks dan tak terduga |
| **RISK CATEGORY** | Schedule/Time Management |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 3 |
| **PI SCORE** | 6 |
| **EXPECTED RESULT \| NO ACTION** | Proyek gagal mencapai target waktu, berdampak negatif pada kredibilitas tim dan Project Manager, potensi pembengkakan biaya |
| **POSITIVE RISK RESPONSE** | ENHANCE |
| **NEGATIVE RISK RESPONSE** | MITIGATE |
| **RESPONSE TRIGGER** | Milestone terancam terlewat atau kompleksitas teknis melebihi estimasi |
| **RESPONSE OWNER** | Project Manager |
| **RESPONSE DESCRIPTION** | Tambahkan buffer waktu 15% pada Time Management Plan untuk menghadapi risiko tak terduga, komunikasi proaktif dengan stakeholder mengenai potensi keterlambatan, review progress mingguan |
| **EXPECTED RESPONSE IMPACT** | Proyek dapat diselesaikan tepat waktu dengan buffer yang memadai, stakeholder terinformasi dengan baik, kredibilitas tim terjaga |

---

## R-08: Defect Leakage (Kegagalan Uji Coba)

| Field | Value |
|-------|-------|
| **REF ID** | R-08 |
| **RISK** | Defect Leakage (Kegagalan Uji Coba) |
| **RISK OWNER** | Aryasatya Widyatna Akbar |
| **RISK TRIGGER** | Skenario pengujian (test case) tidak mencakup seluruh edge case kritis (misalnya memutus jaringan saat proses bayar) sehingga bug lolos ke produksi |
| **RISK CATEGORY** | Quality Assurance/Testing |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 3 |
| **PI SCORE** | 6 |
| **EXPECTED RESULT \| NO ACTION** | Bug yang lolos menyebabkan sengketa pembayaran atau perhitungan diskon salah, kepercayaan pelanggan menurun, kerugian finansial |
| **POSITIVE RISK RESPONSE** | ENHANCE |
| **NEGATIVE RISK RESPONSE** | MITIGATE |
| **RESPONSE TRIGGER** | Fase User Acceptance Testing dimulai atau ditemukan gap dalam test coverage |
| **RESPONSE OWNER** | QA Expert, Backend Developer |
| **RESPONSE DESCRIPTION** | Review dan tingkatkan test coverage ke 100% untuk semua flow pembayaran kritis, QA Expert wajib melakukan Uji Keamanan dan Uji Ekstrim (misal: simulasi koneksi terputus saat transaksi, test perhitungan diskon hingga akurat 100%) |
| **EXPECTED RESPONSE IMPACT** | Semua bug kritis tertangkap sebelum Go-Live, sistem berjalan tanpa defect mayor, perhitungan pembayaran akurat sempurna |

---

## R-09: Scope Creep (Penambahan Ruang Lingkup)

| Field | Value |
|-------|-------|
| **REF ID** | R-09 |
| **RISK** | Scope Creep (Penambahan Ruang Lingkup) |
| **RISK OWNER** | Giovan Lado |
| **RISK TRIGGER** | Stakeholder (Manajemen Indogrosir) secara lisan meminta fitur yang belum disetujui setelah project scope dikunci, tanpa penambahan waktu dan anggaran |
| **RISK CATEGORY** | Scope Management |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 3 |
| **PI SCORE** | 6 |
| **EXPECTED RESULT \| NO ACTION** | Proyek melanggar batas waktu yang ditetapkan, anggaran membengkak, tim menjadi overworked, kualitas deliverable menurun |
| **POSITIVE RISK RESPONSE** | SHARE |
| **NEGATIVE RISK RESPONSE** | TRANSFER |
| **RESPONSE TRIGGER** | Stakeholder mengajukan permintaan fitur baru atau perubahan scope setelah scope dikunci |
| **RESPONSE OWNER** | Project Manager |
| **RESPONSE DESCRIPTION** | Terapkan Change Request Form formal, scope dikunci dan setiap perubahan harus disetujui Executive Sponsor dengan penyesuaian waktu dan anggaran, Project Manager secara rutin me-review Scope Statement dengan stakeholder |
| **EXPECTED RESPONSE IMPACT** | Scope terkontrol dengan baik, setiap perubahan terdokumentasi dan disetujui formal, waktu dan anggaran tetap sesuai rencana |

---

## R-10: Ketergantungan/Kegagalan Vendor (Vendor Lock-in Risk)

| Field | Value |
|-------|-------|
| **REF ID** | R-10 |
| **RISK** | Ketergantungan/Kegagalan Vendor (Vendor Lock-in Risk) |
| **RISK OWNER** | Bayu Brigas Novaldi |
| **RISK TRIGGER** | Vendor Payment Gateway utama tiba-tiba menghentikan layanan, mengubah struktur pricing secara drastis, atau mengalami masalah operasional internal yang berkepanjangan dan tak terduga |
| **RISK CATEGORY** | Vendor Management/External Dependencies |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 3 |
| **PI SCORE** | 6 |
| **EXPECTED RESULT \| NO ACTION** | Sistem utama pembayaran tidak berfungsi sama sekali, seluruh transaksi tidak dapat terjadi, proyek berisiko gagal total, kerugian revenue signifikan |
| **POSITIVE RISK RESPONSE** | EXPLOIT |
| **NEGATIVE RISK RESPONSE** | AVOID |
| **RESPONSE TRIGGER** | Vendor utama mengalami downtime berkepanjangan atau mengumumkan perubahan layanan signifikan |
| **RESPONSE OWNER** | Project Manager, Backend Developer, Security Engineer |
| **RESPONSE DESCRIPTION** | Integrasi Dual Vendor: mengidentifikasi dan mulai mengintegrasikan Vendor Pembayaran Sekunder (Backup Vendor), Modular Design agar migrasi ke vendor baru dapat dilakukan cepat, Legal Review untuk memastikan klausul kontrak mencakup penalti downtime yang ketat |
| **EXPECTED RESPONSE IMPACT** | Business continuity terjaga dengan backup vendor, tidak ada single point of failure, sistem dapat beralih vendor dengan minimal downtime |

---

## R-11: Dokumentasi yang Tidak Akurat

| Field | Value |
|-------|-------|
| **REF ID** | R-11 |
| **RISK** | Dokumentasi yang Tidak Akurat |
| **RISK OWNER** | Pradana Figo Ariansya |
| **RISK TRIGGER** | Technical writer gagal mencatat pembaruan sistem dan riwayat penanganan risiko, menyebabkan developer di masa depan membuat kesalahan |
| **RISK CATEGORY** | Documentation/Knowledge Management |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 2 |
| **PI SCORE** | 4 |
| **EXPECTED RESULT \| NO ACTION** | Kesalahan pengoperasian oleh staf atau developer baru di masa depan, maintenance sistem menjadi sulit, knowledge loss saat pergantian tim |
| **POSITIVE RISK RESPONSE** | ENHANCE |
| **NEGATIVE RISK RESPONSE** | MITIGATE |
| **RESPONSE TRIGGER** | Update sistem dilakukan atau ada perubahan konfigurasi penting |
| **RESPONSE OWNER** | Technical Writer, QA Expert, Backend Developer |
| **RESPONSE DESCRIPTION** | Dokumentasi harus ditinjau dan disetujui oleh QA Expert dan Lead Developer setiap kali ada update sistem, Technical Writer rutin mencatat seluruh riwayat penanganan risiko sebagai Lessons Learned, buat SOP dokumentasi yang jelas |
| **EXPECTED RESPONSE IMPACT** | Dokumentasi selalu up-to-date dan akurat, knowledge transfer berjalan lancar, maintenance sistem lebih mudah, developer baru dapat onboard dengan cepat |

---

## R-12: Kinerja Sistem Menurun (Degradasi Performance)

| Field | Value |
|-------|-------|
| **REF ID** | R-12 |
| **RISK** | Kinerja Sistem Menurun (Degradasi Performance) |
| **RISK OWNER** | Elfa Noviana Sari |
| **RISK TRIGGER** | Query database yang tidak dioptimalkan atau kurangnya implementasi caching saat sistem mulai menerima trafik tinggi |
| **RISK CATEGORY** | Performance/System Optimization |
| **PROBABILITY (1-3)** | 2 |
| **IMPACT (1-3)** | 3 |
| **PI SCORE** | 6 |
| **EXPECTED RESULT \| NO ACTION** | Transaksi lambat atau gagal, response time meningkat drastis, antrian menumpuk (mirip Downtime Server), user experience buruk, pelanggan kecewa |
| **POSITIVE RISK RESPONSE** | ENHANCE |
| **NEGATIVE RISK RESPONSE** | MITIGATE |
| **RESPONSE TRIGGER** | Response time sistem melebihi threshold yang ditetapkan atau Load Testing menunjukkan degradasi performance |
| **RESPONSE OWNER** | Back-End Developer, Project Manager |
| **RESPONSE DESCRIPTION** | Rutin melakukan Load Testing (misalnya dengan JMeter) untuk simulasi concurrent users sebelum soft launch, Back-End Developer fokus pada optimasi query database dan implementasi caching, monitoring performance real-time dengan tools APM |
| **EXPECTED RESPONSE IMPACT** | Sistem tetap responsif bahkan saat high traffic, query database teroptimasi, response time konsisten cepat, user experience tetap smooth |

---

## PROBABILITY KEY (1-3)
- **1 = Low**: Kemungkinan kecil terjadi (0-33%)
- **2 = Medium**: Kemungkinan sedang terjadi (34-66%)
- **3 = High**: Kemungkinan besar terjadi (67-100%)

## IMPACT KEY (1-3)
- **1 = Low**: Dampak minimal terhadap proyek
- **2 = Medium**: Dampak sedang terhadap proyek (waktu/biaya/kualitas)
- **3 = High**: Dampak signifikan terhadap proyek (dapat menyebabkan kegagalan)

## POSITIVE RISK RESPONSE STRATEGIES
- **EXPLOIT**: Memastikan peluang positif benar-benar terjadi
- **ENHANCE**: Meningkatkan kemungkinan atau dampak positif
- **SHARE**: Berbagi risiko positif dengan pihak ketiga
- **ACCEPT**: Menerima risiko tanpa tindakan aktif

## NEGATIVE RISK RESPONSE STRATEGIES
- **AVOID**: Menghilangkan ancaman dengan menghilangkan penyebabnya
- **MITIGATE**: Mengurangi kemungkinan atau dampak risiko
- **TRANSFER**: Mengalihkan dampak risiko ke pihak ketiga
- **ACCEPT**: Menerima risiko dan konsekuensinya
