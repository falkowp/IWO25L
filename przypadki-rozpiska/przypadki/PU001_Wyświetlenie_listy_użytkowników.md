# PU0001: Wyświetlenie listy użytkowników

#### Autor: Marta Stankevich

## 1. Cel przypadku użycia
Umożliwienie administratorowi systemu przeglądania listy wszystkich użytkowników w systemie w celu zarządzania dostępem i uprawnieniami.

## 2. Aktorzy
- Administrator systemu

## 3. Przebieg główny
1. Administrator loguje się do systemu
2. Administrator wybiera opcję "Zarządzanie użytkownikami"
3. System wyświetla listę wszystkich użytkowników zawierającą:
   - Identyfikator użytkownika
   - Imię i nazwisko
   - Adres email
   - Status konta (aktywne/nieaktywne)
   - Data utworzenia konta
   - Ostatnie logowanie
   - Przypisane role i uprawnienia

## 4. Przebiegi alternatywne

### 4.1. Brak użytkowników w systemie
1. System wyświetla komunikat "Brak zarejestrowanych użytkowników"
2. Administrator może utworzyć nowe konto użytkownika (PU009)

### 4.2. Błąd dostępu
1. System wyświetla komunikat "Brak uprawnień do przeglądania listy użytkowników"
2. Przypadek użycia kończy się niepowodzeniem

## 5. Warunki początkowe
- Administrator jest zalogowany do systemu
- Administrator posiada odpowiednie uprawnienia do przeglądania listy użytkowników

## 6. Warunki końcowe
- Lista użytkowników została wyświetlona
- Administrator może wykonać dodatkowe operacje na wyświetlonej liście (np. nadanie hasła, przypisanie uprawnień, usunięcie konta)

## 7. Wymagania specjalne
- Lista użytkowników powinna być sortowalna według różnych kryteriów
- System powinien umożliwiać filtrowanie listy użytkowników
- Dane wrażliwe użytkowników (np. hasła) nie powinny być wyświetlane

## 8. Rozszerzenia
- Przypisanie uprawnień/roli użytkownikowi do metadanych (PU002)
- Nadanie hasła (PU006)
- Usunięcie konta (PU008)
- Utworzenie konta (PU009)

## 9. Słownik pojęć dla PU0001

### Administrator systemu
- **Definicja**: Osoba uprawniona do zarządzania użytkownikami i ich uprawnieniami w systemie
- **Synonim**: Admin, Administrator
- **Użycie**: Administrator może przeglądać listę użytkowników i zarządzać ich uprawnieniami

### Użytkownik systemu
- **Definicja**: Osoba posiadająca konto w systemie
- **Synonim**: Użytkownik, Konto użytkownika
- **Użycie**: Użytkownik systemu może być wyświetlony na liście użytkowników

### Konto użytkownika
- **Definicja**: Zbiór danych identyfikujących użytkownika w systemie wraz z jego uprawnieniami
- **Synonim**: Konto, Profil użytkownika
- **Użycie**: Każde konto użytkownika zawiera podstawowe informacje identyfikacyjne i uprawnienia

### Status konta
- **Definicja**: Informacja o aktualnym stanie konta użytkownika w systemie
- **Wartości**: aktywne, nieaktywne
- **Użycie**: Status konta określa, czy użytkownik może korzystać z systemu

### Uprawnienia
- **Definicja**: Zbiór praw i możliwości przypisanych do konta użytkownika
- **Synonim**: Prawa dostępu, Role
- **Użycie**: Uprawnienia określają zakres działań, jakie użytkownik może wykonywać w systemie

### Lista użytkowników
- **Definicja**: Zbiór wszystkich kont użytkowników w systemie wraz z ich podstawowymi informacjami
- **Synonim**: Rejestr użytkowników, Spis użytkowników
- **Użycie**: Lista użytkowników jest głównym elementem interfejsu zarządzania użytkownikami

### Identyfikator użytkownika
- **Definicja**: Unikalny kod identyfikujący użytkownika w systemie
- **Synonim**: ID użytkownika, Login
- **Użycie**: Identyfikator użytkownika jest używany do jednoznacznego rozpoznawania użytkownika w systemie
