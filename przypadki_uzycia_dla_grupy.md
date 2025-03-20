# Przypadki użycia dla grupy

Adrian Rybaczuk:
*   **Wyświetlenie listy użytkowników**: Administrator **może przeglądać listę użytkowników systemu**. Jest to kluczowy element zarządzania, umożliwiający monitorowanie aktywnych kont.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Jakie informacje o użytkownikach są wyświetlane na liście (np. nazwa użytkownika, rola, data ostatniego logowania)?
    - Czy lista użytkowników jest stronicowana lub posiada mechanizm wyszukiwania?
    - Czy administrator może eksportować listę użytkowników do pliku (np. CSV, Excel)?
*   **Przypisanie uprawnień/roli użytkownikowi do źródła danych**: Administrator **może przypisywać użytkownikom role i uprawnienia do różnych zasobów**. Ten przypadek użycia rozszerza wyświetlenie listy użytkowników.\
    [(CF0005) Zarządzanie uprawnieniami](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0005.md)
    - Jakie role i uprawnienia mogą być przypisane użytkownikom?
    - Czy system wspiera dziedziczenie uprawnień?
    - Czy administrator może przypisywać uprawnienia grupom użytkowników?
*   **Zmiana uprawnień**: Administrator **może modyfikować istniejące uprawnienia użytkowników**. Jest to kluczowe dla zarządzania dostępem i zabezpieczeń systemu.\
    [(CF0005) Zarządzanie uprawnieniami](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0005.md)
    - Czy zmiana uprawnień jest rejestrowana w audycie systemu?
    - Czy administrator może cofnąć zmiany uprawnień?
    - Jakie mechanizmy kontroli są dostępne, aby zapobiec przypadkowemu nadaniu zbyt szerokich uprawnień?

Artem Omelchenko:
*   **Rejestracja w systemie**: Nowy użytkownik **może zarejestrować się w systemie**.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Jakie informacje są wymagane podczas rejestracji użytkownika?
    - Jak system weryfikuje poprawność danych wprowadzonych podczas rejestracji?
    - Jakie są procedury w przypadku nieudanej rejestracji?
    - Jakie powiadomienia otrzymuje użytkownik po zakończeniu procesu rejestracji?
*   **Logowanie do systemu**: Użytkownik **może zalogować się do systemu**.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Jakie metody uwierzytelniania są dostępne dla użytkowników (np. hasło, uwierzytelnianie dwuskładnikowe)?
    - Co się dzieje, gdy użytkownik wprowadzi błędne dane logowania?
    - Jak długo użytkownik może pozostać zalogowany w systemie bez aktywności?
    - Jak system monitoruje i rejestruje próby logowania?
*   **Nadanie hasła**: Administrator **przypisuje użytkownikowi nowe hasło**.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Jakie są zasady dotyczące bezpieczeństwa haseł (np. minimalna długość, złożoność)?
    - Jak system informuje użytkownika o nadaniu nowego hasła?
    - Jaki jest **proces nadawania hasła**? Czy system generuje hasło automatycznie, czy administrator wprowadza je ręcznie?
    - W jaki sposób nowe hasło jest przekazywane użytkownikowi?
    - Jakie są kroki, które administrator musi podjąć, aby przypisać nowe hasło użytkownikowi?

Bartek Cylwik:
*   **Zmiana hasła**: Użytkownik **może zmienić swoje hasło**, co zwiększa bezpieczeństwo konta.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Czy użytkownik musi podać swoje stare hasło przed zmianą na nowe?
    - Czy istnieją wymagania dotyczące złożoności nowego hasła (np. minimalna długość, duże litery, cyfry, znaki specjalne)?
    - Czy użytkownik otrzymuje powiadomienie (np. e-mail) o zmianie hasła?
Usunięcie konta
*   **Usunięcie konta**: Administrator **może usunąć konto użytkownika**, co kończy jego dostęp do systemu.\
    [(CF0010) Rejestracja działań użytkowników](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0010.md)
    - Czy użytkownik otrzymuje potwierdzenie o usunięciu konta przed zakończeniem procesu?
    - Czy po usunięciu konta przechowywane są jakiekolwiek dane użytkownika (np. do celów archiwalnych lub zgodności z przepisami)?
    - Czy administrator może cofnąć decyzję o usunięciu konta w określonym czasie?
