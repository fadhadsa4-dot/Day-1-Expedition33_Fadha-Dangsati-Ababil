# Day-1-Expedition33_Fadha Dangsati Ababil
# Dokumentasi Workshop: From AI to GitHub

**Nama Lengkap:** Fadha Dangsati Ababil
**Program Studi:** D4 Teknik Multimedia dan Jaringan (TMJ 1B)

---

## Deskripsi Repository

Repository ini berisi dokumentasi pribadi selama mengikuti workshop **"From AI to GitHub: Building with AI, Managing Change with GitHub"**. Isinya mencakup rangkuman materi, catatan pembelajaran, dan poin-poin penting seputar pemanfaatan kecerdasan buatan (AI) untuk membangun aplikasi serta pengelolaan perubahan kode menggunakan Git dan GitHub.

## Tujuan Repository

1. Menjadi pusat penyimpanan dokumentasi dan catatan workshop secara daring dan terstruktur.
2. Melatih penggunaan GitHub sebagai media pengelolaan dan publikasi dokumentasi proyek di bidang Teknologi Informasi dan Komunikasi (TIK).
3. Menjadi bahan belajar ulang tentang prompt engineering, version control, dan kolaborasi pengembangan perangkat lunak.
4. Membiasakan penulisan dokumentasi menggunakan format Markdown.

## Informasi Kegiatan Workshop

| Keterangan | Detail |
|---|---|
| Judul | From AI to GitHub: Building with AI, Managing Change with GitHub |
| Pemateri | Nugi Farhan (Senior Product Designer) |
| Tanggal | 07/11/2026 |
| Topik utama | Prompt Engineering, Git, GitHub, dan pembuatan aplikasi sederhana (Student Task Planner) |

### Capaian Pembelajaran Workshop

- Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
- Mengidentifikasi repository, commit, branch, dan pull request.
- Membedakan Git dan GitHub.
- Melakukan version controlling.

---

## Dokumentasi Materi

### 1. Prompt Engineering

**Materi:** Prompt engineering adalah cara merancang instruksi agar AI memberikan jawaban yang tepat, relevan, dan layak digunakan. Prompt bisa berupa pertanyaan sederhana, kata kunci, instruksi rumit, atau potongan kode.

**Rangkuman:**

- Konteks sangat menentukan kualitas hasil. Prompt singkat seperti "Create student task planner" menghasilkan jawaban yang umum, sedangkan prompt dengan konteks menghasilkan aplikasi yang lebih sesuai kebutuhan.
- Struktur prompt yang baik terdiri dari empat unsur:
  - **Role**: peran yang diminta dari AI.
  - **Task**: tugas atau tujuan yang ingin dicapai.
  - **Context**: kebutuhan, batasan, dan latar belakang.
  - **Format**: bentuk output yang diinginkan.
- Taktik menulis prompt yang baik:
  - Gunakan kata kerja aksi untuk menentukan tindakan.
  - Tentukan panjang dan format output.
  - Tentukan target audiens.
  - Sertakan fakta dan data yang relevan.
  - Rujuk sumber atau dokumen tertentu.
  - Definisikan istilah dan konsep kunci.
- Keuntungan prompt engineering: performa model AI meningkat, bias dan respons ofensif berkurang, kontrol dan prediktabilitas bertambah, serta pengalaman pengguna lebih baik.

**Poin penting:** Semakin jelas role, task, context, dan format dalam prompt, semakin kecil kemungkinan AI memberi jawaban yang melenceng. Hasil dari AI tetap perlu diverifikasi sebelum digunakan.

### 2. Git dan GitHub

**Materi:** Pengenalan Git sebagai version control system dan GitHub sebagai platform kolaborasi.

**Rangkuman:**

- **Git** adalah sistem version control terdistribusi (DVCS) yang melacak siapa, kapan, dan apa yang berubah pada suatu file. Git dibuat oleh Linus Torvalds pada tahun 2005 dan bekerja secara lokal.
- **GitHub** adalah platform berbasis web untuk menyimpan repository Git secara online dan mendukung kolaborasi.
- Alur kerja Git memiliki tiga area:
  - **Working directory**: salinan satu versi proyek yang sedang dikerjakan di komputer.
  - **Staging area (index)**: tempat menampung perubahan yang akan dimasukkan ke commit berikutnya.
  - **Git directory (repository)**: tempat Git menyimpan metadata dan object database proyek. Bagian inilah yang disalin saat melakukan clone.

