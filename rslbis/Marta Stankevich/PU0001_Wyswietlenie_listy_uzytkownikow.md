# PU0001: Wyświetlenie listy użytkowników

#### Autor: Patrycja Falkowska
##### Część merytoryczna: Adrian Rybaczuk

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU0001

PRE: Użytkownik jest zalogowany do systemu i posiada rolę „Administratora”.

1. Administrator wybiera opcję „Lista użytkowników”.  
[ DANE POPRAWNE ]  
2. System wyświetla okno „Lista użytkowników”.

POST: Wyświetlono listę użytkowników.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Brak użytkowników

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM  
[ DANE NIEPOPRAWNE ]  
2. a. System wyświetla okno z komunikatem: „Brak użytkowników”.

FINAL: Success  
POST: Wyświetlono pustą listę użytkowników.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Błąd połączenia z bazą danych

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM  
[ DANE NIEPOPRAWNE ]  
2. b. System wyświetla komunikat: „Błąd połączenia z bazą danych”.

FINAL: Failure  
POST: Wyświetlono komunikat o braku możliwości pobrania danych.

## 3. SŁOWNIK POJĘĆ

### Lista użytkowników  
- **Definicja**: Lista zawierająca informacje o użytkownikach systemu.

### Okno listy użytkowników  
- **Definicja**: Okno wyświetlające dane z „listy użytkowników”.  

### Użytkownik  
- **Definicja**: Osoba korzystająca z systemu.  
- **Atrybuty**:  
  - ID: numer  
  - Imię: tekst  
  - Nazwa: string  
  - Hasło: string  
  - Uprawnienia: enum  
  - Role: enum
