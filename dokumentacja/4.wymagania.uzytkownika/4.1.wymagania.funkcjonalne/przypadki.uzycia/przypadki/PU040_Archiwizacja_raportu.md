# **PU040: Archiwizacja raportu**

#### Autor: Jan Gębal

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Administrator jest zalogowany do systemu oraz ma uprawnienia do archiwizacji raportu

1. Administrator wybiera opcję „Zarchiwizuj”.
2. System wyświetla okno potwierdzenia akcji.
3. Administrator wybiera opcję "Potwierdź".
4. System zapisuje raport w bazie danych.
5. System wyświetla komunikat o poprawnej archiwizacji.
6. Administrator wybiera opcję „Ok”.
7. System przekierowuje do listy raportów.

**FINAL:** Success

**POST:** Raport został zapisany jako archiwalny w bazie danych

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Anulowanie akcji

1.-2. Tak samo, jak w SCENARIUSZU GŁÓWNYM.  
3. a. Administrator wybiera opcję "Anuluj".\
4. a. System zamyka okno potwierzenia akcji.

**FINAL:** Failure

**POST:** Raport nie został zapisany jako archiwalny w bazie danych

## 3. SŁOWNIK POJĘĆ

### Raport

* **Definicja**: Zorganizowany zestaw danych, wygenerowany na podstawie zgromadzonych informacji w systemie.

- **Atrybuty**:  
  - ID: numer  
  - Typ: enum
  - AdresUrl: tekst
  - DataArchwizacji: data

