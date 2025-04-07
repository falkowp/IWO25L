# PU014: Dodanie nowego zestawu metadanych

#### Autor: Mikołaj Pątkowski

## 1. Cel przypadku użycia

Umożliwienie administratorowi systemu dodania nowego zestawu metadanych po uprzedniej rejestracji metadanych w systemie.

## 2. Aktorzy

- Administrator systemu

## 3. Przebieg główny

1. Administrator wybiera opcję "Dodaj nowy zestaw metadanych" w interfejsie systemu
2. System wyświetla formularz dodawania nowego zestawu metadanych, zawierający pola:
    - Nazwa zestawu
    - Opis zestawu
    - Data utworzenia
    - Lista dostępnych metadanych do włączenia w zestaw
3. Administrator wprowadza wymagane informacje oraz zaznacza metadane, które mają zostać włączone do zestawu
4. Administrator zatwierdza formularz przyciskiem "Zapisz"
5. System weryfikuje poprawność i kompletność wprowadzonych danych
6. System zapisuje nowy zestaw metadanych w bazie danych
7. System wyświetla potwierdzenie pomyślnego dodania nowego zestawu metadanych
8. Nowy zestaw staje się widoczny na liście dostępnych zestawów metadanych

## 4. Przebiegi alternatywne

### 4.1. Brak dostępnych metadanych

1. System wykrywa, że nie istnieją zarejestrowane metadane do włączenia w zestaw
2. System wyświetla komunikat "Brak zarejestrowanych metadanych. Najpierw zarejestruj metadane"
3. System przekierowuje administratora do formularza rejestracji metadanych
4. Przypadek użycia zostaje wstrzymany

### 4.2. Niekompletne dane

1. System wykrywa brakujące obowiązkowe pola zestawu metadanych
2. System wyświetla komunikat o błędzie wskazujący brakujące pola
3. System uniemożliwia zatwierdzenie formularza do czasu uzupełnienia danych
4. Administrator uzupełnia brakujące dane i ponownie zatwierdza formularz

### 4.3. Duplikat nazwy zestawu

1. System wykrywa, że zestaw metadanych o podanej nazwie już istnieje w systemie
2. System wyświetla komunikat o błędzie informujący o konflikcie nazw
3. Administrator zmienia nazwę zestawu i ponownie zatwierdza formularz

### 4.4. Administrator anuluje operację

1. Administrator wybiera opcję "Anuluj" przed zatwierdzeniem formularza
2. System zamyka formularz dodawania bez zapisywania wprowadzonych danych
3. System powraca do poprzedniego widoku

## 5. Warunki początkowe

- Administrator jest zalogowany do systemu
- Administrator posiada uprawnienia do dodawania zestawów metadanych
- W systemie istnieją zarejestrowane metadane, które można włączyć do zestawu

## 6. Warunki końcowe

- Nowy zestaw metadanych został pomyślnie dodany do systemu
- Zestaw metadanych jest dostępny dla użytkowników z odpowiednimi uprawnieniami
- Administrator może zarządzać utworzonym zestawem (edytować, usuwać)

## 7. Wymagania specjalne

- Interfejs dodawania zestawu powinien umożliwiać wygodne wybieranie metadanych z dostępnej puli
- System powinien zapewniać unikalność nazw zestawów metadanych
- Zestaw metadanych musi zawierać przynajmniej jeden element metadanych

## 8. Rozszerzenia

Automatyczne wylogowanie przy braku aktywności użytkownika

## 9. Słownik pojęć dla PU014

### Zestaw metadanych

- **Definicja**: Uporządkowana kolekcja powiązanych ze sobą metadanych tworzących logiczną całość, służąca do opisu określonego typu zasobu lub kategorii danych
- **Synonim**: Kolekcja metadanych, Grupa metadanych, Szablon metadanych
- **Użycie**: Administrator tworzy zestaw metadanych zawierający pola niezbędne do opisu publikacji naukowej

### Metadane

- **Definicja**: Dane opisujące inne dane, zawierające informacje o strukturze, atrybutach i kontekście opisywanych danych
- **Synonim**: Dane o danych, Atrybuty danych
- **Użycie**: Metadane zawierają informacje takie jak autor, data utworzenia czy format dokumentu

### Rejestracja metadanych

- **Definicja**: Proces definiowania i wprowadzania do systemu nowego typu metadanych przed ich wykorzystaniem w zestawach
- **Synonim**: Definiowanie metadanych, Utworzenie metadanych
- **Użycie**: Przed utworzeniem zestawu metadanych, administrator musi zarejestrować wszystkie potrzebne typy metadanych

### Dodanie zestawu metadanych

- **Definicja**: Proces tworzenia nowej kolekcji metadanych poprzez wybór i organizację wcześniej zarejestrowanych elementów metadanych
- **Synonim**: Utworzenie zestawu metadanych, Kompilacja metadanych
- **Użycie**: Administrator dodaje nowy zestaw metadanych, aby umożliwić uporządkowane opisywanie zasobów w systemie
