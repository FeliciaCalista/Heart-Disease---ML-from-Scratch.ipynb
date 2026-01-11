# Heart Disease Prediction – Machine Learning From Scratch

## Deskripsi Proyek

Proyek ini bertujuan untuk memprediksi risiko penyakit jantung menggunakan dataset **Heart Disease (`heart.csv`)** dengan pendekatan:

- Exploratory Data Analysis (EDA)
- Machine Learning
- Implementasi model **from scratch** (tanpa library ML siap pakai)

Fokus utama proyek ini adalah **memahami arsitektur dan matematika di balik model ML**, bukan hanya menghasilkan prediksi.

---

## Tujuan Proyek

1. Memahami karakteristik data kesehatan melalui EDA
2. Mengimplementasikan algoritma ML dari nol
3. Memahami:
   - Cara model belajar
   - Cara membuat prediksi

---

## Dataset

- **Nama**: Heart Disease Dataset
- **Kaggle**: `https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset`
- **Target**:
  - `0` → Tidak memiliki penyakit jantung
  - `1` → Memiliki penyakit jantung

Setelah penghapusan data duplikat, dataset berisi **302 sampel**.

---

## Exploratory Data Analysis (EDA)

Tahapan EDA meliputi:

### Pembersihan Data
- Menghapus data duplikat
- Mengecek missing values
- Validasi tipe data

### Analisis Distribusi Data
- Histogram:
  - Melihat sebaran data
  - Mengidentifikasi skewness
- Boxplot:
  - Mendeteksi outlier
  - Membandingkan distribusi antar kelas

### Analisis Hubungan Fitur
- Crosstab (`pd.crosstab`)
  - Digunakan untuk melihat hubungan antara fitur kategorikal dan target

---

## Preprocessing Data

- **Train-Test Split**
  - Menggunakan `stratify=y` agar distribusi kelas tetap seimbang
- **Feature Scaling**
  - Diperlukan untuk Logistic Regression
  - Tidak wajib untuk Decision Tree & Random Forest

---

## Model Machine Learning

### Logistic Regression (From Scratch)

**Tujuan:**
- Model baseline
- Mudah diinterpretasi
- Menghasilkan probabilitas secara matematis

**Konsep yang diimplementasikan:**
- Linear combination
- Sigmoid function
- Binary Cross-Entropy Loss
- Gradient Descent

---

### Decision Tree (From Scratch)

**Konsep utama:**
- Struktur node dan leaf
- Pemilihan split menggunakan **Gini Impurity**
- Rekursi
- Early stopping

---

### Random Forest (From Scratch)

**Prinsip kerja:**
- Ensemble dari beberapa Decision Tree
- Bootstrapping data
- Random feature selection
- Voting dan probability averaging

---

## Evaluasi Model

### Metrik Evaluasi:
- ROC-AUC
- Confusion Matrix
- Accuracy, Precision, Recall