*   **Wyświetlenie listy źródeł**: Administrator **może przeglądać listę dostępnych źródeł danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Czy lista źródeł może być filtrowana według określonych kryteriów (np. typ źródła, data dodania)?
    - Czy administrator może sortować listę źródeł według różnych parametrów (np. nazwa, status, ostatnia aktualizacja)?
    - Czy system zapisuje historię wyświetleń listy źródeł dla celów audytu?

Jakub Wypych:
*    **Eksport listy źródeł do pliku**: Administrator **może zapisać listę źródeł do pliku**, co pozwala na dalszą analizę.\
    [(CF0004) Generowanie raportów i backupów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0004.md)  
    - W jakim formacie plik ma być generowany (CSV, XLSX, JSON, XML)?  
    - Czy plik ma być szyfrowany lub zabezpieczony hasłem?  
    - Czy eksportowana lista ma zawierać wszystkie szczegóły źródeł danych czy tylko wybrane pola?
*   **Rejestracja nowego źródła danych**: Administrator **może dodać nowe źródło danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Jakie informacje są wymagane podczas rejestracji źródła (np. nazwa, typ, lokalizacja, właściciel)?
    - Czy źródło danych może mieć przypisane kategorie lub tagi?
    - Czy rejestracja źródła powinna inicjować jakiś workflow np. akceptacyjny?
    - Czy system powinien walidować poprawność danych podczas rejestracji? Jakie reguły walidacji?
*   **Dodanie nowego zestawu metadanych**: Po rejestracji źródła administrator **może dodać zestaw metadanych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Czy administrator może definiować nowe typy metadanych?
    - Jakie pola powinny być obowiązkowe w metadanych?

Jan Gębal: 
*   **Wyszukanie źródła danych**: Administrator **może przeszukiwać istniejące źródła danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Jakie kryteria wyszukiwania będą dostępne dla administratora? (np. nazwa, typ, status, data utworzenia)
    - Czy dostęp do wyszukiwania powinien być ograniczony w zależności od ról użytkowników?
    - Jakie informacje o znalezionych źródłach danych będą wyświetlane w wynikach wyszukiwania?
*   **Archiwizacja źródeł danych**: Administrator **może oznaczyć źródło jako archiwalne**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Jakie są konsekwencje oznaczenia źródła jako archiwalne? (np. blokada edycji, brak widoczności w wyszukiwarce)
    - Czy możliwe jest cofnięcie archiwizacji?
    - Czy użytkownicy nadal będą mieli dostęp do archiwalnych źródeł?
*   **Zlecenie automatycznej kontroli poprawności źródła danych**: Administrator **może zlecić systemowi sprawdzenie poprawności źródła**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)
    - Jakie aspekty źródła danych są sprawdzane w ramach automatycznej kontroli? (np. kompletność, poprawność formatów, dostępność)
    - Czy administrator może konfigurować zakres weryfikacji?
    - Jak system powiadamia administratora o wynikach kontroli?
    - Czy istnieje możliwość ręcznej korekty po wykryciu błędów?
    
Kamil Mądrzyk:  
*    **Usunięcie źródła danych**: Administrator **może usunąć wybrane źródło danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)  
    - Jakie są wymagania dotyczące usunięcia źródła danych? Czy administrator musi spełnić określone warunki przed usunięciem?
    - Czy po usunięciu źródła dane powinny być trwale usuwane czy jedynie oznaczane jako archiwalne?
    - Czy system powinien rejestrować historię usuniętych źródeł i umożliwiać ich odzyskanie?
*   **Wyświetlenie informacji o źródle danych**: Administrator **może zobaczyć szczegółowe informacje o danym źródle**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)  
    - Jakie informacje o źródle danych powinny być dostępne dla administratora?
    - Czy wyświetlane informacje powinny obejmować historię zmian i operacji na danym źródle?
    - Czy istnieją ograniczenia dotyczące dostępu do szczegółowych informacji o źródle danych w zależności od ról użytkowników?
*   **Pobranie szczegółowych informacji o źródle danych**: Możliwość uzyskania rozszerzonych informacji o danym źródle.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)  
    - W jakich formatach administrator powinien móc pobierać szczegółowe informacje o źródle danych?
    - Czy eksportowane dane powinny zawierać pełną historię zmian źródła?
    - Czy dostęp do pobierania szczegółowych informacji powinien być ograniczony na podstawie ról i uprawnień użytkowników?

