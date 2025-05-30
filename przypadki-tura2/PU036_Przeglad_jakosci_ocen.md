# PU0036: Przegląd jakości ocen

#### Autor: Maciej Przybylski

## 1. SCENARIUSZ GŁÓWNY

**PRE:** Użytkownik jest zalogowany do systemu i ma odpowiednie uprawnienia.

1. Użytkownik wybiera z listy pozycję
2. System wyświetla okno z informacjami o metadanych
3. Użytkownik wybiera zakładkę "Ocena"
4. System wyświetla ocenę jakości metadanych

**POST:** Użytkownikowi zostaje wyświetlona ocena metadanych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - System traci połączenie z internetem

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
   \[ SYSTEM TRACI POŁĄCZENIE Z INTERNETEM ]
2. a. System wyświetla komunikat o braku połączenia z internetem

**POST:** Użytkownik zostaje poinformowany o braku połączenia z internetem.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - System nie posiada danych o ocenie

1. -3. Tak samo, jak w SCENARIUSZU GŁÓWNYM
   \[ SYSTEM NIE POSIADA DANYCH O OCENIE ]


4. b System wyświetla komunikat o braku danych o ocenie

**POST:** Użytkownik zostaje poinformowany o braku ocen w bazie.

## 3. SŁOWNIK POJĘĆ

### Metadane

* **Definicja**: informacje o danym źródle danych

- **Atrybuty**:
    - ID: numer
    - Nazwa: tekst
    - Opis: tekst
    - Właściciel: tekst
    - Data utworzenia: data
    - Data modyfikacji: data

### Ocena źródła danych

* **Definicja**: informacje o jakości i wiarygodności danego źródła danych

- **Atrybuty**:
    - ID: numer
    - Metadana ID: numer
    - Ocena: liczba
    - Komentarz: tekst
