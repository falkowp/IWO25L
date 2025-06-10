# PU032: Wyświetlenie listy zarchizowanych raportów

#### Autor: [Nie podano w tekście]

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU032

PRE: Administrator jest zalogowany do systemu z odpowiednią rolą

1. Administrator wybrał "Przeglądaj raporty"
2. System pobiera dane raportów
3. System pobierał dane raportów poprawnie
4. System wyświetla okno listy raportów

FINAL: Success
POST: Dane raportów zostały wyświetlone

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Brak raportów w systemie

1.-2. Tak samo, jak w SCENARIUSZU GŁÓWNYM
    [ Brak raportów ]
3a. System pobrał pustą listę raportów
4. System wyświetla informację "Brak raportów"

FINAL: Success
POST: Brak raportów był spowodowany brakiem danych userowi

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - System zwraca błąd podczas pobierania danych

1.-2. Tak samo, jak w scenariuszu głównym
    [ Wystapil blad ]
3. System zwraca błąd 
4. System wyświetla informację "Wystapil blad podczas dostepu do danych"

FINAL: Fail
Post: System nie zwrócił danych przez blad

## 3. SŁOWNIK POJĘĆ

### Raport o
* **Definicja**: raport dot. zgłoszeń zawiera informacje statystyczne na temat zgłoszeń w
systemie

### Okno listy raportów
* **Definicja**: Okno w systemie przedstawiające nam listę raportów dostępnych w systemie

### Lista raportów
* **Definicja**: lista zbiór raportów w systemie
