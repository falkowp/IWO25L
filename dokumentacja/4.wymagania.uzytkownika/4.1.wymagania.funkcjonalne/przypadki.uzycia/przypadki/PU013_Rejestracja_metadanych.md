# PU013: Rejestracja metadanych

#### Autor: Jan Gębal

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU013

PRE: Administrator jest zalogowany oraz ma uprawnienia do rejestracji metadanych.

1. Administrator wybiera opcję "Zarejestruj metadane".  
2. System wyświetla formularz rejestracji metadanych.  
<< invoke >> Dodanie nowego zestawu metadanych
3. Administrator wprowadza nazwę, opis, tagi i właściciela metadanych.
4. System waliduje wprowadzone dane.
[ DANE POPRAWNE ]
5. System rejestruje metadane.
6. System wyświetla komunikat o pomyślnej rejestracji metadanych.

FINAL: Success 
POST: Nowe metadane znajdują się w bazie danych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Wprowadzono niepoprawne dane w formularzu rejestracji     

1. -4. Tak samo, jak w SCENARIUSZU GŁÓWNYM.
[ DANE NIEPOPRAWNE ]
5. a. System wyświetla komunikat o niepoprawnych danych.
6. a. Powrót do punktu 2 w SCENARIUSZU GŁÓWNYM.

FINAL: Failiure
POST: Nowe metadane nie znajdują się w bazie danych.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Rejestracja została anulowana

1. -2. Tak samo, jak w SCENARIUSZU GŁÓWNYM.
3. b. Administrator wybiera opcję "Anuluj".
4. b. System zamyka formularz rejestracji metadanych. 

FINAL: Failiure
POST: Nowe metadane nie znajdują się w bazie danych.

## 3. SŁOWNIK POJĘĆ

### Metadane  
- **Definicja**: Dane na temat źródła danych.  
- **Atrybuty**: 
  - ID: liczba
  - Nazwa: tekst
  - Opis: tekst
  - Właściciel: tekst
  - Data utworzenia: data
  - Data aktualizacji: data
  - status: enum
  - czy_zarchiwizowane: bool