**Poin penting:** Git dan GitHub adalah dua hal berbeda. Git adalah alat pelacak versinya, sedangkan GitHub adalah tempat menyimpan dan membagikannya secara online.

### 3. Perintah Dasar Git

| Perintah | Fungsi |
|---|---|
| `git init` | Memulai repository baru |
| `git add .` | Memindahkan file ke staging area |
| `git commit -m "pesan"` | Menyimpan perubahan ke repository |
| `git remote add <name> <url>` | Menghubungkan repository lokal ke repository di GitHub |
| `git push origin main` | Mengirim perubahan ke GitHub |
| `git pull origin main` | Mengambil perubahan dari GitHub dan menggabungkannya |
| `git clone "url"` | Menyalin repository dari GitHub ke komputer |

Variasi perintah `git add`:

- `git add --all` dan `git add -A` berfungsi sama, yaitu menambahkan semua perubahan ke staging area.
- `git add .` menambahkan semua file pada direktori saat ini beserta isinya.
- `git add *` menambahkan file yang dimodifikasi atau baru, tetapi tidak file yang dihapus.

**Poin penting:** Urutan dasar bekerja dengan Git adalah `add` → `commit` → `push`.

### 4. Setup Lingkungan Kerja

**Rangkuman:**

- **Git:** instal Git sesuai perangkat, cek dengan `git --version`, lalu atur identitas dengan `git config --global user.name` dan `git config --global user.email`. Periksa hasilnya dengan `git config --global --list`.
- **VS Code:** instal VS Code, lalu pasang perintah `code` ke PATH melalui Command Palette (`Ctrl+Shift+P` atau `Cmd+Shift+P`) dan cek dengan `code --version`.
- **SSH key:** buat kunci dengan `ssh-keygen -t ed25519 -C "email@domain.com"`, daftarkan kunci publik (`.pub`) di pengaturan *SSH and GPG keys* pada GitHub, lalu uji koneksi dengan `ssh -T git@github.com`.
- Ed25519 adalah skema tanda tangan digital berbasis kurva eliptik yang dirancang untuk keamanan dan performa tinggi.

**Poin penting:** Hanya kunci publik (`.pub`) yang boleh didaftarkan ke GitHub. Kunci privat tidak boleh dibagikan atau diunggah.

### 5. Praktik: Student Task Planner

**Rangkuman:** Praktik workshop adalah membuat aplikasi web sederhana bernama *Student Task Planner* untuk membantu mahasiswa tahun pertama mencatat tugas dan tenggat waktu. Alur praktiknya:

1. Gunakan platform AI (Claude, Antigravity, atau ChatGPT).
2. Tulis prompt untuk membuat aplikasi web.
3. Tambahkan proyek ke Git dengan `git init`.
4. Commit dan push ke GitHub.
5. Lakukan perubahan, lalu commit dan push kembali.

**Poin penting:** Version control membuat setiap perubahan pada proyek tercatat, sehingga mudah dilacak dan dikelola.

---

## Pengetahuan Baru yang Dipelajari

- Prompt yang terstruktur (role, task, context, format) menghasilkan jawaban AI yang lebih tepat dan mudah digunakan.
- Git dan GitHub memiliki fungsi berbeda, tetapi saling melengkapi dalam pengelolaan proyek.
- Perubahan kode dicatat melalui tiga tahap: working directory, staging area, lalu repository.
- GitHub dapat dimanfaatkan sebagai media dokumentasi dan publikasi, bukan hanya untuk menyimpan kode.

## Struktur Repository

```
.
├── README.md
└── (file dokumentasi tambahan)
```

---

*Dokumentasi ini disusun oleh Fadha Dangsati Ababil sebagai bagian dari misi proyek workshop.*
