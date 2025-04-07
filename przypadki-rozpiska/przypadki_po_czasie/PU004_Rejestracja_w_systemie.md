# Przypadek użycia: PU004: Rejestreacja w systemie
| Pole        | Wartość           |
|-------------|--------------------|
| **Autor**   | Marcin Komza       |
| **ID**      | PU004              |
| **Wersja**  | 1.0                |
| **Waga**    | 10                 |
| **UCP**     | 9,46               |
| **Trudność**| średnia            |

---
## Aktorzy główni: 

Użytkownik

## Cel: 

Rejestracja w systemie

## Warunek rozpoczęcia: 
brak

## Scenariusz główny:
1. Użytkownik wybiera opcję "Zarejestruj się" w interfejsie systemu.
2. System wyświetla formularz rejestracji nowego użytkownika, zawierający pola `Imię`, `Nazwisko`, `Nazwa użytkownika`, `Adres E-mail`, `Hasło`, `Powtórz Hasło`
3. Po wprowadzeniu wszystkich wymaganych informacji, użytkownik zatwierdza formularz.
4. System sprawdza poprawność wprowadzonych danych
5. System wysyła wiadomość z kodem na podany adres e-mail.
6. System wyświetla formularz potwierdzenia kodem z email, zawierający pole `Kod potwierdzający`
7. Po wprowadzeniu kodu, użytkownik zatwierdza formularz
8. System sprawdza wpisany kod
9. System zapisuje wprowadzone dane w bazie danych, tworząc nowego użytkownika.
10. System wyświetla potwierdzenie pomyślnej rejestracji nowego użytkownika.


## Scenariusze alternatywne:

**Niepoprawne lub niepełne dane:**\
4a.1. System zaznacza na czerwono niepoprawne lub nie wypełnione pola formularza\
4a.2. System wyświetla komunikat o niepoprawnych lub niepełnych danych\
4a.3. System blokuje przejście do kolejnego ekran do czasu zmiany danych

**Instnieje użytkownik z podanym adresem e-mail lub nazwą:**\
4b.1. System wyświetla komunikat z informacją że taki użytkownik już istnieje\
4b.2. System blokuje przejście do kolejnego ekran do czasu zmiany danych

**Pola z hasłami nie zgadzają się:**\
4c.1. System usuwa zawartość pól `Hasło` oraz `Powtórz hasło`\
4c.2. System wyświetla komunikat o niezgadzających się hasłach\
4c.3. System blokuje przejście do kolejnego ekran do czasu zmiany danych

**Kod potwierdzający nie zgadza się**\
8a.1. System usuwa zawartość pola `Kod potwierdzający`\
8a.2. System wysyła nowy kod na adres e-mail\
8a.3. System wyświetla komunikat o niepoprawnym kodzie

**Anulowanie rejestracji:**\
2a = 6a\
6a.1. Użytkownik wciska przycisk `anuluj`\
6a.2. System zamyka formularz rejestracji bez zapisywania wprowadzonych danych.\
6a.3. System powraca do poprzedniego widoku.

## Warunki zakończenia:  
- (**sukces**) ⇒ Nowy użytkownik został zarejestrowany w systemie, można zalogować się na to konto

- (**porażka**) ⇒ Proces rejestracji został przerwany przez użytkownika, a żadne nowe dane nie zostały zapisane.

- (**porażka**) ⇒ Użytkownik nie potwierdził adresu e-mail kodem, żadne nowe dane nie zostały zapisane.

-------------------------
## Słownik pojęć:
- **Użytkownik** – Osoba fizyczna lub podmiot, który korzysta z systemu i rejestruje się, aby uzyskać dostęp do jego funkcjonalności.
- **Formularz rejestracji** – Interfejs graficzny zawierający pola do wprowadzenia danych potrzebnych do utworzenia nowego konta w systemie.
- **Nazwa użytkownika** – Unikalny identyfikator przypisany użytkownikowi, służący do logowania do systemu.
- **Adres e-mail** – Elektroniczny adres poczty, wykorzystywany do komunikacji z użytkownikiem oraz do potwierdzenia rejestracji.
- **Hasło** – Sekretny ciąg znaków służący do uwierzytelnienia użytkownika.
- **Powtórz hasło** – Pole służące do ponownego wprowadzenia hasła w celu weryfikacji poprawności wpisu.
- **Kod potwierdzający** – Tymczasowy kod wysyłany na adres e-mail użytkownika w celu potwierdzenia jego tożsamości podczas rejestracji.
