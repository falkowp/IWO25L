# Przypadek użycia: PU015: Wyszukanie źródła danych:

**Autor:** Jakub Wypych\
**Cel:** Administrator może przeszukiwać istniejące metadane.

## Aktorzy
- Administrator

## Warunki wstępne
- Administrator jest zalogowany do systemu.
- Administrator znajduje się na liście metadanych [(PU011)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0002.md)

## Scenariusz podstawowy
1. Administrator podaje filtr.
2. Administrator naciska przycisk "Szukaj".
3. System pobiera metadane na podstawie filtru.
4. System wyświetla pobrane metadane, w tym:
5. Administrator może:
   - Archiwizować metadane [(PU016)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0002.md)
   - Sprawdzić poprawność metadanych [(PU017)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0002.md)
   - Usunąć metadane [(PU018)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0002.md)
   - Wyświetlić informacje o metadanych [(PU019)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0002.md)

## Scenariusze alternatywne
### Reset filtru
**2a.** Administrator resetuje filtry.\
**2a.1.** System informuje o resecie i powraca do listy metadanych.

### Błąd pobrania metadanych
**3a.** System napotyka błąd w pobieraniu metadanych.\
**3a.1.** System informuje o błędzie w pobraniu metadanych i powraca do listy metadanych.

## Warunki końcowe
- Administrator ma wyświetlone metadane na podstawie filtru.

## Wyjątki
- W przypadku błędu pobrania danych system powinnien wyświetlić informacje o błędzie pobioru metadanych.

## Słownik pojęć 
- **Filtr** - informacje na podstawie których będą szukane metadane, gdzie informacjami sa atrybuty metadanych.
[(Metadane)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.3.slownik/4.3.2.slownik.dziedziny/slownik.dziedziny.md)
