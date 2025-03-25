# Sekcja 1: Pytania i Odpowiedzi

## 1. Cele i wymagania biznesowe

**Pytanie 1:**  
_Jakie problemy biznesowe ma rozwiązać system?_  
**Odpowiedź:**  
System ma umożliwić otwarty dostęp do publicznych informacji o źródłach danych.
Jego zadaniem jest zebranie i ujednolicenie informacji dotyczących m.in.
lokalizacji, charakterystyki i specyfiki źródeł, aby mieszkańcy oraz inne
podmioty mogły łatwo uzyskać potrzebne informacje, a zewnętrzni użytkownicy –
zarówno programiści, jak i osoby udostępniające informacje o własnych źródłach –
mogli je wykorzystać zgodnie z obowiązującymi normami i standardami.

**Pytanie 2:**  
_Jaki jest cel i zastosowanie poszczególnych składników systemu w odniesieniu do
procesów biznesowych?_  
**Odpowiedź:**

- **Interfejs użytkownika (UI):** Umożliwia bezpośredni dostęp do informacji o
  źródłach (np: przy pomocy telefonu możliwość zobaczenia liczby osób w kolejce
  u doktora). oraz ich edycję przez upoważnionych pracowników.
- **API:** Zapewnia automatyczny dostęp do informacji, co ułatwia integrację z
  systemami zewnętrznymi i umożliwia programistom pobieranie danych w
  ustandaryzowanej formie.

**Pytanie 3:**  
_Jaka jest grupa docelowa użytkowników i jakie są ich główne potrzeby?_  
**Odpowiedź:**

- **Programiści:** korzystający z API.
- **Pracownicy administracji:** rejestrujący i wprowadzający informacje o
  źródłach danych.
- **Administratorzy i kierownictwo:** zarządzający systemem (backupowanie,
  bezpieczenstow danych itd).
- **Mieszkańcy:** korzystający z publicznie udostępnianych informacji.
- **Użytkownicy zewnętrzni:** obejmujący zarówno podmioty korzystające z danych,
  jak i osoby udostępniające informacje o własnych źródłach.

## 2. Funkcjonalności systemu

**Pytanie 4:**  
_Jakie są główne cechy i funkcje systemu?_  
**Odpowiedź:**  
System ma umożliwiać rejestrację, aktualizację i zarządzanie informacjami o
źródłach danych, przy czym kluczowym wymogiem jest zgodność informacji z
obowiązującymi standardami oraz możliwość ich dalszego wykorzystania przez
uprawnione podmioty. Z tymi danymi można rozbudowywać inne system, np.
platoframa do sprawdzenia jak autobusy jezda po miescie itd.

**Pytanie 5:**  
_Jakie role użytkowników powinny istnieć i jakie będą ich uprawnienia?_  
**Odpowiedź:**

- **Pracownicy systemu:** odpowiedzialni za obsluga system, wprowadzanie i
  edycję informacji o źródłach danych.
- **Użytkownicy zewnętrzni:** nie tylko korzystający z danych, ale także
  udostępniający informacje o własnych źródłach (np. właściciele instytucji czy
  firm lokalnych).
- **Mieszkańcy:** mający dostęp do publicznie udostępnianych informacji.  
  Uprawnienia do edycji lub dodawania nowych informacji mają wyłącznie osoby
  upoważnione.

**Pytanie 6:**  
_Czy system powinien oferować subskrypcję oraz powiadomienia o zmianach lub
problemach z danymi?_  
**Odpowiedź:**  
System powinien umożliwić subskrypcję oraz powiadomienia – informując
użytkowników o zmianach w źródłach danych, awariach lub aktualizacjach, aby
użytkownicy mieli bieżący wgląd w stan informacji.

**Pytanie 7:**  
_Czy aplikacja mobilna i webowa powinny dostarczać te same funkcjonalności?_  
**Odpowiedź:**  
Obie platformy powinny być dostosowane do specyfiki użytkowania – wersja mobilna
może być zoptymalizowana pod kątem szybkiego dostępu do kluczowych informacji,
głownie dla procosów z obsluga mieskzanców, natomiast wersja webowa może
oferować pełniejszy zakres funkcji zarządzania i raportowania, gdzie
funckjonalność jest bardziej wykonana pod pracowników urzędu.

