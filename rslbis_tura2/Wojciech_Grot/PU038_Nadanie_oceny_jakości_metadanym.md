# **PU0038: Nadanie oceny jakości metadanym**

#### Autor: Wojciech Grot

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Użytkownik jest zalogowany do systemu i wyświetla szczegóły metadanych.

1. Użytkownik wybiera ocenę.
2. Użytkownik klika przycisk "wyślij ocenę".
3. System wyswietla "formularz wyboru oceny"
4. Użytkownik wybiera ocenę od 1 do 5
5. Uzytkownik wybiera przycisk "nadaj ocenę"
6. System wyświetla komunikat "nadano ocenę".

**POST:** Ocena dodana do bazy danych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Użytkownik anulował wystawienie oceny

2a. Użytkownik klika przycisk "anuluj".

**POST:** Powrót do wyświetlania szczegółów metadanych.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Użytkownik próbuje wysłać ocenę bez wyboru.

4b. Użytkownik klika przycisk "wyślij ocenę".

**POST:** Przycisk nie zareagował.

## 3. SŁOWNIK POJĘĆ

### Użytkownik  
- **Definicja**: Osoba korzystająca z systemu.  
- **Atrybuty**:  
  - ID: numer  
  - Imię: tekst  
  - Nazwa: string  
  - Hasło: string  
  - Uprawnienia: enum  
  - Role: enum