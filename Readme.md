 Students Performance Prediction Project
Dataset: StudentsPerformance.csv Domena: Performance studenata, opis: Dataset sadrži Stepen obrazovanja studenata, kurseve za pripremu za ispit. Predikcija uspjeha na ispitu iz matematike. Cilj: Predikcija usphjeha studenata.

Ovaj projekat koristi dataset StudentsPerformance.csv za analizu i predikciju uspjeha studenata.

📁 Struktura projekta
zavrsni_projekat/
├── data/                          # Ulazni CSV fajlovi
├── etl/                           # ETL moduli (Extract, Transform, Load)
│   ├── extract/
│   │   └── extractor.py
│   ├── transform/
│   │   └── transformer.py
│   └── load/
│       └── loader.py
├── analysis/                      # Analiza podataka
│   ├── eda.ipynb                  # Exploratory Data Analysis u Jupyteru
|   |── eda_executed.ipynb         # Rezultati Data Analysis
|   |── upiti.py                   # SQL upiti u Pythonu
├── ml/                            # Machine Learning modul
│   ├── model.py                   # Trening i evaluacija modela
│   └── train_model.ipynb          # ML Notebook
├── requirements.txt               # Lista biblioteka
├── main.py                        # Glavna ETL skripta
└── README.md                      # Dokumentacija projekta
📌 Opis projekta
Cilj projekta je analizirati uspjeh studenata i na osnovu tih karakteristika predvidjeti njihov uspjeh korištenjem regresionih i klasifikacionih algoritama.

✅ Ključne faze projekta
ETL obrada podataka

Učitavanje iz CSV fajla
Čišćenje podataka i transformacija
Ubacivanje u SQLite bazu
SQL analiza

5 SQL upita nad bazom
Integracija upita u Python koristeći sqlite3 i pandas
EDA - Exploratory Data Analysis
Korelacija, boxplot, histogrami, scatter plot
Vizualizacije sa matplotlib i seaborn
Mašinsko učenje

split_data() za pripremu podataka
train_model() sa Pipeline + GridSearchCV
evaluate_model() za izvještaj tačnosti
explain_model_shap() za SHAP analizu (samo RandomForest)
plot_feature_importance() za feature importance (samo RandomForest)
Objektno-orijentisani kod

Trening modela sa GridSearchCV pipeline-om
Evaluacija modela na test skupu
SHAP analiza (samo za RandomForest)
Feature importance
▶️ Pokretanje projekta
Kloniraj repozitorij:
git clone https://github.com/Haris-Mujanovic/Zavrsni
cd Zavrsni
Instaliraj zavisnosti:
pip install -r requirements.txt
Pokreni Jupyter notebook:
🔧 Requirements
pandas
sqlalchemy
pyodbc
matplotlib
seaborn
scikit-learn
notebook
nbconvert
nbformat
scipy
os