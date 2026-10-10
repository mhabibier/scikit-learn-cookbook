# scikit-learn Cookbook

[![Python Version](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.5%2B-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Code reproduction, visual evaluations, and theoretical explanations from John Sukup's ***scikit-learn Cookbook***, Third Edition (Packt Publishing, 2025). Repositori ini berisi notebook Jupyter mandiri untuk setiap bab dengan implementasi resep kode serta pembahasan dan analisis komprehensif dalam Bahasa Indonesia.

---

### Identitas Mahasiswa

- **Nama:** Muhammad Habibie Rabbani
- **Kelas:** TK-47-04
- **Program Studi:** S1 Teknik Komputer, Telkom University
- **Mata Kuliah:** Machine Learning

---



---

## Panduan Menjalankan Notebook

### Opsi 1: Google Colab (Tanpa Setup Lokal)
Klik tombol **Open In Colab** pada tabel di atas untuk membuka notebook langsung di Google Colab. Pilih menu **Runtime → Restart session and run all** (atau tekan `Ctrl + F9`).

### Opsi 2: Eksekusi Lokal (Python 3.9+)

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/mhabibier/scikit-learn-cookbook.git
   cd scikit-learn-cookbook
   ```

2. **Buat dan aktifkan virtual environment:**
   - **Windows (PowerShell):**
     ```powershell
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
   - **Linux / macOS:**
     ```bash
     python3 -m venv .venv
     source .venv/bin/activate
     ```

3. **Install seluruh dependensi:**
   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. **Jalankan Jupyter Notebook / JupyterLab:**
   ```bash
   jupyter notebook
   ```

> **Catatan Mode Offline (Chapter 2):** Jika lingkungan lokal Anda tidak memiliki koneksi internet untuk mengunduh dataset California Housing, set environment variable berikut sebelum menjalankan Jupyter:
> ```bash
> # Windows PowerShell
> $env:SCIKIT_COOKBOOK_OFFLINE="1"
> # Linux/macOS
> export SCIKIT_COOKBOOK_OFFLINE=1
> ```

---

##  Referensi & Sumber Primer

1. **Buku Rujukan:** Sukup, John. *scikit-learn Cookbook: Over 80 Recipes for Machine Learning in Python with scikit-learn*, 3rd Edition, Packt Publishing, 2025.
2. **Official Repository:** [PacktPublishing/scikit-learn-Cookbook-Third-Edition](https://github.com/PacktPublishing/scikit-learn-Cookbook-Third-Edition)
3. **Dokumentasi Resmi:** [scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html) & [scikit-learn Common Pitfalls](https://scikit-learn.org/stable/common_pitfalls.html)

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).
