# PU011: Wyświetlenie listy metadanych

#### Autor: Bartosz Cylwik

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU011

PRE: Adminsitrator jest zalogowany do systemu

1. Administrator wybiera opcję "Wyświetl metadane".
2. System wyświetla liste dostępnych metadanych.\
<< invoke >> Wyświetlenie szczegółow metadanej  

FINAL: Success\
POST: Metadane zostały poprawnie wyświetlone

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Brak metadanych w systemie  

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
    [ Brak metadanych ]
2. a System wyświetla komunikat o braku metadanych z przyciskiem "Powrót do Panelu Adminiistracyjnego"
3. a Administrator klika przycisk "Powrót do Panelu Administracyjnego"

FINAL: Failoure\
POST: Metadane nie zostały wyświetlon, gdyż nie ma ich w bazie

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - System nie odpowiada dla endpointu wyświetlenia metadanych  

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
    [ Przerwa w funkcjonowaniu systemu ]
2. b System wyświetla komunikat "Funkcjonalność niedostępna" z przyciskiem "Powrót do Panelu Administracyjnego"
3. b Administrator klika przycisk "Powrót do Panelu Administracyjnego"

FINAL: Failoure\
POST: Metadane nie zostały wyświetlone z powodu problemu kominukacji z serwerem.

## 3. SŁOWNIK POJĘĆ

### Metadane  
- **Definicja**: Dane na temat źródła danych.  
- **Atrybuty**: 
  - ID: liczba
  - Nazwa: tekst
  - Opis: tekst
  - Właściciel: tekst
  - Data utworzenia: data
  - Data aktualizacji: data
  - status: enum
  - czy_zarchiwizowane: bool

### Panel Administracyjny
- **Definicja**: Interfejs umożliwiający zarządzanie zasobami systemu przez uprawnionych użytkowników (administratorów). 