**Pytanie 8:**  
_Jakie powinny być opcje wyszukiwania i dostosowywania wyświetlania danych
(sortowanie, filtrowanie)?_  
**Odpowiedź:**  
System powinien umożliwiać zaawansowane wyszukiwanie oraz filtrowanie informacji
o źródłach, co ułatwi użytkownikom odnalezienie interesujących ich danych.

## 3. Obsługa i zarządzanie danymi

**Pytanie 9:**  
_Jakie typy źródeł danych może obsługiwać system?_  
**Odpowiedź:**  
System przechowuje informacje na temat źródeł danych (np. pliki, systemy
zewnętrzne, urządzenia pomiarowe), a nie same dane. Dane mogą byc zarówno
dynamiczne, np. wyniki ankiet, albo statyczne jak godzina otwaracai urzędu.
Istotne jest, aby informacje te były zgodne z obowiązującymi standardami oraz
normami krajowymi i unijnymi.

**Pytanie 10:**  
_Czy dane są już w określonych formatach, czy wymagają konwersji przed
publikacją?_  
**Odpowiedź:**  
Informacje o źródłach mogą pochodzić z różnych formatów. Konieczne jest
wdrożenie procedur konwersji i standaryzacji, które zapewnią zgodność z
przyjętymi normami.

**Pytanie 11:**  
_Jakie mechanizmy importu danych masowych powinien obsługiwać system?_  
**Odpowiedź:**  
Obecnie dane są wprowadzane ręcznie przez pracowników. Należy opracować
mechanizmy umożliwiające masowy import informacji, z automatyczną weryfikacją
źródła danych oraz zgodności udostępnianych przez nie informacji ze standardami
i normami.

**Pytanie 12:**  
_Jak system będzie zarządzał archiwizacją, przechowywaniem oraz usuwaniem
danych?_  
**Odpowiedź:**  
Aktualnie zadania te wykonują administratorzy manualnie. W przyszłości warto
opracować procesy automatyzujące archiwizację, przechowywanie oraz usuwanie
informacji o źródłach danych, aby usprawnić operacje i zmniejszyć ryzyko błędów.

## 4. Jakość i spójność danych

**Pytanie 13:**  
_Jak system będzie monitorował jakość danych (aktualność, dokładność,
kompletność) oraz rozwiązywał problem sprzecznych informacji?_  
**Odpowiedź:**  
W obecnym systemie weryfikacja danych odbywa się ręcznie przez pracowników w
trakcie wprowadzania informacji. W przyszłości warto wdrożyć automatyczne
mechanizmy monitoringu, które będą kontrolować zgodność informacji z
obowiązującymi normami oraz generować alerty w przypadku wykrycia niespójności.

**Pytanie 14:**  
_Jak zapewnić spójność danych między różnymi źródłami?_  
**Odpowiedź:**  
Ponieważ system przechowuje wyłącznie informacje o źródłach danych, spójność
dotyczy poprawności wprowadzanych informacji przy ich rejestracji /
aktualizacji.System zakłada ze dane sa dostarczone, ale nie zakłada ich
poprawności. Obecna manualna weryfikacja powinna zostać uzupełniona o
zautomatyzowane procedury.

**Pytanie 15:**  
_Jak system będzie zarządzał priorytetyzacją aktualizacji danych w czasie
rzeczywistym?_  
**Odpowiedź:**  
System powinien umożliwiać ustalanie priorytetów aktualizacji, definiując, które
źródła wymagają częstszej kontroli oraz szybszej reakcji w przypadku awarii lub
niespójności.

## 5. Zarządzanie użytkownikami i interakcje

**Pytanie 16:**  
_W jaki sposób użytkownicy będą mogli zgłaszać uwagi i poprawki do danych? Jak
te zgłoszenia będą weryfikowane i wdrażane?_  
**Odpowiedź:**  
Obecnie zgłoszenia dotyczące niespójności czy problemów z informacjami o
źródłach danych trafiają mailowo lub telefonicznie. W przyszłości warto wdrożyć
system elektronicznego zgłaszania, który umożliwi rejestrację, automatyczną
weryfikację (w miarę możliwości) oraz śledzenie postępów prac nad poprawkami.
Można by było również wprowadzic Ai do werytikowania czy nie dane nie sa jakimś
spammingiem.