Maciej Przybylski:
*    **Edycja metadanych**: Administrator **może edytować metadane** przypisane do źródła danych.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Jakie kryteria uprawniają administratora do edycji metadanych przypisanych do źródła danych?
     - Które elementy informacji o źródle danych są aktualizowane i jak często powinno się je weryfikować?
     - Czy istnieją specyficzne procedury lub narzędzia wspomagające rejestrację oraz aktualizację tych informacji?
*   **Zagregowanie metadanych**: Możliwość **scalenia i analizy metadanych** z różnych źródeł.\
    [(CF0001) Agregacja danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0001.md)
    - Z jakich rodzajów źródeł danych zbierane są metadane do agregacji?
    - Jakie narzędzia lub technologie są wykorzystywane do scalenia i analizy metadanych z różnych źródeł?
    - Czy istnieją standardy lub kryteria, które muszą być spełnione przy łączeniu metadanych z wielu systemów?

*   **Walidacja poprawności metadanych**: Sprawdzenie **czy metadane spełniają wymagane kryteria jakości**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)
    - Jakie kryteria jakości są stosowane podczas automatycznej weryfikacji poprawności metadanych?
    - Jakie mechanizmy są używane do identyfikacji i zgłaszania potencjalnych błędów w metadanych?
    - Czy istnieje procedura eskalacji problemów wykrytych w czasie automatycznej walidacji, a jeśli tak – jak wygląda jej przebieg?

Marcin Komza:
- **Sprawdzanie kompletności danych w źródle**: Weryfikacja, czy dane są **pełne i nie brakuje istotnych elementów**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)
    - Jakie konkretnie elementy danych są uważane za istotne i których brak będzie wskazywał na niekompletność źródła?
    - Czy istnieją jakieś ustalone standardy lub normy, względem których będzie oceniana kompletność danych w źródle? Jeśli tak, jakie to są standardy?
    - W jaki sposób system będzie informował pracownika o braku istotnych elementów w danych źródłowych? Czy będzie generowany jakiś raport lub komunikat?

- **Identyfikacja nieaktualnych metadanych**: System **może wskazać metadane, które straciły aktualność**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)

    - Jakie kryteria będą decydowały o tym, że metadane zostaną uznane za nieaktualne? Czy będzie to związane z datą ich ostatniej modyfikacji, brakiem powiązania z aktualnymi danymi, czy innymi czynnikami?
    - W jaki sposób system będzie wskazywał, które metadane straciły aktualność? Czy będzie to wizualne oznaczenie, generowanie powiadomień, czy inne metody?
    - Czy system będzie sugerował jakieś akcje w związku z identyfikacją nieaktualnych metadanych (np. aktualizację, weryfikację)?
  
- **Weryfikacja zgodności źródła z systemem CKAN**: Sprawdzenie **czy dane są zgodne z platformą CKAN**.\
    [(CF0008) Integracja z CKAN](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0008.md)
    
    - Jakie aspekty danych będą weryfikowane pod kątem zgodności z platformą CKAN (np. format danych, schemat metadanych, struktura plików)?
    - Czy istnieją jakieś konkretne standardy CKAN, z którymi źródło musi być zgodne? Jeśli tak, jakie to są standardy?
    - Co się stanie, jeśli źródło danych nie będzie zgodne z systemem CKAN? Czy system zablokuje wprowadzenie danych, wygeneruje raport o błędach, czy podejmie inne działania?

Marta Stankievich:
*    **Weryfikacja organizacji chcącej dodawać źródła**: Administrator **sprawdza organizację**, zanim ta uzyska możliwość dodawania nowych źródeł danych.\
     [(CF0011) Automatyzacja rejestracji firm](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0011.md)
     - Jakie kryteria są brane pod uwagę podczas weryfikacji organizacji zewnętrznej chcącej dodawać źródła metadanych do systemu? (np. formalne, prawne, dotyczące reputacji)
     - Czy proces weryfikacji organizacji jest w pełni automatyczny, czy wymaga również manualnej weryfikacji przez administratora? Jeśli tak, jakie elementy podlegają weryfikacji manualnej?
     - W jaki sposób system powiadamia administratora o nowej organizacji oczekującej na weryfikację
     - Czy system rejestruje historię weryfikacji organizacji? (datę zgłoszenia, administratora weryfikującego, status weryfikacji, ewentualne uwagi)
