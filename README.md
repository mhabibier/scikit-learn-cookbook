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

## 📌 Progress Pembelajaran (Chapters 1–5 Milestone)

| Chapter | Topik & Cakupan Materi | Notebook | Status | Quick Run |
|---|---|---|---|:---:|
| **01** | **Common Conventions & API Elements**<br>Estimators, transformers, `fit()`/`transform()`, custom classes, Pipelines, hyperparameter search, and metadata tags | [Chapter 1](01_Common_Conventions_and_API_Elements.ipynb) | ✅ Complete | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mhabibier/scikit-learn-cookbook/blob/main/01_Common_Conventions_and_API_Elements.ipynb) |
| **02** | **Pre-Model Workflow & Preprocessing**<br>Data quality audit, missing values, scaling, categorical encoding (`ColumnTransformer`), feature engineering, and robust leakage-free pipelines | [Chapter 2](02_Pre_Model_Workflow_and_Data_Preprocessing.ipynb) | ✅ Complete | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mhabibier/scikit-learn-cookbook/blob/main/02_Pre_Model_Workflow_and_Data_Preprocessing.ipynb) |
| **03** | **Dimensionality Reduction Techniques**<br>PCA (variance preservation & geometric rotation), Linear Discriminant Analysis (LDA), t-SNE visualization on high-dimensional data, and clustering comparison | [Chapter 3](03_Dimensionality_Reduction_Techniques.ipynb) | ✅ Complete | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mhabibier/scikit-learn-cookbook/blob/main/03_Dimensionality_Reduction_Techniques.ipynb) |
| **04** | **Distance Metrics & Nearest Neighbors**<br>KNN classification & regression, metrics comparison (Euclidean, Manhattan, Chebyshev), hyperparameter tuning via `GridSearchCV`, and decision boundary analysis | [Chapter 4](04_Distance_Metrics_and_Nearest_Neighbors.ipynb) | ✅ Complete | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mhabibier/scikit-learn-cookbook/blob/main/04_Distance_Metrics_and_Nearest_Neighbors.ipynb) |
| **05** | **Linear Models & Regularization**<br>Ordinary Least Squares (OLS), multicollinearity diagnosis, L1/L2 regularization (Ridge, Lasso, ElasticNet), coefficient paths, Polynomial regression, and Spline basis | [Chapter 5](05_Linear_Models_and_Regularization.ipynb) | ✅ Complete | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mhabibier/scikit-learn-cookbook/blob/main/05_Linear_Models_and_Regularization.ipynb) |
| 06 | Logistic Regression: Multiclass, Regularization, and Evaluation | — | ⏳ Planned | — |
| 07 | Support Vector Machines & Kernel Methods | — | ⏳ Planned | — |
| 08 | Decision Trees, Random Forests, and Ensemble Methods | — | ⏳ Planned | — |
| 09 | Text Processing and Multiclass Classification | — | ⏳ Planned | — |
| 10 | Clustering Techniques and Cluster Evaluation | — | ⏳ Planned | — |
| 11 | Novelty and Outlier Detection | — | ⏳ Planned | — |
| 12 | Cross-Validation and Model Evaluation | — | ⏳ Planned | — |
| 13 | Model Deployment and Maintenance | — | ⏳ Planned | — |

> **Milestone Catatan:** Target pemenuhan tugas perkuliahan untuk Bab 1 sampai 5 selesai sebelum **10 Oktober 2026 pukul 23:59 WIB**. Bab 6–13 dicantumkan sebagai cakupan keseluruhan buku teks.

---

## 🔍 Ringkasan Isi Setiap Notebook

Setiap notebook disusun secara terstruktur dengan standar akademik:
1. **Reproducibility & Environment:** Menggunakan seed acak tetap (`random_state=42`), pengecekan versi library, dan pemisahan data train-test sebelum proses fitting untuk mencegah *data leakage*.
2. **Implementasi Resep Buku:** Reproduksi akurat dari kode rujukan buku dengan adaptasi modern scikit-learn 1.5+.
3. **Analisis Teoretis & Interpretasi Hasil:** Pembahasan mendalam dalam Bahasa Indonesia mengenai cara kerja algoritma, asumsi matematis, visualisasi interaktif, dan keterbatasan model.
4. **Latihan Mandiri & Pertanyaan Refleksi:** Menguji performa model pada berbagai skenario dataset sintetis maupun riil.

### Sorotan Teknis per Bab:
- **Chapter 1:** Menelaah arsitektur konsisten scikit-learn (`fit`, `transform`, `predict`), pembuatan custom transformer dengan `BaseEstimator` dan `TransformerMixin`, otomatisasi alur kerja melalui `Pipeline`, serta eksplorasi metadata tags API.
- **Chapter 2:** Pipeline pembersihan data lengkap tanpa kebocoran (*leakage-free*). Menggunakan `ColumnTransformer` untuk memproses fitur numerik (imputasi median + standardisasi) dan kategorikal (one-hot encoding) secara terpisah, dilengkapi mekanisme fallback dataset offline (California Housing vs Diabetes).
- **Chapter 3:** Eksplorasi reduksi dimensi linear tanpa supervisi (PCA) vs dengan supervisi (LDA), analisis varians kumulatif, serta reduksi dimensi nonlinier probabilistik (t-SNE pada dataset Digits) beserta evaluasi clustering KMeans pada manifold tereduksi.
- **Chapter 4:** Eksplorasi geometri metrik jarak pada dataset non-linear (Noisy Circles & Checkerboard), optimasi parameter $k$ dan bobot jarak menggunakan `GridSearchCV`, learning curve, serta perbandingan KNN klasifikasi dan regresi.
- **Chapter 5:** Diagnostik multikolinearitas OLS, visualisasi *regularization paths* pada Ridge ($L_2$), Lasso ($L_1$), dan ElasticNet ($L_1 + L_2$), validasi silang otomatis (`RidgeCV`, `LassoCV`, `ElasticNetCV`), hingga penanganan non-linearitas menggunakan `PolynomialFeatures` dan `SplineTransformer`.

---

## 📂 Struktur Repositori

```text
scikit-learn-cookbook/
├── .gitignore                                       # Konfigurasi ignore file Python, Jupyter, dan IDE
├── LICENSE                                          # Lisensi Open Source (MIT)
├── README.md                                        # Dokumentasi utama proyek
├── requirements.txt                                 # Dependensi library Python
├── 01_Common_Conventions_and_API_Elements.ipynb      # Notebook Chapter 1
├── 02_Pre_Model_Workflow_and_Data_Preprocessing.ipynb # Notebook Chapter 2
├── 03_Dimensionality_Reduction_Techniques.ipynb     # Notebook Chapter 3
├── 04_Distance_Metrics_and_Nearest_Neighbors.ipynb   # Notebook Chapter 4
└── 05_Linear_Models_and_Regularization.ipynb         # Notebook Chapter 5
```

---

## 🚀 Panduan Menjalankan Notebook

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

## 📚 Referensi & Sumber Primer

1. **Buku Rujukan:** Sukup, John. *scikit-learn Cookbook: Over 80 Recipes for Machine Learning in Python with scikit-learn*, 3rd Edition, Packt Publishing, 2025.
2. **Official Repository:** [PacktPublishing/scikit-learn-Cookbook-Third-Edition](https://github.com/PacktPublishing/scikit-learn-Cookbook-Third-Edition)
3. **Dokumentasi Resmi:** [scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html) & [scikit-learn Common Pitfalls](https://scikit-learn.org/stable/common_pitfalls.html)

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).
