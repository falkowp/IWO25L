# **PU006: Nadanie hasła**

#### Autor: Wojciech Grot

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Administrator jest zalogowany na swoje konto,
           Na ekranie wyświetlona jest lista użytkowników

1. Administrator wybiera przycisk "opcje użytkownika", obok użytkownika któremu hasło chce nadać.
2. System wyświetla menu kontekstowe dla wybranego użytkownika.
3. Administrator wybiera opcję "nadaj hasło".
4. System wyświetla formularz nadania hasła.
5. Administrator wpisuje nowe hasło w przeznaczone do tego pole w formularzu.
6. Administrator klika przycisk "zapisz zmiany"
   \[ DANE ZAPISANE POPRAWNIE]
7. System zapisuje zmiany w bazie danych.
8. System wysyła maila do użytkownika z informacją o nadaniu hasła
9. System wyświetla komunikat o sukcesie nadania hasła
10. Adm,inistrator klika przycisk "OK"
11. System wyświetla ponownie listę użytkowników

**POST:** Wybrany użytkownik ma nadane nowe hasło wpisane przez administratora

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Autopmatyczne generowanie hasła

1 - 4. Tak samo, jak w SCENARIUSZU GŁÓWNYM
5. a. Administrator wybiera przycisk "Generuj hasło automatycznie"
     << invoke >> Generowanie hasła użytkownika
6 - 11. Tak samo, jak w scenariuszu głównym.

**POST:** Wybrany użytkownik ma nadane nowe hasło wygenerowane przez system.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Błąd zapisu danych

1-6. Tak samo, jak w SCENARIUSZU GŁÓWNYM
   \[ BŁĄD ZAPISU DANYCH ]
7. b. System wyświetla komunikat o błedzie zapisu hasła w bazie dancych.
8. b. Administrator wybiera opcję "OK".
9. b. System wyświetla ponownie listę użytkowników.

**POST:** Wybrany użytkownik nie ma nadanego nowego hasła

## 3. SŁOWNIK POJĘĆ

### Formularz nadania hasła

* **Definicja**: Formularz używany do nadani hasła przez administratora
- **Atrybuty**:  
  - NewPassword: tekst  

 ### komunikat o sukcesie nadania hasła

* **Definicja**: komunikat informujący administratora o sukcesie operacji nadania hasła
- **Atrybuty**:  
  - message: tekst 


 ### komunikat o błedzie zapisu hasła

* **Definicja**: komunikat informujący administratora o błedzie podczas operacji zapisania hasła
- **Atrybuty**:  
  - message: tekst 
  