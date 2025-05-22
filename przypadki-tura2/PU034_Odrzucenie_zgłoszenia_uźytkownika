# **PU0021: Odrzucenie_zgłoszenia_uźytkownika**

#### Autor: Michał Janaszewski

## 1. SCENARIUSZ GŁÓWNY 

**PRE:** Administrator jest zalogowany do systemu i wyświetlone jest zgłoszenie użytkownika.

1. Administrator wybiera opcję „Odrzuć zgłoszenie”.
2. System wyświetla okno potwierdzenia.
3. Administrator potwierdza wybierając "Usuń".
4. System usuwa zgłoszenie.
5. System wyświetla komunikat o usunięciu zgłoszenia.

**FINAL:** SUCCESS.\
**POST:** W bazie danych zostało usunięte zgłoszenie użytkownika.

## 2. PRZEBIEGI ALTERNATYWNE

### 2.1. SCENARIUSZ ALTERNATYWNY 1 – Anulowanie odrzucenia

1.-2. Tak samo, jak w SCENARIUSZU GŁÓWNYM.
3. a. Administrator anuluje odrzucenie zgłoszenia wybierając "Anuluj".
4. a. System zamyka okno potwierdzenia odrzucenia.

**FINAL:** FAILURE.\
**POST:** W bazie danych niezostała wprowadzona żadna zmiana zgłoszenia użytkownika.

### 2.2. SCENARIUSZ ALTERNATYWNY 2 – Błąd usuwania zgłoszenia

1.-3. Tak samo, jak w SCENARIUSZU GŁÓWNYM.
4. b. System nie usuwa zgłoszenia.
5. b. System wysietla komuniak o błędzie usunięcia odrzucenia.

**FINAL:** FAILURE.\
**POST:** W bazie danych niezostała wprowadzona żadna zmiana zgłoszenia użytkownika.

## 3. SŁOWNIK POJĘĆ

### Okno potweirzenia odrzucenia

* **Definicja**: okno potwierdzające odrzucenie zgłoszenia, zawiera dwie opcje: "Usuń" do usunięcia zgłoszenia oraz "Anuluj" do anulowania odrzucenia zgłoszenia. (poprawiono "zawiea" → "zawiera", dodano przecinki i dwukropek)
