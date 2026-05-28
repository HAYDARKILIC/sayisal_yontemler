# Sayısal Yöntemler

Bu depo, klasik sayısal analiz konularını sıfırdan öğreten 6 haftalık bir ders niteliğindedir. Buradaki temel felsefe şudur: bir yöntemi gerçekten anlamanın tek yolu, onu kendi elinizle inşa etmektir. Bu yüzden hiçbir hazır çözücü kütüphanesi (örneğin SciPy) kullanılmaz; her algoritma yalnızca NumPy ve Matplotlib ile, en temel yapı taşlarından başlanarak kodlanır.
Ders, her biri tek başına yeterli olan altı Jupyter notebook'tan oluşur. Her notebook üç katmanı bir arada sunar: konunun matematiksel temeli (türetmeler ve teoremler), bu teorinin çalışan koda dönüştürülmüş hâli ve sonuçları sezgisel kılan görselleştirmeler. Her haftanın sonunda, okuyucuyu konuyu kendi başına derinleştirmeye iten araştırma tarzı alıştırmalar yer alır.

---

## Müfredat

| Hafta | Konu | Sıfırdan inşa edilen yöntemler |
|:---:|---|---|
| **1** | Kayan Nokta ve Hata Analizi | Makine epsilonu, felaket sadeleşmesi, koşullanma, geri hata |
| **2** | Kök Bulma | İkiye bölme, sabit nokta, Newton, sekant, güvenli hibrit; yakınsama mertebesi kestirimi |
| **3** | Lineer Sistemler | Pivotlu LU, Cholesky, koşul sayıları, iteratif iyileştirme |
| **4** | İnterpolasyon ve Yaklaşıklama | Lagrange/Newton biçimleri, Runge olgusu, Chebyshev düğümleri, kübik spline'lar, en küçük kareler |
| **5** | Türev ve İntegral | Sonlu farklar, Richardson ekstrapolasyonu, Newton–Cotes, uyarlamalı ve Gauss kuadratürü |
| **6** | ADD'ler ve Sonlu Farklar *(capstone)* | Euler, RK4, uyarlamalı RK, katılık ve örtük yöntemler, sınır-değer problemleri |

---

## Repo yapısı

```
sayisal_yontemler/
├── notebooks/
│   ├── hafta1_kayan_nokta_ve_hata_analizi.ipynb
│   ├── hafta2_kok_bulma.ipynb
│   ├── hafta3_lineer_sistemler.ipynb
│   ├── hafta4_interpolasyon_yaklasiklama.ipynb
│   ├── hafta5_turev_integral.ipynb
│   └── hafta6_adiler_ve_sonlu_farklar.ipynb
├── requirements.txt
├── LICENSE
└── README.md
```

---

## Başlangıç

```bash
git clone https://github.com/HAYDARKILIC/sayisal_yontemler.git
cd sayisal_yontemler
pip install -r requirements.txt
jupyter notebook notebooks/
```

Tek bağımlılıklar **NumPy**, **Matplotlib** ve **Jupyter**'dir. Her notebook dış veri olmadan baştan sona çalışır.

---

## Ön koşullar

- Kalkülüs (Taylor serileri, türevler, integraller)
- Lineer cebir (matrisler, özdeğerler — bkz. [`linear_algebra_for_ml`](https://github.com/HAYDARKILIC/linear_algebra_for_ml))
- Rahat Python + NumPy

---

## Lisans

MIT Lisansı ile yayımlanmıştır — bkz. [`LICENSE`](LICENSE).
