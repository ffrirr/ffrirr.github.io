# Spec Kit — Personal GitHub Page Feri Irawan

Personal website satu halaman (single-page) untuk menampilkan profil profesional sebagai **Odoo Developer** dengan struktur rapi, modern, dan mudah dikembangkan.

---

## 1. Tujuan & Sasaran

- Menjadi _online CV_ / portfolio utama yang mudah diakses (link di CV, LinkedIn, email).
- Menampilkan profil profesional sebagai **Odoo Developer** dengan fokus pada:
  - Skills teknis (Python, PostgreSQL, Odoo Framework, Docker, Git, API, dll). :contentReference[oaicite:0]{index=0}  
  - Pengalaman kerja (Arkana, MileApp, Prosa.ai, Zenius). :contentReference[oaicite:1]{index=1}  
  - Proyek Odoo dan integrasi yang relevan dengan HR, attendance, dan omnichannel. :contentReference[oaicite:2]{index=2}  
  - Pendidikan & sertifikasi yang memperkuat branding sebagai tech professional. :contentReference[oaicite:3]{index=3}  

- Mengarahkan recruiter/client untuk:
  - Mengunduh CV (PDF).
  - Menghubungi via email / WhatsApp / LinkedIn.

---

## 2. Teknologi & Stack

- **Frontend:**
  - HTML5 + CSS3 + JavaScript
  - **Tailwind CSS** (direkomendasikan) _atau_ Bootstrap 5 untuk styling cepat dan konsisten.
- **Ikon:**
  - Font Awesome (CDN) untuk ikon sosial, skills, dan kontak.
- **Hosting:**
  - GitHub Pages (branch `main` / `gh-pages`).
- **Struktur file utama:**
  - `index.html`
  - `style.css` (jika tidak menggunakan Tailwind full CDN) _atau_ `tailwind.config.js` (kalau pakai build)
  - `script.js`
  - `README.md`
  - `/assets/` (opsional)
    - `/assets/img/profile.jpg`
    - `/assets/img/projects/...`
    - `/assets/docs/CV_Feri_Irawan.pdf`

---

## 3. Informasi Arsitektur & Section

Single-page layout dengan navigasi scroll ke anchor:

1. **Hero**
2. **About Me**
3. **Skills**
4. **Experience**
5. **Projects**
6. **Education**
7. **Contact**
8. Footer

### 3.1 Hero Section

**Tujuan:**
- Memberikan kesan pertama yang kuat.
- Menyampaikan headline profesional dalam 1–2 kalimat.
- CTA: “Download CV” dan “Contact Me”.

**Elemen:**

- Foto profil (bisa siluet/avatar profesional).
- Headline:
  - `Odoo Developer`
  - Subheadline: ringkasan singkat seperti:
    > Odoo Developer dengan pengalaman membangun modul kustom, integrasi API, dan solusi HR/Payroll berbasis Odoo.
- CTA Button:
  - `Download CV` (link ke `/assets/docs/CV_Feri_Irawan.pdf`)
  - `Contact Me` (scroll ke section Contact)
- Ikon sosial:
  - Email (`mailto:`)
  - LinkedIn (`linkedin.com/in/frrwn98`)
  - WhatsApp / Phone (klik untuk open `wa.me/` atau `tel:`)

**Font Awesome (contoh):**

- `fa-brands fa-linkedin`
- `fa-solid fa-envelope`
- `fa-solid fa-phone`
- `fa-brands fa-github` (dapat ditambahkan walau belum banyak repo).

---

### 3.2 About Me

**Tujuan:**
- Menjelaskan profil profesional secara singkat, padat, dan relevan dengan role Odoo Developer.

**Konten utama (sekali lagi dalam bahasa first person, “saya”):**

- 2–3 paragraf ringkas:
  - Latar belakang sebagai Odoo Developer.
  - Keahlian utama: desain modul, kustomisasi workflow, integrasi API, troubleshooting, performance tuning. :contentReference[oaicite:4]{index=4}  
  - Value yang dibawa: scalable solutions, support end-user, dokumentasi yang rapi.

**Contoh struktur isi:**

- Paragraf 1: Siapa saya, role utama, dan fokus tech.
- Paragraf 2: Pengalaman di Arkana dan jenis solusi yang pernah dibangun.
- Paragraf 3: Pendekatan kerja (problem-solving, kolaborasi, dokumentasi).

---

