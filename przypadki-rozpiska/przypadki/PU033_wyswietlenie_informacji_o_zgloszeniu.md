# Przypadek użycia: PU033: Wyświetlenie informacji o zgłoszeniu:

**Autor:** Jan Gębal\
**Cel:** Administrator może zobaczyć szczegóły konkretnego zgłoszenia użytkownika.

## Aktorzy
- Administrator

## Warunki wstępne
- Administrator jest zalogowany do systemu.
- Administrator znajduje się na liście zgłoszeń użytkownika [(PU030)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0005.md) w panelu admninistratora

## Scenariusz podstawowy
1. Administrator naciska przycisk "Wyświetl szczególy" przy wybranym zgłoszeniu.
2. System wyświetla szczegółowe informacje dotyczące zgłoszenia, w tym:
3. Administrator może:
   - Przyjąć zgłoszenie [(PU034)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0005.md)
   - Odrzucić zgłosenie [(PU035)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0005.md)

## Scenariusze alternatywne
**2a.** Zgłoszenie zostało usunięte.\
**2a.1.** System informuje o usunięciu i powraca do listy zgłoszeń.

## Warunki końcowe
- Administrator zapoznał się ze szczegółami zgłoszenia, ewentualnie wykonał dodatkowe działania administracyjne.

## Wyjątki
- W przypadku błędu ładowania danych zgłoszenia (np. problem z serwerem), system wyświetla odpowiedni komunikat i daje możliwość ponownego załadowania strony.

## Słownik pojęć
- **Zgłoszenie** – w systemie, wpis zawierający informacje o zaobserwowanym problemie, potrzebie lub incydencie zgłoszonym przez użytkownika.
[(Zgłoszenie)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.3.slownik/4.3.2.slownik.dziedziny/slownik.dziedziny.md)  
- **Panel administracyjny** – specjalny interfejs umożliwiający zarządzanie zasobami i danymi systemu, dostępny tylko dla administratorów. 
