# Przypadek użycia: PU037: Zgłaszanie błędów i problemów z metadanymi

**Autor:** Artem Omelchenko\
**Cel:** Użytkownik może zgłosić błędy dotyczące wybranych metadanych.

## Aktorzy
- Użytkownik

## Warunki wstępne
- Użytkownik jest zalogowany do systemu
- Użytkownik znajduje się na stronie szczegółów metadanych [(PU019)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.1.wymagania.funkcjonalne/PU0005.md)

## Scenariusz podstawowy
1. Użytkownik naciska przycisk "Zgłoś problem" przy wybranych metadanych
2. System wyświetla formularz zgłoszenia zawierający:
   - Pole opisu problemu
   - Kategorię problemu (np. błędne dane, nieaktualne informacje, problemy techniczne)
   - Możliwość dodania załącznika (np. zrzut ekranu)
3. Użytkownik wypełnia formularz zgłoszenia
4. Użytkownik zatwierdza zgłoszenie przyciskiem "Wyślij"
5. System waliduje wprowadzone dane
6. System zapisuje zgłoszenie i przypisuje mu unikalny identyfikator
7. System wyświetla potwierdzenie przyjęcia zgłoszenia

## Scenariusze alternatywne
**5a.** Formularz zawiera błędy\
**5a.1.** System wyświetla komunikat o błędach\
**5a.2.** Użytkownik poprawia błędy\
**5a.3.** Powrót do kroku 4

## Warunki końcowe
- Zgłoszenie zostało zapisane w systemie
- Użytkownik otrzymał potwierdzenie przyjęcia zgłoszenia
- Administrator zostaje powiadomiony o nowym zgłoszeniu

## Wyjątki
- **W przypadku błędów walidacji**: Jeśli wprowadzone dane nie spełniają wymagań (np. pole opisu jest puste), system wyświetla komunikat o błędzie i prosi użytkownika o poprawienie danych.

- **W przypadku problemów z zapisem do bazy danych**: Jeśli wystąpi błąd podczas zapisywania zgłoszenia (np. problem z serwerem), system informuje użytkownika o błędzie i sugeruje ponowną próbę wysłania zgłoszenia.

## Słownik pojęć
- **Metadane** – dane opisujące inne dane, zawierające informacje o ich strukturze, pochodzeniu i sposobie wykorzystania.
[(Metadane)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.3.slownik/4.3.2.slownik.dziedziny/slownik.dziedziny.md)
- **Zgłoszenie** – w systemie, wpis zawierający informacje o zaobserwowanym problemie, potrzebie lub incydencie zgłoszonym przez użytkownika.
[(Zgłoszenie)](../../dokumentacja/specyfikacja.wymagan/4.wymagania.uzytkownika/4.3.slownik/4.3.2.slownik.dziedziny/slownik.dziedziny.md)
