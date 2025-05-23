# PU030: Wyświetlenie listy zgłoszeń użytkowników

#### Autor: Bartosz Cylwik

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU030

PRE: Adminsitrator jest zalogowany do systemu

1. Administrator wybiera opcję "Wyświetl zgłoszenia".
3. System pobiera dane z bazy.
2. System wyświetla liste zgłoszeń.\
<< invoke >> Wyświetlenie szczegółow zgłoszenia  

FINAL: Success\
POST: Lista zgłoszeń została poprawnie wyświetlona

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Brak zgłoszeń w systemie  

1.-2. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
    [ Brak zgłoszeń ]
3. a System wyświetla komunikat o braku zgłoszeń z przyciskiem "Powrót do Panelu Administracyjnego"
4. a Administrator klika przycisk "Powrót do Panelu Administracyjnego"

FINAL: Failoure\
POST: Zgłoszenia nie zostały wyświetlone, gdyż nie ma ich w bazie

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Token autoryzacyjny stracił ważność w menu Panelu Administracyjnego  

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM\
    [ Niepoprawność tokenu ]
2. b System wyświetla komunikat "Aby mieć dostęp do zasobu należy się zalogować" z przyciskiem "zaloguj".
3. b Administrator klika przycisk "zaloguj"
4. b System przekierowuje do strony Logowania.

FINAL: Failoure\
POST: Metadane nie zostały wyświetlone z powodu problemu kominukacji z serwerem.

## 3. SŁOWNIK POJĘĆ

### Zgłoszenie użytkownika

* **Definicja**: Prośba, pytanie lub problem zgłoszony przez użytkownika do administratora.

- **Atrybuty**:  
  - ID: numer  
  - ID użytkownika: numer
  - Treść: tekst
  - Status: tekst
  - Data złożenia: data

### Panel Administracyjny
- **Definicja**: Interfejs umożliwiający zarządzanie zasobami systemu przez uprawnionych użytkowników (administratorów).
