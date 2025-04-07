**Przypadek użycia: PU016: Archiwizacja metadanych**  
**Autor:** Mateusz Tyl 325520 \
**Cel:** Administrator może oznaczyć wybrane metadane jako archiwalne, co pozwala wykluczyć je z bieżącej edycji i eksploatacji, a jednocześnie zachować je w systemie dla celów historycznych i audytowych.

---

### Aktorzy  
- **Administrator**  

---

### Warunki wstępne  
1. Administrator jest zalogowany do systemu.  
2. Administrator posiada uprawnienia do zarządzania metadanymi (w tym do ich archiwizacji).  
3. Administrator znajduje się na liście metadanych lub w widoku szczegółów konkretnego zestawu metadanych (np. w panelu administratora, gdzie może przeglądać i edytować metadane).

---

### Scenariusz podstawowy  
1. Administrator otwiera widok listy metadanych (lub widok szczegółów konkretnego zestawu metadanych).  
2. Administrator wybiera zestaw metadanych, który chce zarchiwizować.  
3. System prezentuje przycisk lub opcję „Oznacz jako archiwalne” (lub „Archiwizuj”).  
4. Administrator klika przycisk „Archiwizuj” przy wybranych metadanych.  
5. System wyświetla komunikat z prośbą o potwierdzenie operacji archiwizacji (opcjonalnie może wyświetlić informacje o konsekwencjach – np. brak możliwości dalszej edycji tych metadanych).  
6. Administrator potwierdza decyzję o archiwizacji metadanych.  
7. System oznacza wybrane metadane jako archiwalne (zmienia ich status na „zarchiwizowane”).  
8. System wyświetla komunikat o pomyślnej archiwizacji.  

---

### Scenariusze alternatywne  
**2a. Metadane, które Administrator próbuje zarchiwizować, zostały już wcześniej zarchiwizowane lub usunięte.**  
2a.1. System informuje Administratora, że dane metadane są już w stanie archiwalnym bądź nie istnieją (np. zostały usunięte).  
2a.2. System powraca do listy metadanych lub widoku szczegółów bez wykonywania dalszych czynności.  

**5a. Administrator rezygnuje z archiwizacji metadanych.**  
5a.1. System anuluje procedurę archiwizacji i pozostawia metadane w dotychczasowym stanie.  
5a.2. System wyświetla listę metadanych lub widok szczegółów, dając możliwość wykonania innych operacji.  

---

### Warunki końcowe  
- Metadane zostały zarchiwizowane i posiadają status „zarchiwizowane”, nie są już dostępne do bieżącej edycji.  
- Administrator otrzymał informację o pomyślnej archiwizacji.  

---

### Wyjątki  
- **Błąd komunikacji z serwerem lub bazy danych.**  
  - System wyświetla odpowiedni komunikat o błędzie i umożliwia Administratorowi ponowienie operacji lub powrót do listy metadanych.  

---

### Słownik pojęć  
- **Metadane** – informacje opisujące i charakteryzujące źródło danych lub inny zasób w systemie; zawierają takie informacje jak nazwa, opis, format, datę aktualizacji itp.  
- **Archiwizacja metadanych** – proces zmiany statusu metadanych w systemie tak, aby nie były aktywnie wykorzystywane i edytowane, ale wciąż możliwe do wglądu w razie potrzeby historycznej lub audytowej.  
- **Panel administracyjny** – specjalny interfejs systemu, dostępny wyłącznie dla Administratorów, służący do zarządzania zasobami i konfiguracją systemu.