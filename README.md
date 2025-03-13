# Erken Evre Akciğer Kanseri Nüks Tahmini Projesi

Bu proje, erken evre akciğer kanseri (Evre I-II) hastalarında hastalık nüksünü tahmin etmek için oluşturulmuş makine öğrenmesi modellerini içermektedir.

Model, klinik ve patolojik parametreler kullanılarak hastaların nüks riskini skorlamayı amaçlamaktadır.

## Kullanılan Teknolojiler
- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow
- Keras

## Veri Seti

- Veri seti toplam 104 hastaya ait klinik ve patolojik bilgiler içermektedir.
- Özellikler:
  - Yas
  - Hucre tipi
  - DLCO%
  - FEV1/FVC%
  - Ekstranodal tutulum (Ext)
  - Major komplikasyon
  - Vaskuler invazyon
  - Nekroz
  - STAS
  - T, N, M evresi
  - Nuks (hedef degisken)

Veri setine buradan ulasabilirsiniz:
akciger_kanseri_veri_seti.csv (data/akciger_kanseri_veri_seti.csv)

## Modellere Genel Bakis

- Gradient Boosting Classifier
- Decision Tree Classifier
- Yapay Sinir Agi (Keras Sequential)

## Kullanım Ornegi

1. Depoyu kopyalayin:
   git clone <repo-linki>

2. Proje klasorune girin:
   cd proje-klasoru

3. Gerekli kutuphaneleri yukleyin:
   pip install -r requirements.txt

4. Modeli calistirin:
   python model.py

## Model Performanslari

- Gradient Boosting Classifier dogruluk orani: %XX
- Decision Tree dogruluk orani: %XX
- Yapay Sinir Agi (Keras) dogruluk orani: %XX

(Oranlar ornek verilmistir, kendi verinize gore guncelleyebilirsiniz.)

## Klasor Yapisi

.
├── data
│   └── akciger_kanseri_veri_seti.csv
├── models
│   └── lung_cancer_recurrence_model.h5
├── scripts
│   └── model.py
├── README.md
├── requirements.txt
└── .gitignore

1. data: Veri seti dosyalarini barindirir.
2. models: Egitilmis modellerin kaydedildigi klasor.
3. scripts: Kodlarin (veri isleme, model egitimi vb.) bulundugu klasor.
4. README.md: Proje hakkinda aciklamalar.
5. requirements.txt: Python paketleri ve surumleri.

# Bu projenin gerçek veri seti hasta gizliliği açısından paylaşılmamıştır. Benchmark sonuçları paylaşılacaktır.
