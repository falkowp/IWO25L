# PU010: Wylogowanie użytkownika

#### Autor: Marcin Komza

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU010

PRE: Użytkownik jest zalogowany i posiada aktywną sesję.

1. Użytkownik wybiera opcję "Wyloguj się".
2. System wyświetla komunikat zamiaru wylogowania.
3. Użytkownik wybiera opcję "Tak".
4. System usuwa sesję użytkownika.
5. System wyświetla ekran wylogowania.

FINAL: Success\
POST: Sesja użytkownika nie znajduje się w bazie danych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Użytkownik nie chce się wylogować

1.-2. tak samo jak w "SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU010".\
3. a. Użytkownik wybiera opcję "Nie".\
4. a. System zamyka komunikat zamiaru wylogowania.

FINAL: Failure\
POST: Sesja użytkownika dalej znajduje się w bazie danych.

## 3. SŁOWNIK POJĘĆ

### Sesja  
- **Definicja**: Obiekt zawierający informację o tym czy użytkownik jest zalogowany  
- **Atrybuty**: 
  - ID: liczba
  - ID Użytkownika: liczba
  - Data wygaśnięcia: data

### Komunikat zamiaru wylogowania
- **Definicja**: Komunikat pytający użytkownika, czy na pewno chce się wylogować. 
- **Metody**: 
  - Tak()
  - Nie()
