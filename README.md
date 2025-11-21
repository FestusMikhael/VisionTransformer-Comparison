#  VisionTransformer-Comparison: Perbandingan Model Transformer untuk Klasifikasi Gambar

Proyek ini merupakan Tugas Eksplorasi Mata Kuliah Pembelajaran Mendalam (**Deep Learning**) untuk membandingkan secara empiris kinerja dan efisiensi tiga arsitektur Vision Transformer terkemuka: ViT, DeiT, dan Swin Transformer, pada *dataset* CIFAR-10.

## Arsitektur Model yang Dibandingkan

1.  **Vision Transformer (ViT)**: Model Transformer murni.
2.  **DeiT (Data-efficient Image Transformer)**: Varian ViT yang menggunakan *Knowledge Distillation*.
3.  **Swin Transformer**: Model hierarkis yang menggunakan *Shifted Window Attention*.

## Cara Menjalankan Kode 

Kode ini dirancang untuk dijalankan di lingkungan dengan akselerasi GPU (NVIDIA CUDA). Eksperimen ini dilaksanakan menggunakan **NVIDIA Tesla T4 GPU** di **Google Colab**.

### A. Persyaratan Sistem

* Python 3.8+
* NVIDIA CUDA (Perangkat Keras: **NVIDIA Tesla T4**).

### B. Instalasi Dependensi

Instal semua *library* yang diperlukan menggunakan file **`requirements.txt`**:

```bash
pip install -r requirements.txt
```

## Eksekusi
1. Seluruh pipeline eksperimen (Data Loading, Preprocessing, Fine-tuning, dan Evaluation) terkandung dalam file Perbandingan_Model_Vision_Transformer.ipynb.
2. Buka Notebook: Buka Perbandingan_Model_Vision_Transformer.ipynb di Google Colab atau JupyterLab.
3. Jalankan Secara Berurutan: Jalankan semua sel dalam notebook secara berurutan. Kode akan otomatis mengunduh dataset CIFAR-10 dan memuat bobot pretrained ImageNet.
4. Output yang Dihasilkan: Notebook akan menghasilkan log pelatihan, kurva pembelajaran, Confusion Matrix, dan memperbarui file CSV prediksi.

## Konfigurasi 
1. Learning Rate = 1e-5
2. Epoch = 5
3. Batch Size = 32
4. Framework PyTorch
   
## Author
Festus Mikhael
