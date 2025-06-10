# PU037: Zgłaszanie błędów i problemów z metadanymi

#### Autor: Kamil Mądrzyk

## Scenariusz główny
PRE: Użytkownik jest zalogowany. Użytkownik przegląda szczegóły metadanych.
1. Użytkownik klika "zgłoś problem".
2. System wyświetla formularz zgłoszenia.
3. Użytkownik wypełnia formularz zgłoszenia.
<<invoke>> Walidacja formularza zgłoszenia.
[dane poprawne]
4. System zapisuje formularz zgłoszenia.
5. System wyświetla potwierdzenie.
final: success
POST: Formularz zgłoszenia dodany do bazy danych.

## Scenariusz alternatywny 
PRE: Walidacja formularza zgłoszenia zakończona niepowodzeniem.
4a. System wyświetla komunikat o błędzie.
final: failure.
POST: Powrót do punktu 3 scenariusza głównego.

## Słownik pojęć
### Użytkownik
- **Definicja**: Osoba korzystająca z aplikacji w celu przeglądania, wyszukiwania, oceniania i zgłaszania problemów.
- **Atrybuty**:
  - id: int
  - imię: string
  - nazwisko: string
  - email: string
  - login: string
  - hasło: string
  - rola: string
  - uprawnienia: string
### Zgłoszenie
- **Definicja**: Zgłoszenie na temat błędów w metadanych.
- **Atrybuty**:
  - id: int
  - komentarz: string
  - załącznik: string
  - autor: string
  - status: string
  - czasRozpatrzenia: data
  - dataUtworzenia: data
  - dataModyfikacji: data
### Metadane
- **Definicja**: Dane na temat źródła danych
- **Atrybuty**:
  - id: int
  - idŹródła: int
  - dataUtworzenia: data
  - dataAktualizacji: data
  - osobaKontaktowa: string
  - emailKontaktowy: string
  - licencja: string
