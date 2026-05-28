# Sıfırdan Sayısal Yöntemler

İlk ilkelerden inşa edilmiş, araştırma kalitesinde **6 haftalık** bir klasik **Sayısal Analiz** dersi. SciPy yok, hazır çözücü yok — yalnızca **saf NumPy ve Matplotlib**. Her algoritma uygulanır, yakınsama mertebesi açısından analiz edilir ve başarısızlık türlerine karşı sınanır.

Bu ders, [`numerical_methods`](https://github.com/HAYDARKILIC/numerical_methods) reposunun Türkçe ikizidir. [`numerical_methods_for_ml`](https://github.com/HAYDARKILIC/numerical_methods_for_ml) reposu makine öğrenmesinin sayısal yığınını (otomatik türev, SVD, BFGS, GP) yeniden inşa ederken, bu repo **temel sütunları** kapsar: kayan nokta gerçekliği, kök bulma, lineer sistemler, interpolasyon, kuadratür ve diferansiyel denklemler.

Her hafta tek başına yeterli bir Jupyter notebook'tur; **teorik türetmeleri**, **sıfırdan uygulamaları**, **görselleştirmeleri** ve **araştırma tarzı alıştırmaları** birleştirir.

---

## Felsefe

> *Cebirsel olarak eşdeğer ifadeler sayısal olarak eşdeğer değildir.*

Dersin birleştirici ipliği, bir **problemin koşullanması** ile bir **algoritmanın kararlılığı** arasındaki ayrımdır; bunlar sayısal analizin temel kuralıyla birbirine bağlanır:

```
ileri hata  ≲  koşul sayısı  ×  geri hata
```

Her yöntem bu mercekten değerlendirilir — 1. haftadaki ikinci derece denklem formülünden 6. haftadaki katı ADD çözücülerine kadar.

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

Capstone, sayısal yöntemleri **tek ve tutarlı bir disiplin** olarak göstermek için önceki beş haftanın tüm makinesini bilinçli olarak yeniden kullanır — örtük adımların içindeki kök bulma, sınır-değer problemleri için lineer çözücüler, zaman-adımlamanın arkasındaki kuadratür.

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
