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
*   **Rejestracja nowego źródła danych**: Administrator **może dodać nowe źródło danych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)
*   **Dodanie nowego zestawu metadanych**: Po rejestracji źródła administrator **może dodać zestaw metadanych**.\
    [(CF0003) Rejestracja i aktualizacja informacji o źródłach danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0003.md)

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
*   **Zagregowanie metadanych**: Możliwość **scalenia i analizy metadanych** z różnych źródeł.\
    [(CF0001) Agregacja danych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0001.md)
*   **Walidacja poprawności metadanych**: Sprawdzenie **czy metadane spełniają wymagane kryteria jakości**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)

Marcin Komza:
*    **Sprawdzanie kompletności danych w źródle**: Weryfikacja, czy dane są **pełne i nie brakuje istotnych elementów**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)
*   **Identyfikacja nieaktualnych metadanych**: System **może wskazać metadane, które straciły aktualność**.\
    [(CF0002) Automatyczna weryfikacja metadanych](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0002.md)
*   **Weryfikacja zgodności źródła z systemem CKAN**: Sprawdzenie **czy dane są zgodne z platformą CKAN**.\
    [(CF0008) Integracja z CKAN](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0008.md)

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
 **Wyświetlenie listy zgłoszeń użytkowników**: Administrator **może przeglądać zgłoszenia problemów przesłane przez użytkowników**.\
[(CF0013) Zgłaszanie problemów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0013.md)
*   **Generowanie raportów o zgłoszeniach użytkowników**: Administrator **może wygenerować raporty na podstawie zgłoszeń**.\
[(CF0004) Generowanie raportów i backupów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0004.md)
*   **Wyświetlenie listy zarchiwizowanych raportów**: Administrator **może przeglądać wcześniejsze raporty dotyczące zgłoszeń**.\
[(CF0004) Generowanie raportów i backupów](../../3.wizja.systemu/3.3.cechy.funkcjonalne/cechy.funkcjonalne/CF0004.md)

Mikołaj Pątkowski:
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
