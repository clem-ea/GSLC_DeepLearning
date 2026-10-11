# Tugas Take-Home Sesi 05: Transfer Learning & Advanced CNNs

**Nama:** Clement Ernest Atmadja  
**NIM:** 2802420643  
**Kelas:** LD01 - Computer Science BINUS University  
**Mata Kuliah:** Advanced CNNs and Transfer Learning (Sesi 05)


## Ringkasan Eksperimen
Proyek ini mengkaji performa *Transfer Learning* dan *Progressive Fine-Tuning* menggunakan **ResNet-18** dan **EfficientNet-B0** pada subset 10 kelas dari dataset **Oxford-IIIT Pet** (~2.000 citra). Eksperimen mencakup perbandingan model *From Scratch*, *Feature Extraction*, *Progressive Fine-Tuning*, kontrol tanpa augmentasi data, hingga arsitektur modern EfficientNet.

## Ringkasan Hasil Eksperimen (Tabel C1)

| Kode | Strategi Eksperimen | Trainable Params | Epoch | Durasi (s) | Akurasi Val | Test Macro F1 |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: |
| **B1** | Baseline (From Scratch) | 11,181,642 | 10 | 81.0s | 0.2282 | 0.2385 |
| **B2** | Feature Extraction | 5,130 | 20 | 150.3s | 0.9262 | 0.8960 |
| **B3** | Progressive Fine-Tuning | 8,398,858 | 13 | 97.1s | 0.9262 | **0.9124** |
| **B4** | Control (No Augmentation) | 8,398,858 | 20 | 91.6s | 0.9597 | 0.8909 |
| **B5** | EfficientNet-B0 | 424,970 | 20 | 151.5s | 0.9664 | **0.9139** |