**Pytanie 17:**  
_W jaki sposób system będzie wspierał wielojęzyczność metadanych?_  
**Odpowiedź:**  
Obecnie system przewiduje jedynie język polski. W miarę rozwoju warto rozważyć
wdrożenie modułu automatycznej translacji, który pozwoli na prezentowanie
informacji o źródłach danych w innych językach, choć wprowadzanie danych przez
pracowników pozostanie w języku polskim.

## 6. Bezpieczeństwo i dostęp do danych

**Pytanie 18:**  
_Jakie są wymagania dotyczące bezpieczeństwa danych w systemie, szczególnie w
kontekście ochrony prywatności użytkowników?_  
**Odpowiedź:**  
Dane udostępniane przez system są publiczne, co oznacza, że ich dostęp jest
otwarty. Ochrona danych osobowych dotyczy jedynie użytkowników systemu
(edytorów, administratorów itp.) i odbywa się zgodnie z obowiązującymi
procedurami bezpieczeństwa.

**Pytanie 19:**  
_Jak system poradzi sobie z konfliktem interesów w dostępie do danych, np. gdy
część danych podlega ograniczeniom prawnym?_  
**Odpowiedź:**  
Nasz system nie zawiera danych, które wymagałyby ograniczenia dostępu ze względu
na przepisy – wszystkie informacje o źródłach danych są udostępniane publicznie,
a kwestie ograniczeń regulowane są przez obowiązujące dyrektywy i przepisy.

## 7. Wydajność i skalowalność

**Pytanie 20:**  
_Jakie są wymagania dotyczące skalowalności oraz ograniczenia techniczne
systemu?_  
**Odpowiedź:**  
Choć obecnie nie określono szczegółowych wymagań, system musi być elastyczny i
skalowalny, aby sprostać rosnącej liczbie rejestrowanych źródeł informacji oraz
potencjalnie zwiększonej liczbie użytkowników korzystających z otwartych danych.

## 8. Zarządzanie awariami i błędami

**Pytanie 21:**  
_W jaki sposób system powinien obsługiwać sytuacje awaryjne, takie jak przerwy w
dostępie do źródeł danych lub błędne aktualizacje?_  
**Odpowiedź:**  
Obecnie wszelkie incydenty zgłaszane są manualnie. W przyszłości konieczne
będzie opracowanie procedur awaryjnych – obejmujących automatyczne
powiadomienia, backupy i procedury reagowania – aby szybko identyfikować
problemy oraz minimalizować ryzyko długotrwałych zakłóceń.

## 9. Analiza i raportowanie

**Pytanie 22:**  
_Czy istnieją wymagania dotyczące raportowania i analizy wykorzystania
systemu?_  
**Odpowiedź:**  
Aktualnie procesy raportowania są wykonywane manualnie przez administratorów.
Wdrożenie automatycznych mechanizmów raportowania, zgodnych z normami unijnymi i
krajowymi, pozwoli na lepsze monitorowanie stanu systemu i dostosowanie działań
do wymagań instytucjonalnych.

## 10. Weryfikacja danych

**Pytanie 23:**  
_Czy system weryfikuje dane przy ich wprowadzaniu i czy kontrola odbywa się
regularnie?_  
**Odpowiedź:**  
Weryfikacja odbywa się ręcznie przez pracowników w trakcie wprowadzania
informacji. Brakuje systematycznych, automatycznych kontroli – stąd potrzeba
wdrożenia rozwiązań, które będą okresowo sprawdzać poprawność i zgodność
wprowadzonych danych ze zdefiniowanymi standardami.