### 3.3 Skills

**Tujuan:**
- Memvisualisasikan kemampuan teknis dan soft skills secara terstruktur.

**Subkategori Skills:**

1. **Programming & ERP**
   - Python
   - PostgreSQL
   - Odoo Framework
   - XML, QWeb
   - REST/JSON, SQL :contentReference[oaicite:5]{index=5}  

2. **DevOps & Tools**
   - Docker
   - Git
   - CI/CD Pipelines

3. **Other Skills**
   - Problem-Solving
   - Debugging & Troubleshooting
   - Documentation
   - Project Management

**Desain:**

- Grid cards / badges dengan ikon:
  - `fa-brands fa-python`
  - `fa-solid fa-database`
  - `fa-solid fa-box` (untuk Docker)
  - `fa-brands fa-git-alt`
  - `fa-solid fa-code-branch` (untuk CI/CD)
  - `fa-solid fa-bug` (debugging)
  - `fa-solid fa-file-lines` (documentation)
  - `fa-solid fa-diagram-project` (project management)

Opsional: gunakan visual bar/progress “level” (Intermediate / Advanced) tapi jangan terlalu gimmicky; fokus pada readibility.

---

### 3.4 Experience

**Tujuan:**
- Menampilkan timeline pengalaman kerja dengan fokus pada hasil/impact.

**Data dari CV:**

- **Junior Odoo Developer — Arkana Solusi Digital, PT**
  - Feb 2024 – Present
  - Poin utama:
    - Desain & implementasi custom Odoo modules.
    - Custom workflow → mengurangi manual processing time ±70%.
    - Reporting system → waktu generate report turun signifikan.
    - Integrasi REST/JSON API dari/ke aplikasi eksternal.
    - Optimasi SQL & business logic → peningkatan backend performance ±40%.
    - Support & troubleshooting + dokumentasi teknis.
    - Kontribusi di agile sprint & deliver 20+ fitur. :contentReference[oaicite:6]{index=6}  

- **Data Annotation — MileApp (Nov 2023 – Dec 2023)**

- **Quality Assurance & Data Annotation — Prosa.ai (Jun 2023 – Nov 2023)**

- **Content Creator — Zenius (Mar 2021 – Sep 2021)**

**Desain:**

- Vertical timeline / cards dengan:
  - Nama perusahaan, posisi, periode waktu.
  - 3–5 bullet highlights yang ditulis professional, fokus ke hasil (impact-driven).

---

### 3.5 Projects

**Tujuan:**
- Showcase proyek kunci yang relevan dengan Odoo & integrasi.

**Daftar Projects (dari CV):**

1. **Odoo Human Capital Management (HCM) Suite – PT NOK Indonesia**
   - Scope: Odoo 17 HR suite (attendance, overtime, payroll, leave).
   - Highlight:
     - Portal karyawan untuk lembur, time-off, attendance, approval.
     - Tier-based approval workflow.
     - Payroll reports & dashboards untuk HR analysis. :contentReference[oaicite:7]{index=7}  

2. **Odoo Attendance Integration – PT Jakarta Post**
   - Integrasi fingerprint → Odoo Attendance.
   - Sinkronisasi check-in/out → HR accuracy meningkat. :contentReference[oaicite:8]{index=8}  

3. **Odoo HCM Suite – PT Karya Pacific Shipping (Jakarta)**
   - Full HR suite: recruitment, payroll, attendance, overtime, leave.
   - Integrasi multiple biometric devices (Solution, ZKTeco, Fingerspot).
   - Self-service portal & automated workflows. :contentReference[oaicite:9]{index=9}  

4. **Odoo–Jubelio Integration – Margaria Group**
   - Integrasi Odoo dengan Jubelio Omnichannel.
   - Automasi sinkronisasi produk, sales order, inventory updates.
   - Real-time data flow untuk operasional retail. :contentReference[oaicite:10]{index=10}  

**Desain:**

- Project cards (3–4 kolom di desktop, 1 kolom di mobile).
- Setiap card:
  - Nama project.
  - Perusahaan & stack (Odoo 17, API, Biometric, Jubelio, dll).
  - 3 bullet highlight.
- Ikon:
  - `fa-solid fa-people-group` (HR/HCM)
  - `fa-solid fa-fingerprint` (attendance)
  - `fa-solid fa-arrows-rotate` (integrasi)
  - `fa-solid fa-shop` (retail/omnichannel)

