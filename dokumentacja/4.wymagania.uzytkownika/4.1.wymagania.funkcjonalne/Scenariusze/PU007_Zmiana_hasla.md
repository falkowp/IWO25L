# **PU007: Zmiana hasła**

#### Autor: Marcin Komza

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Użytkownik jest zalogowany do systemu.

1. Użytkownik wybiera opcję „Zmień hasło”.
2. System wyświetla formularz zmiany hasła.
3. Użytkownik wprowadza dane formularza zmiany hasła.
4. System sprawdza dane formularza zmiany hasła.\
   [ DANE POPRAWNE ]
5. System zmienia hasło w bazie danych.
6. System wyświetla komunikat poprawnej zmiany hasła.

**POST:** Konto użytkownika w bazie danych posiada zmienione hasło.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Niepoprawne obecne hasło

1.-4. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
&nbsp;&nbsp;&nbsp;&nbsp;[ DANE NIEPOPRAWNE ]\
5. a. System wyświetla komunikat o niepoprawnym obecnym haśle.

**POST:** Konto użytkownika w bazie danych nie ulega zmianie.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Nowe hasło oraz potwórz nowe hasło nie są takie same

1.-4. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
&nbsp;&nbsp;&nbsp;&nbsp;[ DANE NIEPOPRAWNE ]\
5. b. System wyświetla komunikat o niepoprawnym nowym haśle.

**POST:** Konto użytkownika w bazie danych nie ulega zmianie.

## 3. SŁOWNIK POJĘĆ

### Formularz zmiany hasła
- **Atrybuty**:  
  - Obecne hasło: tekst  
  - Nowe hasło: tekst
  - Powtórz nowe hasło: tekst

### Hasło

* **Definicja**: ciąg znaków wymagany do uwierzytelnienia użytkownika

### Konto użytkownika
* **Definicja**: Profil użytkownika w systemie
- **Atrybuty**:  
  - id: liczba  
  - nazwa: tekst
  - hasło: tekst

  
