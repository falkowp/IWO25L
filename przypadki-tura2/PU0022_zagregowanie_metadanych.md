# **PU0022: Zagregowanie metadanych**

#### **Autor:** Artem Omelchenko

#### **Opis:** Możliwość scalania i analizy metadanych z różnych źródeł.

---

## **1. SCENARIUSZ GŁÓWNY PU0022**

**PRE:**
Użytkownik jest zalogowany do systemu.
Użytkownik znajduje się w module przeglądu metadanych.
Lista metadanych została wcześniej załadowana.

1. Użytkownik zaznacza metadane do scalenia z dostępnej listy.
2. Użytkownik klika przycisk **„Scal metadane”**.
3. System scala wybrane metadane.
   \[SCALONE]
4. System wyświetla komunikat: **„Metadane zostały scalone”** oraz przyciski **„Analizuj metadane”** i **„Pobierz metadane”**.
5. Użytkownik klika przycisk **„Analizuj metadane”**.
6. System rozpoczyna analizę i wyświetla komunikat: **„Trwa analiza metadanych…”**.
   \[DANE PRZEANALIZOWANE]
7. System wyświetla wyniki analizy w osobnym oknie.

**POST:**
Metadane są scalone oraz przeanalizowane. Wynik analizy dostępny do pobrania.

---

## **2. PRZEBIEGI ALTERNATYWNE**

### **2.1. SCENARIUSZ ALTERNATYWNY PU0022-2 – Błąd scalania**

1–3. Tak samo jak w SCENARIUSZU GŁÓWNYM.
\[NIE SCALONE]
4B. System wyświetla komunikat: **„Nie można scalić wybranych metadanych.”**
5B. System wyświetla przycisk **„Powrót”** i przekierowuje użytkownika do listy metadanych.

**POST:**
Metadane nie zostały scalone. Operacja została anulowana.

---

### **2.2. SCENARIUSZ ALTERNATYWNY PU0022-3 – Błąd analizy, ale możliwe pobranie**

1–5. Tak samo jak w SCENARIUSZU GŁÓWNYM.
\[NIE UDAŁO SIĘ PRZEANALIZOWAĆ]
6C. System wyświetla komunikat: **„Błąd analizy – nie udało się przeanalizować scalonych danych.”**
7C. System wyświetla przycisk **„Pobierz metadane mimo błędu analizy”**.
8C. Użytkownik klika przycisk **„Pobierz metadane mimo błędu analizy”**.

**POST:**
Metadane zostały scalone, ale nie przeanalizowane. Użytkownik je pobrał.

---

### **2.3. SCENARIUSZ ALTERNATYWNY PU0022-4 – Pobranie po scaleniu**

1–4. Tak samo jak w SCENARIUSZU GŁÓWNYM.
5D. Użytkownik klika przycisk **„Pobierz metadane”**.

**POST:**
Metadane zostały scalone i pobrane. Analiza nie została przeprowadzona.

---


## **3. SŁOWNIK POJĘĆ**

### **Lista metadanych**

**Definicja:** Zbiór danych zawierający pewną liczbę wybranych metadanych.

* **Atrybuty:**

  * **Nazwa:** tekst
  * **Opis:** tekst
  * **Data utworzenia:** data
  * **Zawartość:** metadane \[Lista]

---

### **Metadane**

**Definicja:** Dane na temat źródła danych.

* **Atrybuty:**

  * **id:** int
  * **idŹródła:** int
  * **dataUtworzenia:** data
  * **dataAktualizacji:** data
  * **osobaKontaktowa:** string
  * **emailKontaktowy:** string
  * **licencja:** string