**Pytanie 24:**  
_Czy sposób dostępu do danych będzie kategoryzowany w zależności od rodzaju
informacji?_  
**Odpowiedź:**  
Dostęp do informacji o źródłach danych jest otwarty i nie wymaga specjalnych
uprawnień. Specjalne uprawnienia są natomiast wymagane jedynie w przypadku
edycji lub dodawania nowych informacji, co zostało już wcześniej opisane.

# Sekcja 2: Procesy biznesowe – Analiza obecnego systemu oraz nowe usprawnienia

## I. Obecne procesy biznesowe w systemie

- **Rejestracja i wprowadzanie danych źródłowych**  
  Pracownicy ręcznie wprowadzają informacje o źródłach danych do systemu.

- **Manualna weryfikacja danych**  
  Dane są sprawdzane „na oko” przez pracowników, bez użycia zautomatyzowanych
  narzędzi weryfikujących zgodność z normami.

- **Zgłaszanie niezgodności i problemów**  
  Użytkownicy (mieszkańcy, odbiorcy danych) zgłaszają błędy, niespójności lub
  brak danych telefonicznie.

- **Manualne zarządzanie backupem i raportowaniem**  
  Administratorzy systemu ręcznie wykonują zadania związane z tworzeniem kopii
  zapasowych, archiwizacją danych oraz generowaniem raportów.

- **Brak automatycznej integracji z systemami zewnętrznymi**  
  Obecny system nie wspiera automatycznej synchronizacji czy wymiany informacji
  z platformami takimi jak CKAN lub innymi systemami zewnętrznymi.

## II. Procesy wymagające poprawy

- **Wprowadzanie danych** Wdrożenie systemu pozwajacego dodanie danych poprzez
  jednostke samorządu w tym z odpowiednim podziałem na role (pracownik,
  kierownik, administrator), oraz udostepnie mozliwosci dodania danych osobom
  zewnetrzym po wczesniejszej weryfikacji

- **Automatyzacja weryfikacji danych**  
  Wdrożenie modułów automatycznej walidacji, które będą sprawdzały zgodność
  zródeł danych z obowiązującymi normami.

- **Mechanizmy masowego importu i konwersji danych**  
  (TUTAJ TRZEBA BYLO BY DOPRACOWAC ODPOWIEDZ W ZWIAZKU Z TYM ZE MY
  PRZECHOWYWUJEMY ZRODLA I JAKO TAKO MASOWO ZRODEL NIE DA SIE WPROAWADZAC BO NIE
  DO KONCA MA TO SENS)

- **Dynamiczne monitorowanie i aktualizacja danych**  
  Wprowadzenie automatycznego monitorowania zródeł danych i ich zgodnosci z
  normami oraz udostepnienie tej informacji razem z informacja o zrodle

- **Automatyzacja backupu i raportowania**  
  Implementacja automatycznych mechanizmów tworzenia kopii zapasowych oraz
  generowania raportów, gdzie raporty powinny byc zgodne z wymaganiami instacji
  wyzszych (kontrolujacych).

- **Usprawnienie systemu zgłaszania i śledzenia błędów**  
  Wdrożenie elektronicznego systemu rejestracji zgłoszeń, umożliwiającego
  monitorowanie statusu zgłoszeń i szybką reakcję.

- **Integracja z systemami zewnętrznymi**  
  Wdrożenie automatycznej integracji z platformami krajowymi i europejskimi
  (m.in. CKAN) oraz udostępnienie interfejsów API.

## III. Dla kogo ten system?

- **Programiści**
- **Pracownicy administracji**
- **Administratorzy i kierownictwo**
- **Mieszkańcy**
- **Użytkownicy zewnętrzni**

## IV. Zweryfikowanie problemów które procesy opisuj

- Powinna być funkcjonalnośc, aby mieszkańcy albo firma wewnetrzna oceniala czy
  system zbiór danych jest przydatny.
- Nie ma procesu dla usunięcia konta. np, dla systemu, której działalnosć jest
  zakonczona, lub zfałszfowana a została wczesniej zarejestrowana
- Wprowadzenie identyfikowania systemu z systemem weryfikującym który np.
  sprawdza czy taka działalność jest zarejestrowana
- Możliwość pobierania informacji ustatystycznionych i ich raportowania
- Zarządzanie uprawnieniami w systemie
