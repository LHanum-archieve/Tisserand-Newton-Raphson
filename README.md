# Plotter Parameter Tisserand (Metode Newton-Raphson)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)]()
![Status](https://img.shields.io/badge/Status-Active-success)

Ini adalah program sederhana untuk menghitung dan memvisualisasikan Parameter Tisserand untuk beberapa planet (Merkurius hingga Saturnus). Program ini menggunakan metode :
- Newton–Raphson,
- Secant,
- Bisection, dan
- Brent
  
untuk menyelesaikan persamaan terkait dan menghasilkan kurva hubungan antara :
- Semi-major axis (a)
- Eksentrisitas (e)
- Parameter Tisserand (Tₚ)

## Teori Singkat:
Parameter Tisserand relatif terhadap sebuah planet (dengan sumbu semi-mayor aₚ) didefinisikan sebagai:

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
│   └── tisserand-bisection.py
│   └── tisserand-brent.py
│   └── tisserand-newton-raphson.py
│   └── tisserand-secant.py
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
   python src/tisserand-newton-raphson.py
