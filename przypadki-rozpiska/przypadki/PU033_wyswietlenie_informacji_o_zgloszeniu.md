# PU033: Wyświetlenie informacji o zgłoszeniu

#### Autor: Jan Gębal

## 1. Cel przypadku użycia  
Administrator może zobaczyć szczegóły konkretnego zgłoszenia użytkownika.

## 2. Aktorzy  
- Administrator

## 3. Przebieg główny  
1. Administrator znajduje się na liście zgłoszeń użytkownika w panelu administratora.  
2. Administrator naciska przycisk „Wyświetl szczegóły” przy wybranym zgłoszeniu.  
3. System wyświetla szczegółowe informacje dotyczące zgłoszenia.  
4. Administrator może:  
   - Przyjąć zgłoszenie (PU034) 
   - Odrzucić zgłoszenie (PU035)

## 4. Przebiegi alternatywne  

### 4.1. Zgłoszenie zostało usunięte  
1. System wykrywa brak zgłoszenia.  
2. System informuje Administratora o usunięciu zgłoszenia.  
3. System powraca do listy zgłoszeń.

## 5. Warunki początkowe  
- Administrator jest zalogowany do systemu.  
- Administrator znajduje się na liście zgłoszeń użytkownika (PU030)

## 6. Warunki końcowe  
- Administrator zapoznał się ze szczegółami zgłoszenia.  
- Administrator może wykonać działania administracyjne (przyjęcie lub odrzucenie).

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Wyjątki  
- Błąd ładowania danych zgłoszenia:  
  - System wyświetla komunikat o błędzie.  
  - Umożliwia ponowne załadowanie strony.

## 9. Słownik pojęć  

### Zgłoszenie  
- **Definicja**: Wpis zawierający informacje o problemie, potrzebie lub incydencie zgłoszonym przez użytkownika.  
- **Użycie**: Przeglądany i obsługiwany przez administratora w panelu.

### Panel administracyjny  
- **Definicja**: Interfejs systemu dostępny dla administratorów.  
- **Użycie**: Umożliwia m.in. zarządzanie zgłoszeniami użytkowników.
