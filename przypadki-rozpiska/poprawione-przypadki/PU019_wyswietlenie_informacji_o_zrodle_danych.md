# PU019: Wyświetlenie informacji o źródle danych

#### Autor: Maciej Przybylski

## 1. SCENARIUSZ GŁÓWNY

#### PRE:

- Użytkownik jest zalogowany do systemu
- Użytkownik posiada odpowiednie uprawnienia do przeglądania informacji o źródle danych
- Źródło danych istnieje w systemie

1. Użytkownik wybiera opcję "Źródło danych"
2. Użytkownik wybiera pozycję z listy
3. System wyświetla szczegółowe informacje o źródle danych

#### POST: Szczegółowe informacje o źródle danych zostały wyświetlone

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1

1. i 2. Tak samo jak w SCENARIUSZU GŁÓWNYM
   
[brak połączenia z internetem]

3. a. System wyświetla informację o braku połączenia z internetem

#### POST: Informacja o braku połączenia zostaje wyświetlona

### 2.2. SCENARIUSZ ALTERNATYWNY 2

1. i 2. Tak samo jak w SCENARIUSZU GŁÓWNYM
   
[kończy się sesja użytkownika]

3. b. System wyświetla informację o wylogowaniu
4. b. System wyświetla formularz logowania

#### POST: Formularz do logowania zostaje wyświetlony

### 2.3. SCENARIUSZ ALTERNATYWNY 3

1. Tak samo jak w SCENARIUSZU GŁÓWNYM
   
[przeglądarka nie obsługuje wyświetlenia listy źródeł danych]

3. c. System wyświetla informację o niewspieranej przeglądarce

#### POST: Informacja o braku wspieranej przeglądarki zostaje wyświetlona


## 3. SŁOWNIK

### Źródło danych  
- **Definicja**: Zbiór danych, usługa dostarczająca dane, bądź API (Application Programming Interface) udostęniające dane do systemu
- **Atrybuty**: 
  - Nazwa: tekst
  - Usługa: tekst

### Metadane
- **Definicja**: Dane opisujące charakterystykę i właściwości źródla danych
- **Atrybuty**: 
  - Id: numer
  - Nazwa: string
  - Opis: string
  - Właściciel: string
  - Data utworzenia: data
  - Data aktualizacji: data
  - Status: enum
  - Czy zarchiwizowane: bool

### Status źródła danych
- **Definicja**: Informacja o aktualnym stanie źródła danych w systemie
- **Atrybuty**: 
  - Wartość: enum
    - Możliwe wartości: aktywne, nieaktywne, w aktualizacji 

### Właściciel źródła danych
- **Definicja**: Osoba lub jednostka odpowiedzialna za źródło danych
- **Atrybuty**: 
  - Imię: tekst
  - Nazwisko: tekst
  - Organizacja: tekst
 
### Dokumentacja źródła danych
- **Definicja**: Zbiór dokumentów opisująca źródło danych
- **Atrybuty**: 
  - Dokumentacja: tekst
 
### Szczegółowe informacje o źródle danych
- **Definicja**: Podstawowe informacje o źródle
- **Atrybuty**: 
  - Nazwa: tekst
  - Opis: tekst
  - Typ: tekst
  - Metadane: metadane
  - Status: Status źródła danych
  - Historia zmian: tablica tekstów
  - Powiązane zasoby: tablica identyfikatorów
  - Statystyki wykorzystania: tekst
  - Dokumentacja: Dokumentacja
