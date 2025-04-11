# PU014: Dodanie nowego zestawu metadanych

#### Na podstawie: Mikołaj Pątkowski
#### Poprawił: Artem Omelchenko

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014

PRE: Administrator jest zalogowany do systemu oraz posiada uprawnienia do dodawania zestawów metadanych. W systemie istnieją zarejestrowane metadane, które można włączyć do zestawu

1. Administrator wybiera opcję "Dodaj nowy zestaw metadanych" w interfejsie systemu
3. System wyświetla formularz dodawania nowego zestawu metadanych
5. Administrator wprowadza wymagane informacje oraz zaznacza metadane, które mają zostać włączone do zestawu
[WSZYSTKIE OBOWIĄZKOWE POLA SĄ UZUPEŁNIONE]
7. Administrator zatwierdza formularz przyciskiem "Zapisz"
9. System weryfikuje poprawność danych
[DANE POPRAWNE]
11. System zapisuje nowy zestaw metadanych w bazie danych
13. System wyświetla potwierdzenie pomyślnego dodania nowego zestawu metadanych

FINAL: success\
POST: Nowy zestaw metadanych został pomyślnie dodany do systemu oraz jest widoczny dla użytkowników

## 2. Przebiegi alternatywne

### 2.1. SCENARIUSZ ALTERNATYWNY PU0014-1 'Niekompletne dane'
1.-3. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014\
4a. System wykrywa brakujące obowiązkowe pola zestawu metadanych\
[OBOWIĄZKOWE POLA SĄ NIE UZUPEŁNIONE]\
5a. System wyświetla komunikat o błędzie wskazujący brakujące pola\
6a. System blokuje zatwierdzenie formularza do czasu uzupełnienia danych\
7a. Administrator uzupełnia brakujące dane\
4.-7. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014

### 2.2. SCENARIUSZ ALTERNATYWNY PU0014-2 'Duplikat nazwy zestawu'
1.-5. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014\
[DANE NIE POPRAWNE]\
6b. System wykrywa, że zestaw metadanych o podanej nazwie już istnieje w systemie\
7b. System wyświetla komunikat o błędzie informujący o konflikcie nazw\
8b. Administrator zmienia nazwę zestawu\
4.-7. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014

### 2.3. SCENARIUSZ ALTERNATYWNY PU0014-3 'Administrator anuluje operację'
1.-3. tak jak w SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU014\
4c. Administrator wybiera opcję "Anuluj" przed zatwierdzeniem formularza\
5c. System zamyka formularz dodawania bez zapisywania wprowadzonych danych

FINAL: failure\
POST: Nowy zestaw metadanych nie był utworzony oraz dodany

# 3. SŁOWNIK POJĘĆ

### Zestaw metadanych

- **Definicja**: Uporządkowana kolekcja powiązanych ze sobą metadanych tworzących logiczną całość, służąca do opisu określonego typu zasobu lub kategorii danych
- **Atrybuty**: 
    - Nazwa: tekst
    - Opis: tekst
    - Data utworzenia: data
    - List<Metadane>

### Metadane  
- **Definicja**: Dane na temat źródła danych.  
- **Atrybuty**: 
  - ID: liczba
  - Nazwa: tekst
  - Opis: tekst
  - Właściciel: tekst
  - Data utworzenia: data
  - Data aktualizacji: data
  - status: enum
  - czy_zarchiwizowane: bool
