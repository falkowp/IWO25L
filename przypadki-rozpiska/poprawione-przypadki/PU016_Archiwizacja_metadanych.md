# PU016: Archiwizacja metadanych

#### Autor: Marta Stankevich

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU016

PRE: Admin jest zalogowany, posiada uprawnienia do archiwizacji metadanych. Admin znajduje się na liście metadanych z już wybranym zestawem metadanych do archiwizacji.

1. System prezentuje opcję "Archiwizuj".
2. Administrator klika opcję archiwizacji.  
3. System wyświetla komunikat z prośbą o potwierdzenie operacji, wyświetla opcję "potwierdzam" i "anuluj".
4. Administrator klika opcję "potwierdzam".  
5. System oznacza wybrane metadane jako zarchiwizowane.  
6. System wyświetla komunikat o pomyślnej archiwizacji.

FINAL: success
POST: Wybrany zesraw metadanych posiada status "zarchiwizowane", nie jest dostępny do edycji.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Metadane już zarchiwizowane lub usunięte

1a. Tak samo, jak w SCENARIUSZU GŁÓWNYM
2a. Tak samo, jak w SCENARIUSZU GŁÓWNYM
3a. System wykrywa, że metadane posiadają status "zarchiwizowane".
4a. System informuje administratora o statusie metadanych.  
5a. System powraca do listy metadanych.

FINAL: Failiure
POST: Żadne metadane otrzymały status "zarchiwizowane".


### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Rezygnacja z archiwizacji  

1b. Tak samo, jak w SCENARIUSZU GŁÓWNYM
2b. Tak samo, jak w SCENARIUSZU GŁÓWNYM
3b. Tak samo, jak w SCENARIUSZU GŁÓWNYM
4b. Administrator klika opcję "anuluj"  
5b. System anuluje procedurę i pozostawia metadane bez zmian.  
6b. System powraca do widoku listy lub metadanych.

FINAL: Failiure
POST: Żadne metadane otrzymały status "zarchiwizowane".


## 3. SŁOWNIK POJĘĆ

### Metadane   
- **Definicja**: Informacje opisujące i charakteryzujące źródło danych lub inny zasób w systemie.
- **Atrybuty**: 
  - ID: liczba
  - STATUS: tekst


### Archiwizacja metadanych  
- **Definicja**: Proces zmiany statusu metadanych na „zarchiwizowane” — dane te nie są edytowalne, ale pozostają w systemie.  


### Lista metadanych
- **Definicja**: Llista zawierająca pewne wybrane metadane.


