# **PU0021: Edycja metadanych**

#### Autor: Jakub Wypych

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Użytkownik jest zalogowany do systemu, posiada uprawnienia administratora i znajduje się na oknie szczegół metadanych.

1. Administrator wybiera opcję „Edytuj metadane”.
2. System wyświetla okno edycji metadanych.
3. Administrator zmienia wartości metadanych.
4. Administrator wciska przycisk "zatwierdź".
5. System weryfikuje wprowadzone dane.\
[DANE POPRAWNE ]
6. System wprowadza zmiany do bazy danych.\
[ZMIANA SUKCESYWNA]
7. System wyświetla okno sukcesu edycji metadanych.

**FINAL:** SUCCESS.\
**POST:** W bazie danych została wprowadzona poprawna zmiana dla edytowaych metadanych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Niepoprawne wprowadzone nowe wartości

1.-5. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
[DANE NIEPOPRAWNE ]\
6. a. System wyświetla komunikat o błednych wprowadzonych wartościach.\
7. a. Administrator wybiera opcję "OK".\
8. a. Powrót do 2. z SCENARIUSZU GŁÓWNYM

**FINAL:** FAILURE.\
**POST:** W bazie danych niezostała wprowadzona żadna zmiana dla edytowaych metadanych.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Brak sukcesu w wprowdzeniu zmiany do bazy danych

1.-6. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
[ZMIANA NIESUKCESYWNA]\
7. b. System wyświetla komunikat o błędzie podczas próby wprowdzenia zmiany do bazy danych.\
8. b. Administrator wybiera opcję "OK".\
9. b. Powrót do 2. z SCENARIUSZU GŁÓWNYM

**FINAL:** FAILURE.\
**POST:** Administrator nie zapoznał się ze zgłoszeniem.

### 2.3. SCENARIUSZ ALTERNATYWNY 3 – Anulowanie edycji

1.-2. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
3. c. Administrator wciska przycisk anuluj.\
4. c. System powraca do okna szczegół metadanych.

**FINAL:** FAILURE.\
**POST:** W bazie danych niezostała wprowadzona żadna zmiana dla edytowaych metadanych.

## 3. SŁOWNIK POJĘĆ

### Okno edycji metadanych

* **Definicja**: formularz który zawiera wszystkie zmienne metadanych które można edytować. Dodatkowo zawiera przycik "zatwierdź" i "anuluj"

- **Atrybuty**:  
  - Metadane : metadane