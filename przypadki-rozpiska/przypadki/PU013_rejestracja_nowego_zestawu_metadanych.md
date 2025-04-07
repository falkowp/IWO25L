# PU013: Rejestreacja nowego zestawu metadanych
**Autor:** Wojciech Grot
**ID:** PU013        **Nazwa:** Rejestracja nowego zestawu metadanych 
**Wersja:** 1.0      **Waga** 10      **UCP:** 9,46  
**Trudność:** średnia     

---
## Aktorzy główni: 

Administrator

## Cel: 

Rejestracja nowego zestawu metadanych

## Warunek rozpoczęcia: 
Administrator jest zalogowany w systemie i posiada odpowiednie uprawnienia do rejestrowania noweych zestawów metadanych
ORAZ
Administrator posiada wszystkie niezbędne informacje o rejestrowanym zestawie metadanych

## Scenariusz główny:
1. Administrator wybiera opcję "Zarejestruj nowy zestaw metadanych" w interfejsie systemu.
2. System wyświetla formularz rejestracji nowego zestawu metadanych, zawierający pola `nazwa`, `opis`, `właściciel`, `data aktualizacji`, oraz możliwe `tagi` do wyboru.  
3. Po wprowadzeniu wszystkich wymaganych informacji, administrator zatwierdza formularz.
4. System zapisuje wprowadzone metadane w bazie danych, tworząc rekord nowego zestawu metadanych.
5. System wyświetla potwierdzenie pomyślnej rejestracji nowego zestawu metadanych.
6. Nowy zestaw staje się widoczne na liście dostępnych zestawów metadanych dla użytkowników.


## Scenariusze alternatywne:

**Niekompletne dane:**
1. W kroku 2, administrator próbuje zatwierdzić formularz z brakującymi obowiązkowymi polami metadanych.
2. System wyświetla komunikat o błędzie wskazujący brakujące pola i uniemożliwia zatwierdzenie formularza do czasu ich uzupełnienia.

**Anulowanie rejestracji:**
1. W dowolnym momencie przed zatwierdzeniem formularza (krok 3), administrator wybiera opcję "Anuluj".
2. System zamyka formularz rejestracji bez zapisywania wprowadzonych danych.
3. System powraca do poprzedniego widoku.

## Warunki zakończenia:  
- (**sukces**) ⇒ Nowy zestaw metadancyh wraz został pomyślnie zarejestrowany w systemie i jest dostępny dla użytkowników

- (**porażka**) ⇒ Proces rejestracji został przerwany przez administratora, a żadne nowe dane nie zostały zapisane.

- (**porażka**) ⇒ W zestawie metadanych znajdował się bład, przez który system odrzucił rejestrację.

-------------------------
## Słownik pojęć:
- Zestaw metadanych: Zbiór danych z określonego miejsca lub instytucji, udostępniany w określonym formacie. Zawierają informacje takie jak nazwa, opis, data utworzenia, data aktualizacji, właściciel.
- Rejestracja: Proces wprowadzania informacji o nowym elemencie (w tym przypadku zestawie matadanych) do systemu.
- Formularz rejestracji: Interfejs użytkownika, który umożliwia administratorowi wprowadzenie metadanych nowego źródła danych.
- Baza danych: Zorganizowany zbiór danych przechowywanych elektronicznie.
- Rekord: Zestaw powiązanych danych, traktowanych jako pojedyncza jednostka w bazie danych (w tym przypadku, dane jednego zestawu).
- Uprawnienia: Prawa dostępu do określonych funkcji i danych w systemie. Dodawanie nowych informacji wymaga specjalnych uprawnień
- Użytkownik: Osoba korzystająca z systemu. Może to być pracownik jednostki samorządowej, administrator, lokalny przedsiębiorca, mieszkaniec
- Lista zestawów metadanych: Wyświetlana w systemie lista dostępnych zestawów metadanych, którą użytkownik może przeglądać
