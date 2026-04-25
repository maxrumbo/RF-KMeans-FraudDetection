# Machine Learning Clustering Classification

Repository ini berisi proyek machine learning end-to-end yang berfokus pada dua task utama:

1. Clustering untuk segmentasi pola transaksi.
2. Classification untuk memprediksi label target hasil clustering.

Seluruh pipeline dikerjakan menggunakan Python di Jupyter Notebook, lalu model disimpan sebagai artefak untuk evaluasi dan reuse.

## Tujuan Proyek

- Membangun model clustering berbasis fitur transaksi.
- Melakukan reduksi dimensi untuk analisis lanjutan.
- Menghasilkan dataset turunan yang memiliki kolom Target.
- Melatih model klasifikasi dari hasil clustering.
- Melakukan eksplorasi model alternatif dan tuning hyperparameter.

## Dataset

Dataset utama terkait pola transaksi finansial dan digunakan untuk:

- Eksplorasi data.
- Feature preprocessing.
- Pembentukan cluster.
- Penyusunan dataset siap klasifikasi.

File dataset yang tersedia di repository:

- data_clustering.csv
- data_clustering_inverse.csv

## Struktur Project

- [Clustering]_Submission_Akhir_BMLP_Your_Name.ipynb
	Notebook untuk tahap clustering, termasuk preprocessing, pemodelan cluster, dan evaluasi.

- [Klasifikasi]_Submission_Akhir_BMLP_Your_Name.ipynb
	Notebook untuk tahap klasifikasi menggunakan data hasil clustering.

- model_clustering.h5
	Model clustering yang telah disimpan.

- PCA_model_clustering.h5
	Artefak PCA untuk reduksi dimensi.

- decision_tree_model.h5
	Model klasifikasi Decision Tree.

- explore_random_forest_classification.h5
	Model Random Forest untuk eksplorasi performa.

- tuning_classification.h5
	Artefak model hasil proses tuning.

## Teknologi dan Library

Library utama yang digunakan di notebook:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- yellowbrick
- joblib

## Cara Menjalankan

1. Clone repository ini.
2. Pastikan Python 3.10+ sudah terpasang.
3. Install dependency yang dibutuhkan notebook.
4. Jalankan notebook clustering terlebih dahulu.
5. Jalankan notebook klasifikasi setelah dataset hasil clustering siap.

Contoh instalasi dependency:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick joblib jupyter
```

Menjalankan Jupyter:

```bash
jupyter notebook
```

## Workflow Singkat

1. Data loading dan data understanding.
2. Data preprocessing dan encoding fitur kategorikal.
3. Scaling dan pembentukan cluster.
4. Evaluasi cluster (termasuk silhouette/elbow sesuai notebook).
5. Penyimpanan artefak clustering dan PCA.
6. Split data untuk klasifikasi.
7. Training Decision Tree dan model alternatif.
8. Evaluasi metrik klasifikasi dan tuning.
9. Simpan model final.

## Catatan

- Ekstensi file model menggunakan .h5, namun proses penyimpanan di notebook menggunakan joblib.
- Untuk reproduksibilitas, gunakan random_state yang sama seperti di notebook.


