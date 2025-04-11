# PU012: Eksport listy metadanych do pliku

#### Autor: [Maciej Przybylski]

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU012

PRE: 
	Administrator jest zalogowany do systemu.  
	Administrator posiada uprawnienia do eksportu metadanych do pliku.  
	System zawiera metadane do eksportu.

1. System generuje plik eksportu listy metadanych.  
    [ PLIK WYGENEROWANY PRAWIDŁOWO ]
2. System zapisuje log eksportu listy metadanych.
3. System wyświetla plik eksportu listy metadanych.
4. Administrator pobiera plik eksportu listy metadanych. 

FINAL: Success 

POST: 
	Plik eksportu listy metadanych znajduje się na komputerze Administratora.  
    Log eksportu listy metadanych znajduje się w systemie.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Plik wygenerowany nieprawidłowo

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM  
    [ PLIK WYGENEROWANY NIEPRAWIDŁOWO ] 
2. a. System wyświetla komunikat "Wystąpił błąd podczas tworzenia pliku. Proszę spróbować ponownie później." 
3. a. System zapisuje log szczegółów błędu eksportu listy metadanych. 
4. a. Administrator wybiera opcję "OK".
5. System zamyka formularz eksportu listy metadanych. 

FINAL: Failure 

POST: 
	Plik eksportu listy metadanych nie znajduje się na komputerze Administratora.  
    Log szczegółów błędu eksportu listy metadanych znajduje się w systemie.

## 3. SŁOWNIK POJĘĆ

### Lista metadanych

- **Definicja**: Zbiór danych zawierający pewną liczbę wybranych metadanych.
- **Atrybuty**:
    - Nazwa: tekst
    - Opis: tekst
    - Data utworzenia: data
	- Zawartość: metadane [Lista]

### Plik eksportu listy metadanych

- **Definicja**: Plik zawierający listę metadanych w określonym formacie, umożliwiający przenoszenie danych między komputerami oraz analizę danych.
- **Atrybuty**:
    - Format: tekst
    - Rozmiar: liczba
    - Zawartość: lista metadanych
    - Data wygenerowania: data

### Log eksportu listy metadanych

- **Definicja**: Zapis w systemie dokumentujący pomyślne wykonanie operacji eksportu listy metadanych.
- **Atrybuty**:
    - ID: liczba
    - Data operacji: data
    - Użytkownik: tekst
    - Opis: tekst

### Log szczegółów błędu eksportu listy metadanych

- **Definicja**: Rozszerzony zapis w systemie dokumentujący niepowodzenie operacji eksportu wraz ze szczegółowymi informacjami o błędzie.
- **Atrybuty**:
    - ID: liczba
    - Data operacji: data
    - Użytkownik: tekst
    - Status: tekst
    - Kod błędu: tekst
    - Szczegóły błędu: tekst
    - Ślad stosu: tekst

