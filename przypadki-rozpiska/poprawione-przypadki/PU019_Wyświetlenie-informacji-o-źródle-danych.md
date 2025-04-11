PU019. Wyswietlenie informacj o źródle danych
Autor: Adrian Rybaczuk


Scenariusz główny:
PRE: 1. Użytkownik jest zalogowany 2. Użytkownik posiada rolę "Administratora"

1. Administrator wybiera opcję "Lista użytkowników"
2. System wyświetla okno "Lista użytkowników"
   final: success POST: Wyświetlono listę użytkowników

Scenariusze alternatywne

Scenariusz alternatywny 1:

1. Tak jak w scenariuszu głównym
2. System wyświetla okno z komunikatem
   "Brak użytkowników"
   final: success
   POST: Wyświetlono pustą listę użytkowników

Słownik pojęć:
Administrator - [definicja znajduje się w słowniku nr. 1]

Lista użytkowników -

[Page 2]
Scenariusz Alternatywny 2:

1. Tak jak w scenariuszu głównym
2. Wyświetlenie okno komunikatu
   "Błąd połączenia z bazą danych"
   final: fail POST: Wyświetlenie komunikatu
   o braku możliwości pobrania danych

Słownik pojęć:
Lista użytkowników - lista zawierająca
informacje o użytkownikach systemu

Okno listy użytkowników - okno
wyświetlające dane z "listy użytkowników"

Użytkownik - osoba korzystająca z systemu
Atrybuty id[numer], imię[tekst], nazwa[string], hasło[string], uprawnienia[enum], role[enum]
