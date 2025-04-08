# PU019: Wyświetlenie informacji o źródle danych

#### Autor: Adrian Rybaczuk

## 1. Cel przypadku użycia
Umożliwienie użytkownikowi systemu przeglądania szczegółowych informacji o wybranym źródle danych w celu zapoznania się z jego charakterystyką i metadanymi.

## 2. Aktorzy
- Użytkownik systemu
- Administrator systemu

## 3. Przebieg główny
1. Użytkownik loguje się do systemu
2. Użytkownik wybiera opcję "Źródła danych"
3. Użytkownik wybiera konkretne źródło danych z listy
4. System wyświetla szczegółowe informacje o źródle danych zawierające:
   - Podstawowe dane źródła (nazwa, opis, typ)
   - Metadane techniczne
   - Informacje o właścicielu i administratorze
   - Status i historię zmian
   - Powiązane zasoby i zależności
   - Statystyki wykorzystania
   - Dokumentację i dodatkowe materiały

## 4. Przebiegi alternatywne

### 4.1. Brak dostępu do źródła danych
1. System wyświetla komunikat "Brak uprawnień do przeglądania informacji o źródle danych"
2. Przypadek użycia kończy się niepowodzeniem

### 4.2. Źródło danych nie istnieje
1. System wyświetla komunikat "Wybrane źródło danych nie istnieje"
2. Użytkownik zostaje przekierowany do listy źródeł danych

## 5. Warunki początkowe
- Użytkownik jest zalogowany do systemu
- Użytkownik posiada odpowiednie uprawnienia do przeglądania informacji o źródle danych
- Źródło danych istnieje w systemie

## 6. Warunki końcowe
- Szczegółowe informacje o źródle danych zostały wyświetlone
- Użytkownik może wykonać dodatkowe operacje na wyświetlonych informacjach (np. eksport metadanych, zgłoszenie problemu)

## 7. Wymagania specjalne
- Informacje powinny być prezentowane w przejrzysty i czytelny sposób
- System powinien umożliwiać eksport wyświetlonych informacji
- Dostęp do wrażliwych informacji powinien być ograniczony zgodnie z uprawnieniami użytkownika

## 8. Rozszerzenia
- Eksport listy metadanych do pliku (PU012)
- Zgłaszanie błędów i problemów z metadanymi (PU037)
- Wyświetlenie listy metadanych (PU011)

## 9. Słownik pojęć dla PU019

### Źródło danych
- **Definicja**: Zbiór danych, usługa dostarczająca dane lub API (Application Programming Interface) udostępniające dane do systemu
- **Synonim**: Zasób danych, Baza danych, Interfejs API
- **Użycie**: Źródło danych jest głównym obiektem, którego informacje są wyświetlane

### Metadane
- **Definicja**: Dane opisujące charakterystykę i właściwości źródła danych
- **Synonim**: Dane opisowe, Informacje o danych
- **Użycie**: Metadane zawierają szczegółowe informacje o źródle danych

### Status źródła danych
- **Definicja**: Informacja o aktualnym stanie źródła danych w systemie
- **Wartości**: aktywne, nieaktywne, w konserwacji
- **Użycie**: Status określa dostępność i stan źródła danych

### Właściciel źródła danych
- **Definicja**: Osoba lub jednostka odpowiedzialna za źródło danych
- **Synonim**: Administrator źródła, Opiekun
- **Użycie**: Właściciel jest odpowiedzialny za zarządzanie źródłem danych

### Dokumentacja źródła
- **Definicja**: Zbiór dokumentów opisujących źródło danych
- **Synonim**: Dokumenty źródła, Materiały źródłowe
- **Użycie**: Dokumentacja zawiera szczegółowe informacje o strukturze i wykorzystaniu źródła danych
