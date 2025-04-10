# PU005: Logowanie w systemie


#### Autor: Bartosz Cylwik

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU005


PRE: Użytkownik nie jest zalogowany do systemu i jest na stronie logowania


1. Użytkownik wybiera opcje "Zaloguj się"
2. System wyświetla "formularz logowania użytkownika"\
<< invoke >> [wybrano opcje] Zaloguj się
3. Użytkownik wprowadza dane logowania
4. Użytkownika wybiera opcje "Zatwierdź"
5. System weryfikuje dane logowania\
<< invoke >> [wybrano opcje] Zatwierdź\
[ DANE POPRAWNE i MNIEJ NIŻ 5 PRÓB LOGOWAŃ ]
6. System uwierzytelnia Użytkownika
7. System przekierowuje Użytkownika do jego panelu głównego


FINAL: success\
POST: Użytkownik jest zalogowany w systemie


## 2. PRZEBIEGI ALTERNATYWNE


### 2.1. SCENARIUSZ ALTERNATYWNY PU005-1 - Dane logowania są niepoprawne


1.-5. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU005\
[ DANE NIEPOPRAWNE i MNIEJ NIŻ 5 PRÓB LOGOWAŃ ]\
6a. System wyświetla komunikat o błędzie logowania\
7a. Powrót do 2. z SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU005


FINAL: failure\
POST: Użytkownik nie jest zalogowany w systemie


### 2.2. SCENARIUSZ ALTERNATYWNY PU005-2 - Więcej niż 5 prób logowań  


1.-5. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU005\
[ WIĘCEJ NIŻ 5 PRÓB LOGOWAŃ ]\
6b. System wyświetla komunikat o zbyt dużej liczbie logowań\
7b. Powrót do 2. z SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU005


FINAL: failure\
POST: Użytkownik nie jest zalogowany w systemie


### 2.3. SCENARIUSZ ALTERNATYWNY PU005-3 - Anulacja logowania 


1c. Użytkownika wybiera opcje "Anuluj"\
2c. System powraca do ekranu głównego\
<< invoke >> [wybrano opcje] Anuluj


FINAL: failure\
POST: Użytkownik nie jest zalogowany w systemie


## 3. SŁOWNIK POJĘĆ

### Formularz logowania użytkownika
  - **Definicja**: Formularz posiadający pola w których można podać dane logowania

### Dane logowania
  - **Definicja**: Dane potrzebne do zalogowania użytkownika w systemie
  - **Atrybuty**: 
    - Nazwa/email: tekst
    - Hasło: tekst
    - OAuth_kod: liczba
