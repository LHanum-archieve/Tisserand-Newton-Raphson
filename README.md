# Plotter Parameter Tisserand (Metode Newton-Raphson)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)]()
![Status](https://img.shields.io/badge/Status-Active-success)

Program sederhana untuk menghitung dan memvisualisasikan Parameter Tisserand terhadap beberapa planet (Merkurius hingga Saturnus). Kode ini menggunakan metode Newton–Raphson untuk menyelesaikan persamaan karakteristik dan menghasilkan kurva hubungan:

- Semi-major axis (a)
- Eksentrisitas (e)
- Parameter Tisserand (Tₚ)

## Teori Singkat:
Parameter Tisserand relatif terhadap suatu planet dengan sumbu semi-mayor aₚ) dirumuskan sebagai:

```math
T_p = \frac{a_p}{a} + 2\cos{i}\sqrt{\frac{a}{a_p}(1 - e^2)}
```
dengan:
- a   : sumbu semi-mayor benda kecil
- aₚ  : sumbu semi-mayor planet
- e   : eksentrisitas orbit
- i   : inklinasi

## Fitur
- Menghitung nilai akar menggunakan metode Newton–Raphson
- Plot per planet dan plot gabungan 
- Nilai parameter dapat dimodifikasi (Tₚ, inklinasi, rentang eksentrisitas)

## Struktur Folder
```bash
tisserand-parameter/
├── src/
│   └── tisserand_plotter.py
├── README.md
└── requirements.txt
```

## Cara Menjalankan

1. Clone repository berikut:  
   ```bash
   git clone https://github.com/LHanum-archieve/tisserand-parameter.git
   cd tisserand-parameter
2. Install dependensi:
   ```bash
   pip install -r requirements.txt
3. Jalankan script:
   ```bash
   python src/tisserand_plotter.py
