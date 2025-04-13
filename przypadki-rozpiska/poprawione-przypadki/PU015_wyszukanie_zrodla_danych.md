# PU015: Wyszukanie źródła danych

#### Autor: Mateusz Tyl

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU015

PRE: Użytkownik jest zalogowany w systemie

1. Użytkownik podaje filtr
2. << invoke >> [Walidacja filtru] \
[filtr poprawny] 
3. Użytkownik wybiera opcję "Szukaj"
4. System wyszukuje metadane
5. << invoke >> [Pobranie metadanych] \
[dane pobrane pomyślnie] 
6. System wyświetla pobrane metadane

POST: Użytkownik uzyskuje informacje o wyszukanych metadanych na podstawie wybranego przez siebie filtru. Może archiwizować, sprawdzać poprawność, usuwać, wyświetlać informacje o metadanych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Użytkownik zresetował filtr  

1-2 Tak samo, jak w SCENARIUSZU GŁÓWNYM \
[Użytkownik resetuje filtr] \
3. System wyświetla komunikat o zresetowaniu filtru \
Powrót do zadania 1 w SCENARIUSZU GŁÓWNYM

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Nastąpił błąd podczas pobierania metadanych  

1-4 Tak samo, jak w SCENARIUSZU GŁÓWNYM \
[błąd podczas pobierania metadanych] \
5. System wyświetla komunikat o błędzie
6. System powraca do listy metadanych \
FINAL: Failure \
POST: Użytkownik nie uzyskuje żądanych informacji o metadanych

## 3. SŁOWNIK POJĘĆ

### Użytkownik  
- **Definicja**: Osoba korzystająca z systemu
- **Atrybuty**: 
  - ID: liczba
  - imie: tekst
  - nazwisko: tekst
  - email: tekst
  - login: tekst
  - hasło: tekst
  - rola: enum
  - uprawnienia: enum
### Metadane 
- **Definicja**: Dane na temat źródła danych
- **Atrybuty**: 
  - ID: liczba
  - nazwa: tekst
  - opis: tekst
  - właściciel: tekst
  - data_utworzenia: data
  - data_aktualizacji: data
  - status: enum
  - czy_zarchiwizowane: bool
### Filtr 
- **Definicja**: Kryteria na podstawie których można wyszukiwać metadane
- **Atrybuty**: 
  - lista_kryteriów: lista
