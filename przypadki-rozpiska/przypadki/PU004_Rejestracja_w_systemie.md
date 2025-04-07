# PU004: Rejestracja w systemie

#### Autor: Marcin Komza

## 1. Cel przypadku użycia  
Użytkownik może zarejestrować się w systemie, tworząc nowe konto użytkownika.

## 2. Aktorzy  
- Użytkownik

## 3. Przebieg główny  
1. Użytkownik wybiera opcję „Zarejestruj się” w interfejsie systemu.  
2. System wyświetla formularz rejestracji nowego użytkownika, zawierający pola:  
   - Imię  
   - Nazwisko  
   - Nazwa użytkownika  
   - Adres e-mail  
   - Hasło  
   - Powtórz hasło  
3. Użytkownik wypełnia formularz, wpisując wymagane dane.  
4. Użytkownik zatwierdza formularz.  
5. System sprawdza poprawność wprowadzonych danych.  
6. System wysyła wiadomość z kodem potwierdzającym na podany adres e-mail.  
7. System wyświetla formularz weryfikacji kodu, zawierający pole „Kod potwierdzający”.  
8. Użytkownik wprowadza kod otrzymany w wiadomości e-mail.  
9. Użytkownik zatwierdza formularz z kodem.  
10. System sprawdza poprawność wprowadzonego kodu.  
11. System zapisuje dane użytkownika w bazie danych, tworząc nowe konto.  
12. System wyświetla komunikat o pomyślnej rejestracji.

## 4. Przebiegi alternatywne  

### 4.1. Niepoprawne lub niepełne dane  
1. System wykrywa niepoprawne lub brakujące dane w formularzu.  
2. System zaznacza na czerwono pola, które wymagają poprawy.  
3. System wyświetla komunikat o błędzie.  
4. Użytkownik poprawia dane i ponownie wysyła formularz (powrót do kroku 4 przebiegu głównego).  

### 4.2. Istnieje użytkownik z podanym adresem e-mail lub nazwą użytkownika  
1. System wykrywa, że użytkownik o podanym adresie e-mail lub nazwie już istnieje w systemie.  
2. System wyświetla komunikat o błędzie.  
3. System blokuje przejście do kolejnego etapu, dopóki użytkownik nie zmieni danych.  

### 4.3. Pola hasła się nie zgadzają  
1. Użytkownik wprowadza różne wartości w polach „Hasło” i „Powtórz hasło”.  
2. System usuwa zawartość obu pól.  
3. System wyświetla komunikat o niezgodnych hasłach.  
4. System blokuje przejście do kolejnego etapu, dopóki użytkownik nie wprowadzi identycznych haseł.

### 4.4. Kod potwierdzający nie zgadza się  
1. Użytkownik wprowadza nieprawidłowy kod potwierdzający.  
2. System usuwa zawartość pola „Kod potwierdzający”.  
3. System wysyła nowy kod na podany adres e-mail.  
4. System wyświetla komunikat o błędzie i prosi o ponowne wprowadzenie poprawnego kodu.

### 4.5. Anulowanie rejestracji  
1. Użytkownik wciska przycisk „Anuluj” w formularzu rejestracyjnym.  
2. System zamyka formularz bez zapisywania danych.  
3. System powraca do poprzedniego ekranu.

## 5. Warunki początkowe  
- Użytkownik nie jest zalogowany do systemu.  
- Użytkownik przegląda stronę rejestracji.  

## 6. Warunki końcowe  
- **Sukces:** Nowy użytkownik został zarejestrowany w systemie, może się zalogować.  
- **Porażka:** Proces rejestracji został przerwany przez użytkownika, a żadne dane nie zostały zapisane.  
- **Porażka:** Użytkownik nie potwierdził adresu e-mail kodem, a dane nie zostały zapisane.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Wyjątki  

- **Błąd walidacji danych:**  
  - System informuje użytkownika o nieprawidłowych lub brakujących danych i uniemożliwia dalszą rejestrację do momentu ich poprawienia.

- **Błąd zapisu do bazy danych:**  
  - System informuje użytkownika o problemie z zapisem danych (np. problem z serwerem) i sugeruje ponowną próbę rejestracji.

## 9. Słownik pojęć  

### Użytkownik  
- Osoba fizyczna lub podmiot, który korzysta z systemu i rejestruje się w celu uzyskania dostępu do jego funkcji.

### Formularz rejestracji  
- Interfejs służący do wprowadzenia danych użytkownika, niezbędnych do założenia konta w systemie.

### Nazwa użytkownika  
- Unikalny identyfikator przypisany użytkownikowi, służący do logowania do systemu.

### Adres e-mail  
- Elektroniczny adres poczty, wykorzystywany do kontaktu z użytkownikiem oraz do potwierdzenia rejestracji.

### Hasło  
- Sekretny ciąg znaków służący do weryfikacji tożsamości użytkownika.

### Powtórz hasło  
- Pole do wprowadzenia hasła w celu potwierdzenia poprawności jego wpisu.

### Kod potwierdzający  
- Tymczasowy kod wysyłany na adres e-mail użytkownika, służący do potwierdzenia tożsamości podczas rejestracji.
