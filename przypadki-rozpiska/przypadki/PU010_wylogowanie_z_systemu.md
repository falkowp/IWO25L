Autor: Kamil Mądrzyk

**Cel:**
Umożliwienie użytkownikowi bezpiecznego zakończenia sesji pracy z systemem.

**Aktorzy:**
- Użytkownik

**Warunki wstępne:**
- Użytkownik jest zalogowany do systemu i posiada aktywną sesję.

**Scenariusz podstawowy:**
1. Użytkownik wybiera opcję „Wyloguj się” z menu użytkownika.
2. System prezentuje użytkownikowi komunikat potwierdzający zamiar wylogowania.
3. Użytkownik potwierdza operację wylogowania.
4. System kończy aktywną sesję użytkownika.
5. System prezentuje ekran potwierdzający pomyślne wylogowanie wraz z opcją ponownego zalogowania się.

**Scenariusze alternatywne:**
3a. Użytkownik anuluje operację wylogowania.
3a.1 System pozostawia aktywną sesję i powraca do ekranu, na którym użytkownik przebywał przed wybraniem opcji wylogowania.

**Warunki końcowe:**
W przypadku udanego wylogowania użytkownik nie ma dostępu do wystawiania ocen metadanych, ani ponownego wylogowania się. Może się jednak ponownie zalogować oraz przeglądać metadane.

**Wyjątki:**
Jeśli sesja wygaśnie automatycznie (np. w wyniku braku aktywności), system automatycznie wykonuje procedurę wylogowania.

**Słownik pojęć:**
- Sesja użytkownika – okres, w którym użytkownik jest aktywnie zalogowany do systemu i posiada dostęp do jego funkcjonalności.
- Wylogowanie – proces bezpiecznego zakończenia sesji użytkownika, w wyniku którego dostęp do akcji dostępnych tylko po zalogowaniu jest blokowany do czasu ponownego zalogowania.
- Ekran potwierdzający – interfejs użytkownika informujący o pomyślnym zakończeniu danej operacji.
- Automatyczne wygaśnięcie sesji – mechanizm bezpieczeństwa, który po określonym czasie bez aktywności użytkownika automatycznie kończy sesję w celu ochrony danych.