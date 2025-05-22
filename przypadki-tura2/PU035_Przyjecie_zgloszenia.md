# **PU0035: Przyjęcie zgłoszenia użytkownika**

#### Autor: Patrycja Falkowska

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Użytkownik jest zalogowany do systemu i posiada uprawnienia administratora.

1. Administrator wybiera opcję „Zgłoszenia użytkowników”.
   \[ DANE POPRAWNE ]
2. System wyświetla listę oczekujących zgłoszeń.
3. Administrator wybiera konkretne zgłoszenie.
4. System wyświetla szczegóły zgłoszenia.
5. Administrator wybiera opcję „Akceptuj”.
6. System zapisuje decyzję i zmienia status zgłoszenia.

**POST:** Zgłoszenie zostało rozpatrzone i zarejestrowano decyzję administratora.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Brak zgłoszeń

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
   \[ DANE NIEPOPRAWNE ]
2. a. System wyświetla komunikat o braku zgłoszeń.
3. a. Administrator wybiera opcję "OK".
4. a. System wyświetla ponownie ekran główny.

**POST:** Administrator nie zapoznał się ze zgłoszeniem.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Zgłoszenie rozpatrzone przez innego administratora

1. Tak samo, jak w SCENARIUSZU GŁÓWNYM
   \[ DANE NIEPOPRAWNE ]
2. a. System wyświetla komunikat o rozpatrzeniu zgłoszenia przez innego administratora.
3. a. Administrator wybiera opcję "OK".
4. a. System wyświetla ponownie ekran główny.

**POST:** Administrator nie zapoznał się ze zgłoszeniem.

## 3. SŁOWNIK POJĘĆ

### Zgłoszenie użytkownika

* **Definicja**: Prośba, pytanie lub problem zgłoszony przez użytkownika do administratora.

- **Atrybuty**:  
  - ID: numer  
  - ID użytkownika: numer
  - Treść: tekst
  - Status: tekst
  - Data złożenia: data

