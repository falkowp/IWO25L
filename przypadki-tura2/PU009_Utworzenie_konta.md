# **PU009: Utworzenie konta**

#### Autor: Mateusz Tyl 325520

## 1. SCENARIUSZ GŁÓWNY

**PRE:** Administrator jest zalogowany do systemu.

1. Administrator klika przycisk „Utwórz konto użytkownika”.
2. System wyświetla formularz „Utwórz konto użytkownika”.
3. Administrator wypełnia dane użytkownika.
4. Administrator klika przycisk „Generuj hasło”.
5. System wyświetla wygenerowane hasło w formularzu „Utwórz konto użytkownika”.
6. Administrator wybiera uprawnienia użytkownika w formularzu.
7. Administrator klika przycisk „Zapisz konto”.
8. < invoke >Wysłanie użytkownikowi powiadomienia o założeniu konta oraz danych do logowania
9. System wyświetla komunikat potwierdzający założenie konta.

**POST:** Konto użytkownika zostało utworzone z odpowiednimi uprawnieniami i użytkownik może się zalogować.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Adres e-mail już istnieje

1. Kroki 1–7 jak w SCENARIUSZU GŁÓWNYM  
   \[ DANE NIEPOPRAWNE – e-mail istnieje ]
2. a. System wyświetla komunikat „Użytkownik o takim adresie e-mail już istnieje”.
3. a. Administrator klika przycisk „Zamknij formularz”.
4. a. System zamyka formularz.

**POST:** Konto nie zostało utworzone.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Niepoprawny dobór uprawnień

1. Kroki 1–7 jak w SCENARIUSZU GŁÓWNYM  
   \[ DANE NIEPOPRAWNE – kolidujące/niekompatybilne uprawnienia ]
2. a. System wyświetla komunikat o niepoprawnym doborze uprawnień.
3. a. Administrator koryguje zestaw uprawnień w formularzu.
4. a. Administrator klika ponownie przycisk „Zapisz konto”.
5. a. < invoke >Wysłanie użytkownikowi powiadomienia o założeniu konta oraz danych do logowania
6. a. System wyświetla komunikat potwierdzający założenie konta.

**POST:** Konto zostało utworzone po poprawnym doborze uprawnień i użytkownik otrzymał dane do logowania.

## 3. SŁOWNIK POJĘĆ

### Administrator  
**Definicja:** Użytkownik systemu posiadający uprawnienia do tworzenia i zarządzania kontami.

### Formularz „Utwórz konto użytkownika”  
**Definicja:** Formularz, w którym Administrator podaje dane użytkownika (e-mail, imię, nazwisko), generuje hasło i wybiera uprawnienia.

### Dane użytkownika  
**Definicja:** Zbiór informacji o użytkowniku, składający się z e-maila, imienia i nazwiska.

### Uprawnienie  
**Definicja:** Pojedyncza rola lub zestaw czynności, które użytkownik może wykonać w systemie.
