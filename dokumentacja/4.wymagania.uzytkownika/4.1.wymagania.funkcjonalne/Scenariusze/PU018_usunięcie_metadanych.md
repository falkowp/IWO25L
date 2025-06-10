# **PU018: Usunięcie metadanych**

#### Autor: Marta Stankevich

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Użytkownik jest zalogowany do systemu, posiada uprawnienia administratora i znajduje się na stronie z listą wszystkich metadanych.

1. Administrator wybiera metadane do usunięcia.
2. Administrator klika opcję "usuń".
3. System wyświetla okno z potwierdzeniem akcji.
4. Administrator klika "ok".
5. System usuwa metadane.
6. System wyświetla wiadomość "metadane zostały usunięte".

**POST:** Wybrane metadane zostały usunięte z listy metadanych.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Anulowanie akcji

1 - 3 Tak samo, jak w SCENARIUSZU GŁÓWNYM

4. a. Administrator klika opcję "Anuluj".
5. a. System wyświetla stronę z listą wszystkich metadanych.

**POST:** Żadne metadane zostały usuniete z listy metadanych.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Błąd ze strony serwera
1 - 5 Tak samo, jak w SCENARIUSZU GŁÓWNYM

6. a.  System wyświetla błąd podczas usunięcia metadanych.
7. a.  Administartor klika "Powrót do listy metadanych"

**POST:** Żadne metadane zostały usuniete z listy metadanych.

## 3. SŁOWNIK POJĘĆ

### Lista metadanych

* **Definicja**: Zbiór danych zawierający pewną liczbę wybranych metadanych.

- **Atrybuty**:
    - Nazwa: tekst
    - Opis: tekst
    - Data utworzenia: data
	- Zawartość: metadane [Lista]
 
### Metadane
- **Definicja**: Dane na temat źródła danych
- **Atrybuty**:
  - id: int
  - idŹródła: int
  - dataUtworzenia: data
  - dataAktualizacji: data
  - osobaKontaktowa: string
  - emailKontaktowy: string
  - licencja: string
