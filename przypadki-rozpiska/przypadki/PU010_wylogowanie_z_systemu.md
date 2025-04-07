# PU010: Wylogowanie użytkownika

#### Autor: Kamil Mądrzyk

## 1. Cel przypadku użycia  
Umożliwienie użytkownikowi bezpiecznego zakończenia sesji pracy z systemem.

## 2. Aktorzy  
- Użytkownik

## 3. Przebieg główny  
1. Użytkownik wybiera opcję „Wyloguj się” z menu użytkownika.  
2. System prezentuje użytkownikowi komunikat potwierdzający zamiar wylogowania.  
3. Użytkownik potwierdza operację wylogowania.  
4. System kończy aktywną sesję użytkownika.  
5. System prezentuje ekran potwierdzający pomyślne wylogowanie wraz z opcją ponownego zalogowania się.

## 4. Przebiegi alternatywne  

### 4.1. Użytkownik anuluje operację wylogowania  
1. Użytkownik anuluje operację wylogowania.  
2. System pozostawia aktywną sesję i powraca do ekranu, na którym użytkownik przebywał przed wybraniem opcji wylogowania.

## 5. Warunki początkowe  
- Użytkownik jest zalogowany do systemu i posiada aktywną sesję.

## 6. Warunki końcowe  
- W przypadku udanego wylogowania użytkownik nie ma dostępu do wystawiania ocen metadanych, ani ponownego wylogowania się.  
- Może się jednak ponownie zalogować oraz przeglądać metadane.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Rozszerzenia  
- Automatyczne wylogowanie przy braku aktywności użytkownika

## 9. Słownik pojęć dla PU0002  

### Sesja użytkownika  
- **Definicja**: Okres, w którym użytkownik jest aktywnie zalogowany do systemu i posiada dostęp do jego funkcjonalności  
- **Synonim**: Sesja  
- **Użycie**: Sesja użytkownika trwa od momentu zalogowania do wylogowania lub wygaśnięcia

### Wylogowanie  
- **Definicja**: Proces bezpiecznego zakończenia sesji użytkownika, w wyniku którego dostęp do akcji dostępnych tylko po zalogowaniu jest blokowany do czasu ponownego zalogowania  
- **Synonim**: Zamknięcie sesji, Zakończenie pracy  
- **Użycie**: Użytkownik wylogowuje się z systemu w celu zakończenia pracy

### Ekran potwierdzający  
- **Definicja**: Interfejs użytkownika informujący o pomyślnym zakończeniu danej operacji  
- **Synonim**: Komunikat końcowy  
- **Użycie**: Po wylogowaniu użytkownik widzi ekran potwierdzający

### Automatyczne wygaśnięcie sesji  
- **Definicja**: Mechanizm bezpieczeństwa, który po określonym czasie bez aktywności użytkownika automatycznie kończy sesję w celu ochrony danych  
- **Synonim**: Auto-wylogowanie  
- **Użycie**: Jeśli użytkownik nie wykonuje żadnych działań, system automatycznie kończy sesję