*   **Weryfikacja konkretnego źródła danych z organizacji**: Administrator **może przeprowadzić kontrolę konkretnego źródła danych**, aby zapewnić jego zgodność z wymaganiami systemu.\
    [(CF0012) Dostęp do formularza rejestracji sprawdzającego dane w KRS](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0012.md)
    - Jakie parametry i standardy są weryfikowane podczas kontroli konkretnego źródła danych? (np. format danych, metadane, aktualność)
    - Jakie działania może podjąć administrator w systemie w zależności od wyniku weryfikacji źródła danych (oprócz zaakceptowania i odrzucenia))?
    - Czy w przypadku negatywnego wyniku weryfikacji źródła danych, system umożliwia organizacji poprawę danych i ponowne zgłoszenie do weryfikacji?
*   **Wyświetlenie listy źródeł**: Użytkownik **może przeglądać dostępne źródła danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
    - Jakie informacje o źródłach danych są prezentowane użytkownikowi na liście dostępnych źródeł?
    - Czy dostęp do listy źródeł jest ograniczony w zależności od roli użytkownika (np. mieszkańcy widzą inne źródła niż pracownicy administracji)

Mateusz Tyl:
*   **Wyszukanie źródła danych**: Użytkownik **może wyszukiwać konkretne źródła danych**, rozszerzając funkcjonalność przeglądania listy źródeł.\
[(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md) \
    - Jakie kryteria wyszukiwania będą dostępne dla użytkownika?
    - Czy system powinien umożliwiać filtrowanie wyników (np. wg daty, typu źródła)?
    - Jak prezentowane będą wyniki wyszukiwania (lista, tabela, dodatkowe metadane)?
    - Czy wyszukiwanie ma uwzględniać jednocześnie różne słowa kluczowe?
*   **Wyświetlenie informacji o źródle danych**: Użytkownik **może zobaczyć szczegółowe informacje na temat wybranego źródła**.\
[(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)\
    - Jakie dokładnie informacje o źródle mają być prezentowane użytkownikowi?
    - Czy dostępne będą odnośniki do powiązanych danych lub historii edycji?
    - Czy poziom szczegółowości prezentowanych danych zależy od uprawnień użytkownika?
    - W jaki sposób system powinien reagować na brak pewnych informacji (np. pola puste, dane nieaktualne)?
*   **Zwizualizowanie danych na mapie**: Użytkownik **może zobaczyć dane przedstawione na mapie**, co umożliwia ich przestrzenną analizę.\
[(CF0006) Wizualizacja danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0006.md)\
    - Jakie typy danych mają być wyświetlane na mapie (punkty, polygon, wartości)?
    - Czy wizualizacja ma uwzględniać różne warstwy lub style wyświetlania (np. heatmapa)?
    - Jakie interakcje z mapą są przewidywane (przybliżanie, zaznaczanie obszaru, kliknięcie w punkt)?
    - Czy użytkownik może eksportować lub zapisywać zestaw wizualizowanych danych (np. zrzut ekranu, plik)?

Michał Janaszewski: 
- **Wyświetlenie listy zgłoszeń użytkowników**: Administrator **może przeglądać zgłoszenia problemów przesłane przez użytkowników**.\
    [(CF0013) Zgłaszanie problemów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)
    - Jakie informacje są dostępne dla administratora w widoku zgłoszenia (np. status, kategoria, priorytet, opis problemu)?
    - Czy użytkownicy otrzymują powiadomienia o zmianach statusu ich zgłoszenia?
    - Jak długo przechowywane są zamknięte zgłoszenia w systemie?
    - Czy system generuje statystyki dotyczące liczby zgłoszeń według kategorii i statusu?
- **Generowanie raportów o zgłoszeniach użytkowników**: Administrator **może wygenerować raporty na podstawie zgłoszeń**.\
    [(CF0004) Generowanie raportów i backupów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0004.md)
    - Jakie metryki i dane są uwzględniane w raportach dotyczących zgłoszeń?
    - Czy raporty mogą być generowane według określonych filtrów (np. zgłoszenia z ostatniego miesiąca, tylko nierozwiązane zgłoszenia)?
    - Czy administrator może wyeksportować raporty do różnych formatów (np. PDF, CSV, Excel)?
    - Czy raporty mogą być generowane w formie wykresów lub wizualizacji danych?
    - Jak długo przechowywane są wygenerowane raporty?
- **Wyświetlenie listy zarchiwizowanych raportów**: Administrator **może przeglądać wcześniejsze raporty dotyczące zgłoszeń**.\
    [(CF0004) Generowanie raportów i backupów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0004.md)
    - Jakie kryteria decydują o archiwizacji raportu?
    - Jakie metadane są dostępne dla raportów archiwalnych (np. data utworzenia, autor, okres raportowania)?
    - Jak długo przechowywane są raporty w archiwum i czy istnieje mechanizm ich automatycznego usuwania?
    - Czy system pozwala na eksportowanie zarchiwizowanych raportów?

Mikołaj Pątkowski:
- **Wyświetlenie informacji o zgłoszeniu**: Administrator **może zobaczyć szczegóły konkretnego zgłoszenia użytkownika**.  
    [(CF0013) Zgłaszanie problemów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)
    - Jakie informacje powinny być widoczne w szczegółach zgłoszenia? (np. data zgłoszenia, opis problemu, status, dane użytkownika)
    - W jaki sposób administrator powinien móc filtrować lub wyszukiwać zgłoszenia? (np. po numerze zgłoszenia, dacie, statusie)
    - Czy administrator powinien mieć możliwość eksportu danych o zgłoszeniu do pliku? (np. PDF, CSV)
- **Odrzucenie zgłoszenia użytkownika**: Administrator **może odrzucić zgłoszenie, jeśli uzna je za nieistotne**.  
    [(CF0013) Zgłaszanie problemów](../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)
    - Jakie powody odrzucenia zgłoszenia powinien móc wybrać administrator? (np. lista predefiniowanych powodów, możliwość wpisania własnego uzasadnienia)
    - Czy użytkownik, którego zgłoszenie zostało odrzucone, powinien otrzymać powiadomienie? (np. powód odrzucenia, data)
    - Czy odrzucone zgłoszenie powinno być archiwizowane? (np. na jak długo i w jaki sposób)
- **Przyjęcie zgłoszenia użytkownika**: Administrator **może zaakceptować zgłoszenie i podjąć działania naprawcze**.  
    [(CF0013) Zgłaszanie problemów](../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)
    - Jakie kroki powinien podjąć administrator po zaakceptowaniu zgłoszenia? (np. przypisanie do działu, osoby odpowiedzialnej)
    - Czy użytkownik powinien otrzymać powiadomienie o zaakceptowaniu zgłoszenia? (np. przewidywany czas rozwiązania problemu)
    - Czy system powinien umożliwiać śledzenie postępów w realizacji zgłoszenia? (np. statusy: "w trakcie realizacji", "zakończone", "wstrzymane")

Wojciech Grot:
**Przegląd ocen jakości źródła danych**: Użytkownik **może sprawdzić ocenę jakości źródła danych**.\
[(CF0007) Możliwość oceny danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0007.md)
- Jakie informacje użytkownik otrzymuje w ramach oceny jakości źródła danych?
- Jakie kryteria są brane pod uwagę przy ocenie jakości źródła danych?
- Czy ocena jakości źródła danych jest prezentowana w formie liczbowej, opisowej czy obu?
- Czy użytkownik może zobaczyć historię ocen jakości danego źródła?
- Czy dostęp do oceny jakości źródła danych wymaga dodatkowych uprawnień (załozenia konta)?



*   **Zgłaszanie błędów i problemów z metadanymi**: Użytkownik **może zgłosić błędy dotyczące metadanych wybranego źródła**.\
[(CF0013) Zgłaszanie problemów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)

-Jakie rodzaje błędów dotyczących metadanych użytkownik może zgłosić?
-Czy użytkownik może dodać szczegółowy opis problemu z metadanymi?
-Czy użytkownik otrzymuje informację zwrotną o statusie swojego zgłoszenia?
-Czy istnieje możliwość dołączania załączników (np. zrzutów ekranu) do zgłoszeń błędów?

*   **Nadanie oceny jakości źródła metadanych**: Użytkownik **może ocenić jakość metadanych danego źródła**.\
[(CF0007) Możliwość oceny danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0007.md)

- Na jakiej podstawie użytkownik może ocenić jakość metadanych?
- Czy ocena jakości metadanych jest w jakiś sposób ustandaryzowana (np. skala liczbowa, ocena opisowa)?
- Czy użytkownik może dodać komentarz do swojej oceny?
- Czy oceny jakości metadanych mogą być edytowane lub usuwane przez użytkownika?
- Czy system przechowuje historię ocen jakości metadanych dla danego źródła?
