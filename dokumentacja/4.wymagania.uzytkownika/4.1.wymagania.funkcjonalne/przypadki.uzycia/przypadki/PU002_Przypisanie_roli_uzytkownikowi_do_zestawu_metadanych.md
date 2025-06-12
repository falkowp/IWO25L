# PU002: Przypisanie roli uzytkownikowi do zestawu metadanych

#### Autor: Wojciech Grot

## 1. SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU002

PRE: 
- Administrator jest zalogowany do systemu.
- Administrator wybrał z listy użytkownika którego rolę chce edytować,
- Administrator wybrał z listy zestaw matadanych do którego rolę ww. użytkownika będzie zmieniał.
-  Na ekranie wyświetla się okno z listą dostępnych ról

1. Administrator wybiera role na liście
2. Administrator klika przycisk "zapisz"
3. System zapisuje zmiany w bazie danych
4. System zamyka okno z listą dostępnych ról
5. System wyświetla komunikat o zapisaniu zmian

FINAL: success\
POST: Użytkownik ma przypisaną nową rolę do wybranego zestawu metadanych

## 2. Przebiegi alternatywne

### 2.1. SCENARIUSZ ALTERNATYWNY 1 - Anulowanie opercji
1 Administrator wybiera role na liście
2a Admiistrator klika przycisk "anuluj"
3a System zamyka okno z listą dostępnych ról
4a System wyświetla komunikat o odrzuceniu zmian

FINAL: failure\
POST: Użytkownik nie ma przypisanej nowej roli do wybranego zestawu metadanych

### 2.2. SCENARIUSZ ALTERNATYWNY 2 - Bład zapisu
1-2 Tak jak w "SCENARIUSZ GŁÓWNY PRZYPADKU UŻYCIA PU002"
3b System natrafia na błąd w podczas zapisu w bazie danych
3a System zamyka okno z listą dostępnych ról
4 System zamyka okno z listą dostępnych ról
5b System wyświetla komunikat o błedzie podczas zapisu

FINAL: failure\
POST: Użytkownik nie ma przypisanej nowej roli do wybranego zestawu metadanych

## 3. SŁOWNIK POJĘĆ

### Rola użytkownika

- **Definicja**: Enum opisujący wszystkie dostępne role dla użytkowników systemu
- **Atrybuty**:
    - Rola: Enum

### Okno z listą dostępnych ról

- **Definicja**: Okno wyświetlające dostępne role w systemie w formie listy

### Zestaw metadanych

- **Definicja**: Uporządkowana kolekcja powiązanych ze sobą metadanych tworzących logiczną całość, służąca do opisu określonego typu zasobu lub kategorii danych
- **Atrybuty**: 
    - Nazwa: tekst
    - Opis: tekst
    - Data utworzenia: data
    - List(Metadane)

### Lista użytkowników
- **Definicja**: Lista zawierająca
informacje o użytkownikach systemu

### Okno listy użytkowników
- **Definicja**: Okno wyświetlające dane z "listy użytkowników"
- **Atrybuty**:
    - List (Użytkownik)


### Lista zestawów metadanych
- **Definicja**: Lista zawierająca
informacje o zestawach metadanych

### Okno listy zestawów metadanych
- **Definicja**: Okno wyświetlające dane z "listy metadnaych"
- **Atrybuty**:
    - List (Metadane)


