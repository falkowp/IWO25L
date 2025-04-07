# PU012: Eksport listy metadanych do pliku

#### Autor: Maciej Przybylski

## 1. Cel przypadku użycia
Umożliwić administratorowi systemu zapis listy metadanych do pliku, co pozwala na dalszą analizę danych przez zespół oraz wykorzystanie ich w raportach i integracjach z innymi narzędziami analitycznymi.

## 2. Aktorzy
- Administrator  
- Użytkownik (w zakresie odczytu niektórych metadanych, jeżeli dostęp do pliku ma być również udostępniony innym rolom)  
- Organizacja (w kontekście danych organizacyjnych, które mogą być eksportowane w raportach)

## 3. Przebieg główny
1. Administrator loguje się do systemu.
2. Na głównym pulpicie lub w dedykowanym module "Zarządzanie metadanymi" wybiera opcję "Eksport listy metadanych".
3. System wyświetla ekran umożliwiający wybór kryteriów eksportu, takich jak:
   - Zakres danych (np. określony czas, kategorie metadanych)
   - Format pliku (CSV, JSON, XML)
   - Dodatkowe filtry (np. metadane związane z określoną funkcjonalnością lub modułem)
4. Administrator ustala preferencje eksportu i zatwierdza wybór.
5. System przetwarza zapytanie i generuje plik eksportu, prezentując użytkownikowi podgląd (opcjonalnie) lub informację o gotowym pliku.
6. Administrator pobiera plik i może udostępnić go do dalszej analizy np. w zewnętrznych narzędziach raportowych.
7. System loguje operację eksportu dla celów audytu.

## 4. Przebiegi alternatywne

### 4.1. Brak danych do eksportu
1. Jeśli w systemie nie znajduje się żaden rekord metadanych spełniający ustawione kryteria, system wyświetla komunikat: "Brak metadanych do eksportu".
2. Administrator może zmodyfikować kryteria wyszukiwania lub anulować operację.

### 4.2. Błąd generowania pliku
1. W przypadku wystąpienia błędu podczas generowania pliku eksportu (np. problemy z serwerem, błędna konfiguracja formatu), system wyświetla komunikat: "Wystąpił błąd podczas tworzenia pliku. Proszę spróbować ponownie później.".
2. System rejestruje szczegóły błędu dla administratora systemu, a administrator ma możliwość kontaktu z działem wsparcia technicznego.

### 4.3. Błąd dostępu lub brak uprawnień
1. Jeżeli użytkownik (lub administrator posiadający niepełne uprawnienia) próbuje wykonać eksport bez odpowiednich uprawnień, system wyświetla komunikat: "Brak uprawnień do eksportu metadanych".
2. Operacja eksportu jest anulowana, a administrator zostaje przekierowany na stronę zarządzania uprawnieniami lub pomoc techniczną.

## 5. Warunki początkowe
- Administrator jest zalogowany do systemu.
- Istnieją metadane w systemie, które mogą być eksportowane.
- Administrator posiada niezbędne uprawnienia do wykonywania operacji eksportu.

## 6. Warunki końcowe
- Plik z listą metadanych został pomyślnie wygenerowany i zapisany.
- Administrator otrzymuje plik eksportu, który następnie może być wykorzystany do dalszej analizy lub raportowania.
- Operacja eksportu jest zarejestrowana w logach systemowych.

## 7. Wymagania specjalne
- System powinien umożliwiać wybór różnych formatów plików (CSV, JSON, XML) tak, aby plik eksportu był kompatybilny z popularnymi narzędziami analitycznymi.
- Eksport danych musi być realizowany zgodnie z obowiązującymi zasadami bezpieczeństwa i ochrony danych.
- Plik wynikowy powinien zawierać aktualne nagłówki kolumn i dane zgodne z wybranymi kryteriami.
- Proces generowania pliku nie powinien znacząco obciążać systemu ani wpływać na działanie innych usług.

## 8. Rozszerzenia
- Wyświetlenie listy metadanych (PU011)

## 9. Słownik pojęć dla PU012

### Metadane
- **Definicja**: Dane opisujące charakterystykę i właściwości innych danych zapisanych w systemie.
- **Synonim**: Dane opisowe, dane dodatkowe
- **Użycie**: Metadane pomagają w identyfikacji, klasyfikacji i przeszukiwaniu zasobów systemowych.

### Eksport
- **Definicja**: Proces zapisywania danych (w tym przypadku metadanych) do pliku w celu ich późniejszej analizy lub przeniesienia.
- **Synonim**: Zapisywanie, wywóz danych
- **Użycie**: Eksport umożliwia administratorowi pobranie bieżących informacji zawartych w systemie.

### Plik
- **Definicja**: Zbiór danych zapisany w określonym formacie (np. CSV, JSON, XML), który może być odczytany przez różne aplikacje.
- **Synonim**: Dokument, zestawienie danych
- **Użycie**: Plik eksportu zawiera uporządkowany zbiór metadanych gotowy do analizy.

### Administrator
- **Definicja**: Osoba zarządzająca systemem informatycznym, posiadająca rozszerzone uprawnienia do konfiguracji, monitorowania i wykonywania operacji administracyjnych.
- **Synonim**: Admin, Kierownik systemu
- **Użycie**: Administrator wykonuje operację eksportu, aby pobrać dane niezbędne do dalszych analiz i raportowania.

### Format pliku
- **Definicja**: Określony układ i struktura danych w pliku, umożliwiająca ich prawidłowe przetwarzanie przez programy.
- **Wartości przykładowe**: CSV, JSON, XML
- **Użycie**: Wybór odpowiedniego formatu zapewnia kompatybilność z narzędziami do analizy danych.
