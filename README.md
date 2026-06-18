# 🏊‍♂️ SwimPace

Aplikace určená pro plavce (závodníky) a trenéry, která zjednodušuje organizaci tréninků a závodů.

---

## 📌 O projektu

Tento projekt se zaměřuje na vytvoření přehledného systému, kde:

- Trenéři mohou plánovat tréninky a závody  
- Plavci se mohou jednoduše zapisovat  
- Každý uživatel má svou roli a odpovídající funkce
- Součástí bude docházka
- Bude viditelná statistika plavců (výsledky, body FINA)


Cílem je usnadnit komunikaci a organizaci v plaveckém klubu a vytvořit funkční aplikaci.

---

## 📂 Struktura projektu

```text
SwimPace/
├── add_disciplines.py
├── check_registrations.py
├── create_future_zavod.py
├── create_trener.py
├── db.sqlite3
├── manage.py
├── plavecke_zavody/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── register_petr.py
├── requirements.txt
└── zavody/
  ├── __init__.py
  ├── admin.py
  ├── apps.py
  ├── models.py
  ├── tests.py
  ├── views.py
  ├── migrations/
  │   ├── 0001_initial.py
  │   ├── 0002_userprofile.py
  │   ├── 0003_vysledek_cas.py
  │   └── __init__.py
  └── templates/
    ├── base.html
    └── zavody/
      ├── add_plavec_to_klub.html
      ├── add_sverenek.html
      ├── home.html
      ├── klub_detail.html
      ├── kluby_list.html
      ├── login.html
      ├── plavci_list.html
      ├── plavec_detail.html
      ├── profile.html
      ├── register.html
      ├── stat_detail.html
      ├── stat_list.html
      ├── trener_detail.html
      ├── treneri_list.html
      ├── zapsat_plavce_na_zavod.html
      ├── zavod_detail.html
      └── zavody_list.html
```

---

## 🧩 Datový model

<!-- Sem později doplníš popis datového modelu. -->

## 🤖 Technologie
- Django
- Docker
- SQL

## 🎯 Moje cíle

- ✅ Vytvořit systém rozdílných uživatelských účtů:
  - 🏊‍♂️ Plavci (závodníci)
  - 🧑‍🏫 Trenéři

- ✅ Umožnit trenérům:
  - vytvářet tréninky
  - přidávat závody(Bude to fungovat podobně jako události na FB)
  - přiřazovat pod sebe své svěřence
  - zapisovat plavce(své svěřence) na závody 

- ✅ Umožnit plavcům:
  - zapisovat se na tréninky
  - přístup ke své docházce a statistice
 

  ❗❗❗Každý klub (trenér + svěřenci) má svůj dashboard, podle toho jaké události(závody/tréninky) vloží.

---

## 🏋️‍♂️ Tréninky

Trenéři budou moci vytvořit trénink, který bude obsahovat:

- 📍 místo (např. bazén)
- 📝 popis tréninku
- 🏊‍♂️ plán (co se bude plavat, série, vzdálenosti apod.)
- 📅 datum a čas

Plavci se následně budou moci na trénink přihlásit.

---

## 🏆 Závody

Trenéři budou moci přidávat závody s informacemi:

- 📍 místo konání
- 📅 datum
- 📝 detaily závodu
- 🏊 disciplíny

Plavci se budou moci na závody zapisovat.

---

## 👥 Uživatelské role

### 🏊‍♂️ Plavec (závodník)
- přihlášení do systému  
- zapisování na tréninky  
- zapisování na závody  

### 🧑‍🏫 Trenér
- vytváření tréninků  
- správa tréninků  
- přidávání závodů  
- správa závodů  

---

## 🎓 Závěrečný školní projekt

Tato aplikace je vytvářena jako závěrečný školní projekt.

---



## 🚀 Budoucí rozšíření (možnosti)

- notifikace  
- chat mezi trenérem a plavcem

## V momentalním stavu se zatím jedná pouze o prototyp ❗❗❗
