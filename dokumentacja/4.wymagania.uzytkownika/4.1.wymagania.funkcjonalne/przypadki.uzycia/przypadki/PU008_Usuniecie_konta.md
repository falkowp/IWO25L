# **PU008: Usunięcie konta**
#### Autor: Mikołaj Pątkowski

## 1. SCENARIUSZ GŁÓWNY 
**PRE:** Administrator jest zalogowany i ma uprawnienia do usunięcia konta użytkownika.

1. Administrator wybiera konto użytkownika z listy użytkowników.
2. Administrator wybiera opcję "Usuń".
3. System wyświetla okno potwierdzenia operacji usunięcia konta.
   
   \[ WYBÓR "TAK" ]
   
4. Administrator wybiera opcję "tak".
5. System zamyka okno potwierdzenia operacji usunięcia konta.
6. System usuwa konto użytkownika z bazy danych.
   
   \[ UŻYTKOWNIK USUNIĘTY PRAWIDŁOWO ]
7. System wyświetla okno potwierdzenia wykonania operacji usunięcia konta.
8. Administrator wybiera opcję "ok".
9. System odświeża listę użytkowników.

**FINAL:** Success

**POST:** Konto użytkownika nie znajduje się w bazie danych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Anulowanie operacji
1-3. Tak samo, jak w SCENARIUSZU GŁÓWNYM

   \[ WYBÓR "NIE" ]
   
4. a. System zamyka okno potwierdzenia operacji usunięcia konta.
   
**FINAL:** Failure

**POST:** Konto użytkownika znajduje się w bazie danych.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Błąd usuwania konta
1-6. Tak samo, jak w SCENARIUSZU GŁÓWNYM

   \[ UŻYTKOWNIK NIE USUNIĘTY PRAWIDŁOWO ]
   
7. a. System wyświetla komunikat błędu usunięcia konta.
8. a. Administrator wybiera opcję "ok".
9. a. System zamyka komunikat błędu usunięcia konta.

**FINAL:** Failure

**POST:** Konto użytkownika znajduje się w bazie danych.

## 3. SŁOWNIK POJĘĆ

### Konto użytkownika
* **Definicja**: Profil użytkownika w systemie
- **Atrybuty**:  
  - id: liczba  
  - nazwa: tekst
  - hasło: tekst

### Lista użytkowników
* **Definicja**: Zbiór kont użytkowników dostępnych w systemie.
- **Atrybuty**:  
  - długość: liczba
  - konta: Konto użytkownika[Lista]
