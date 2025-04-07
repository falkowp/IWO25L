# PU002: Przypisanie uprawnień/roli użytkownikowi do źródła danych

#### Autor: Michał Janaszewski

## 1. Cel: 
Administrator może przypisywać użytkownikom role i uprawnienia do różnych zasobów.

## 2. Aktorzy
- Administrator systemu

## 3. Przebieg główny
1. Administrator wybierą opcję "Przypisanie roli użytkownikowi" przy odpowienim użytkowniku
2. Administrator wybierą rolę i potwierdza jest wybranie

## 4. Przebiegi alternatywne

### 4.1. Administrator rezygnuje z przypisania roli
1. Administrator otwiera formularz przypisania roli, ale zamyka go bez zapisania zmian
2. System anuluje operację i wraca do listy użytkowników
3. Administrator może wybrać innego użytkownika lub zakończyć pracę

## 5. Warunki początkowe
- Administrator jest zalogowany do systemu
- Administroator wyświetlił listę użytkowników

## 6. Warunki końcowe
- Lista użytkowników została wyświetlona
- Administrator może wykonać dodatkowe operacje na wyświetlonej liście (np. nadanie hasła, przypisanie uprawnień, usunięcie konta)

## 7. Wymagania specjalne
- Lista użytkowników nie może być pusta

## 8. Rozszerzenia
- Zmiana uprawnień (PU003)

## 9. Słownik pojęć dla PU0001

### Administrator systemu
- **Definicja**: Osoba uprawniona do zarządzania użytkownikami i ich uprawnieniami w systemie
- **Synonim**: Admin, Administrator

### Uprawnienia
- **Definicja**: Zbiór praw i możliwości przypisanych do konta użytkownika
- **Synonim**: Prawa dostępu, Role
- **Użycie**: Uprawnienia określają zakres działań, jakie użytkownik może wykonywać w systemie
