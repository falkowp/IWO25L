# PU004: Rejestracja w systemie

#### Autor: Michał Janaszewski

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU004

PRE: Użytkownik nie jest zalogowany

1. Użytkownik wybiera opcję „Zarejestruj się”.
2. System wyświetla formularz rejestracji.
3. Użytkownik wypełnia formularz.  
4. System waliduje dane.  
5. \<<invoke\>> Wysłanie kodu rejestracyjnego .
6. System wyświetla formularz kodu rejestracyjnego.
7. Użytkownik wprowadza kod rejestracyjny.  
8. Użytkownik zatwierdza formularz z kodem.  
9. System waliduje kod rejestracyjny.  
10. \<<invoke\>> System zapisuje użytkownika w bazie danych.  
11. System wyświetla komunikat o pomyślnej rejestracji.

POST: Nowe konto użytkownika w bazie danych.

## 2. PRZEBIEGI ALTERNATYWNE  

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Anulowane rejesracji

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
2. a. Użytkownik wybiera opcje "Anuluj rejestrację".
   
FINAL: Failiure
POST: Użytkownik nie zalogowany.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Błąd walidacji danych rejesracji

1-4. Tak samo, jak w SCENARIUSZU GŁÓWNYM
5. \<<invoke\>> Anulowanie rejestracji

FINAL: Failiure
POST: Użytkownik nie zalogowany.

### 2.3. SCENARIUSZ ALTERNATYWNY 3 - Błąd walidacji kodu rejestracyjnego

1-9. Tak samo, jak w SCENARIUSZU GŁÓWNYM
10. c. \<<invoke\>> Anulowanie rejestracji

FINAL: Failiure
POST: Użytkownik nie zalogowany.

## 3. SŁOWNIK POJĘĆ

### Użytkownik  
- Osoba fizyczna lub podmiot, który korzysta z systemu i rejestruje się w celu uzyskania dostępu do jego funkcji.

### Formularz rejestracji
- Interfejs służący do wprowadzenia danych użytkownika,niezbędnych do założenia konta w systemie. Nawiera następujące **Atrybuty**:
  - Nazwa użytkownika : tekst
  - Imię : tekst
  - Nazwisko : tekst
  - Hasło : tekst
  - Powtórz hasło : tekst

### Formularz kodu rejestracjinego
- Interfejs służący do wprowadzenia kodu rejestracyjnego, zawiera  **Atrybut**:
  - Kod rejestracyjny : tekst