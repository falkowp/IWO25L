# PU005: Logowanie w systemie

#### Autor: Bartosz Cylwik

## 1. Cel przypadku użycia  
Użytkownik może zalogować się do systemu, aby uzyskać dostęp do jego funkcji.

## 2. Aktorzy  
- Użytkownik

## 3. Przebieg główny  
1. Użytkownik wybiera opcję „Zaloguj się” w interfejsie systemu.  
2. System wyświetla formularz rejestracji nowego użytkownika, zawierający pola:  
   - Nazwa użytkownika / adres e-mail  
   - Hasło  
   - Autoryzacja przez oauth (google etc.)  
3. Użytkownik wprowadza dane do logowania.  
4. Użytkownik zatwierdza formularz.  
5. System sprawdza poprawność danych logowania.  
6. System uwierzytelnia użytkownika.  
7. System przekierowuje użytkownika do jego panelu głównego.

## 4. Przebiegi alternatywne  

### 4.1. Niepoprawne dane logowania  
1. System wykrywa nieprawidłową nazwę użytkownika lub hasło.
2. System wyświetla komunikat o błędzie logowania.
3. Użytkownik może ponownie spróbować się zalogować (powrót do kroku 3).  

### 4.2. Konto nieaktywne / niepotwierdzone  
1. System informuje użytkownika, że konto nie zostało aktywowane.
2. System wyświetla informację o konieczności potwierdzenia konta (np. poprzez link w e-mailu).  

### 4.3. Zbyt wiele nieudanych prób logowania  
1. Po kilku nieudanych próbach logowania system tymczasowo blokuje możliwość logowania dla danego konta lub IP.
2. System wyświetla komunikat o blokadzie i informuje o czasie jej trwania.

### 4.4. Użytkownik rezygnuje z logowania  
1. Użytkownik wciska przycisk „Anuluj” lub zamyka formularz logowania.
2. System powraca do ekranu głównego lub poprzedniego widoku.

## 5. Warunki początkowe  
- Użytkownik nie jest zalogowany i znajduje się na stronie logowania.

## 6. Warunki końcowe  
- **Sukces:** Użytkownik został pomyślnie uwierzytelniony i ma dostęp do systemu..  
- **Porażka:** Użytkownik nie uzyskał dostępu do systemu z powodu nieprawidłowych danych lub rezygnacji. 

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Wyjątki  

- **Błąd uwierzytelnienia:**  
  - System odrzuca dane logowania i informuje użytkownika o błędzie..

- **Błąd techniczny (np. serwer nie odpowiada):**  
  - System informuje użytkownika o problemie i sugeruje ponowienie próby później.

## 9. Słownik pojęć  

### Użytkownik  
- Osoba fizyczna lub podmiot, który korzysta z systemu i loguje się w celu uzyskania dostępu do jego funkcji.

### Nazwa użytkownika / adres e-mail  
- Identyfikator używany przy logowaniu.

### Hasło  
- Sekretny ciąg znaków zabezpieczający dostęp do konta.

### Formularz logowania  
- Interfejs do wprowadzenia danych logowania.

### Panel użytkownika  
- Strona dostępna po zalogowaniu, zawierająca funkcje systemu.