---

### 3.6 Education

**Data:**

- **Institut Teknologi Bandung (2015 – 2020)**
  - Bachelor’s Degree, Geological/Geophysical Engineering :contentReference[oaicite:11]{index=11}  

**Desain:**

- Satu card sederhana dengan:
  - Logo kecil (generic graduation cap icon).
  - Nama kampus, jurusan, tahun.

Ikon:
- `fa-solid fa-graduation-cap`

---

### 3.7 Certifications

**Data:**

- Odoo Functional Training  
- SQL (Advanced) Certificate  
- Python (Basic) Certificate  
- Google Project Management Professional Certificate  
- Google Data Analytics Professional Certificate :contentReference[oaicite:12]{index=12}  

**Desain:**

- Bisa digabung di section Education atau dibuat subsection kecil.
- List dengan icon `fa-solid fa-certificate`.

---

### 3.8 Contact

**Tujuan:**
- Mempermudah recruiter/klien menghubungi.

**Elemen:**

- Informasi:
  - Lokasi: South Jakarta, Indonesia.
  - Email: `frrwn98@gmail.com`
  - Phone/WhatsApp: `081371822644`
  - LinkedIn: `linkedin.com/in/frrwn98` :contentReference[oaicite:13]{index=13}  

- Form kontak sederhana:
  - Name
  - Email
  - Subject
  - Message
  - Tombol `Send`
  - Untuk GitHub Pages (static), form bisa:
    - Dikirim via mailto (simple) **atau**
    - Menggunakan layanan form eksternal (Formspree, Netlify Forms) — bisa disiapkan placeholder action.

Ikon:
- `fa-solid fa-location-dot`
- `fa-solid fa-envelope`
- `fa-solid fa-phone`
- `fa-brands fa-linkedin`

---

## 4. Desain Visual & UX

### 4.1 Warna Tema

Tema profesional, clean, dan modern.

**Palet (contoh):**

- **Primary:** Navy / Indigo
  - `#1F2933` atau `#1E293B`
- **Secondary / Accent:**
  - `#2563EB` (blue) atau `#0EA5E9` (cyan)
- **Background:**
  - `#0F172A` (untuk hero dark) + `#F3F4F6` / `#FFFFFF` (section lain)
- **Text:**
  - `#0F172A` / `#111827` (dark text)
  - `#E5E7EB` (text on dark bg)
- **Border / Divider:**
  - `#E5E7EB` / `#374151`

Style:
- Banyak whitespace.
- Card dengan shadow halus dan rounded (`border-radius: 0.75rem`).
- Hover state untuk tombol & cards (transform: scale(1.02), shadow sedikit lebih besar).

---

### 4.2 Typography

- Font utama: sistem atau Google Fonts:
  - `Inter`, `Poppins`, atau `Nunito`.
- Hierarki:
  - H1: 2.25rem–3rem (Hero title).
  - H2: 1.75rem–2rem (section title).
  - Body: 1rem–1.125rem.

---

### 4.3 Layout & Responsiveness

- **Desktop:**
  - Max width konten: `max-width: 1080px` atau `1200px` (centered).
  - 2 kolom untuk section seperti About Me (teks + foto), Projects (card grid).
- **Tablet:**
  - 2 kolom → 1 kolom jika minim lebar.
- **Mobile:**
  - Single column stack.
  - Navigasi responsive (hamburger menu dengan slide-down).

**Navigasi:**

- Sticky nav di top.
- Links: `Home`, `About`, `Skills`, `Experience`, `Projects`, `Education`, `Contact`.
- Smooth scrolling.

---

## 5. Interaksi & JavaScript (script.js)

Minimal, fokus pada UX:

1. **Navbar:**
   - Smooth scroll ke section ketika klik nav link.
   - Highlight active section (optional).

2. **Scroll Reveal (optional, non-essensial):**
   - Animasi fade-in atau slide-in ketika section muncul di viewport.

3. **Hamburger Menu (Mobile):**
   - Toggle show/hide nav links.

---

## 6. Struktur File & Folder

```text
root/
├─ index.html
├─ style.css          # jika tidak pakai Tailwind build; kalau pakai, boleh style tambahan
├─ script.js
├─ README.md
└─ assets/
   ├─ img/
   │  ├─ profile.jpg
   │  └─ project-*.png
   └─ docs/
      └─ CV_Feri_Irawan.pdf
