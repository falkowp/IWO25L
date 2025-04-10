# PU033: Wyświetlenie informacji o zgłoszeniu

#### Autor: Patrycja Falkowska

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU033

PRE: Adminsitrator jest zalogowany do systemu i znajduje się w widoku listy zgłoszeń.

1. Administrator naciska przycisk „Wyświetl szczegóły” przy wybranym zgłoszeniu.  
[ DANE POPRAWNE ]
2. System wyświetla atrybuty zgłoszenia.  
3. Administrator zapoznaje się z atrybutami zgłoszenia.

POST: Administrator zapoznał się z atrybutami zgłoszenia i moze wykonać dalsze działania administracyjne.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Zgłoszenie zostało usunięte  

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
[ DANE NIEPOPRAWNE ]
2a. System wykrywa brak zgłoszenia.
3a. System wyświetla komunikat o usunięciu zgłoszenia.
4a. Administrator wybiera opcję "OK".
5a. System zamyka atrybuty zgłoszenia.

FINAL: Failiure
POST: Administrator nie zapoznał się z atrybutami zgłoszenia.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Zgłoszenie zostało przeniesione do archiwum  

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
[ DANE NIEPOPRAWNE ]
2b. System wykrywa przeniesienie zgłoszenia do archiwum.
3b. System wyświetla komunikat o przeniesieniu zgłoszenia do archiwum.
4b. Administrator wybiera opcję "OK".
5b. System zamyka atrybuty zgłoszenia.

FINAL: Failiure
POST: Administrator nie zapoznał się z atrybutami zgłoszenia.

## 3. SŁOWNIK POJĘĆ

### Zgłoszenie  
- **Definicja**: Wpis zawierający informacje o problemie, potrzebie lub incydencie zgłoszonym przez użytkownika.  
- **Atrybuty**: 
  - ID: liczba
  - Autor: tekst
  - Treść zgłoszenia: tekst
  - Data zgłoszenia: data

### Archiwum zgłoszeń 
- **Definicja**: Miejsce do przechowywania nieaktualnych/rozwiązanych zgłoszeń. 
- **Atrybuty**: 
  - Zgłoszenia: lista zgłoszeń

### Lista zgłoszeń 
- **Definicja**: Lista zawierająca aktualne zgłoszenia o błędach/problemach od użytkowników.
- **Atrybuty**: 
  - Zgłoszenia: lista zgłoszeń
