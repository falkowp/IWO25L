# PU037: Zgłaszanie błędów i problemów z metadanymi

#### Autor: Artem Omelchenko

## 1. Cel przypadku użycia  
Użytkownik może zgłosić błędy dotyczące wybranych metadanych.

## 2. Aktorzy  
- Użytkownik

## 3. Przebieg główny  
1. Użytkownik znajduje się na stronie szczegółów metadanych (PU019)
2. Użytkownik naciska przycisk „Zgłoś problem” przy wybranych metadanych.  
3. System wyświetla formularz zgłoszenia zawierający:  
   - Pole opisu problemu  
   - Kategorię problemu (np. błędne dane, nieaktualne informacje, problemy techniczne)  
   - Możliwość dodania załącznika (np. zrzut ekranu)  
4. Użytkownik wypełnia formularz zgłoszenia.  
5. Użytkownik zatwierdza zgłoszenie przyciskiem „Wyślij”.  
6. System waliduje wprowadzone dane.  
7. System zapisuje zgłoszenie i przypisuje mu unikalny identyfikator.  
8. System wyświetla potwierdzenie przyjęcia zgłoszenia.

## 4. Przebiegi alternatywne  

### 4.1. Błędy walidacji formularza  
1. System wykrywa błędy we wprowadzonych danych.  
2. System wyświetla komunikaty o błędach (np. puste pole opisu).  
3. Użytkownik poprawia dane i ponownie wysyła zgłoszenie (powrót do kroku 5 przebiegu głównego).

## 5. Warunki początkowe  
- Użytkownik jest zalogowany do systemu.  
- Użytkownik przegląda szczegóły konkretnego zestawu metadanych.

## 6. Warunki końcowe  
- Zgłoszenie zostało poprawnie zapisane w systemie.  
- Użytkownik otrzymał potwierdzenie przyjęcia zgłoszenia.  
- Administrator został powiadomiony o nowym zgłoszeniu.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Wyjątki  
- **Błąd walidacji danych**  
  - System informuje o nieprawidłowych lub brakujących danych i uniemożliwia wysłanie formularza do momentu ich poprawienia.  

- **Błąd zapisu do bazy danych**  
  - System informuje użytkownika o problemie z zapisaniem zgłoszenia (np. problemy z serwerem) i sugeruje ponowną próbę.

## 9. Słownik pojęć  

### Metadane  
- Dane opisujące inne dane, zawierające informacje o ich strukturze, pochodzeniu i sposobie wykorzystania.  

### Zgłoszenie  
- Wpis zawierający informacje o zaobserwowanym problemie, potrzebie lub incydencie zgłoszonym przez użytkownika.  
