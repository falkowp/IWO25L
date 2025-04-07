# PU016: Archiwizacja metadanych

#### Autor: Mateusz Tyl

## 1. Cel przypadku użycia  
Administrator może oznaczyć wybrane metadane jako archiwalne, co pozwala wykluczyć je z bieżącej edycji i eksploatacji, a jednocześnie zachować je w systemie dla celów historycznych i audytowych.

## 2. Aktorzy  
- Administrator

## 3. Przebieg główny  
1. Administrator otwiera widok listy metadanych lub widok szczegółów konkretnego zestawu metadanych.  
2. Administrator wybiera zestaw metadanych do archiwizacji.  
3. System prezentuje opcję „Oznacz jako archiwalne” (lub „Archiwizuj”).  
4. Administrator klika opcję archiwizacji.  
5. System wyświetla komunikat z prośbą o potwierdzenie operacji (opcjonalnie z informacją o konsekwencjach archiwizacji).  
6. Administrator potwierdza decyzję.  
7. System oznacza wybrane metadane jako zarchiwizowane.  
8. System wyświetla komunikat o pomyślnej archiwizacji.

## 4. Przebiegi alternatywne  

### 4.1. Metadane już zarchiwizowane lub usunięte  
1. Administrator wybiera metadane do archiwizacji.  
2. System wykrywa, że metadane są już zarchiwizowane lub usunięte.  
3. System informuje administratora o stanie metadanych.  
4. System powraca do listy metadanych lub widoku szczegółów.

### 4.2. Rezygnacja z archiwizacji  
1. Administrator anuluje operację archiwizacji.  
2. System anuluje procedurę i pozostawia metadane bez zmian.  
3. System powraca do widoku listy lub szczegółów metadanych.

## 5. Warunki początkowe  
- Administrator jest zalogowany do systemu.  
- Administrator posiada uprawnienia do archiwizacji metadanych.  
- Administrator znajduje się na liście metadanych lub w widoku szczegółów danego zestawu metadanych.

## 6. Warunki końcowe  
- Metadane posiadają status „zarchiwizowane”.  
- Nie są dostępne do dalszej edycji.  
- Administrator otrzymał potwierdzenie archiwizacji.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Rozszerzenia  
*Nie określono.*

## 9. Słownik pojęć dla PU016  

### Metadane  
- **Definicja**: Informacje opisujące i charakteryzujące źródło danych lub inny zasób w systemie.  
- **Użycie**: Metadane mogą być przeglądane, edytowane lub archiwizowane przez administratora.

### Archiwizacja metadanych  
- **Definicja**: Proces zmiany statusu metadanych na „zarchiwizowane” — dane te nie są edytowalne, ale pozostają w systemie.  
- **Użycie**: Archiwizowane metadane są wyłączone z bieżącej eksploatacji.

### Panel administracyjny  
- **Definicja**: Interfejs dostępny dla administratora do zarządzania metadanymi i konfiguracją systemu.  
- **Użycie**: Panel pozwala m.in. na wykonanie operacji archiwizacji.]