#### Diagram Klas

##### Diagram

:[Diagram Klas](diagram.puml)

##### Opis

Diagram przedstawia główne klasy modelujące system zarządzania danymi i użytkownikami:

- **Użytkownik**  
  - Atrybuty: `id`, `imie`, `nazwisko`, `email`, `login`, `haslo`, `rola`, `uprawnienia` (wszystkie prywatne).  
  - Operacje: `zarejestruj()`, `zaloguj()`, `wyloguj()`, `zmienHaslo()`, `przegladajZrodla()`, `zglosProblem()`, `ocenDane()`, `wyszukajZrodla()`.

- **Administrator**  
  - Operacje: `przypiszRole()`, `utworzUzytkownika()`, `usunUzytkownika()`, `nadajHasloUzytkownikowi()`, `zweryfikujOrganizacje()`, `edytujMetadane()`, `eksportujListeZrodel()`, `utworzKopieZapasowa()`, `zarchiwizujZrodlo()`, `rozwiazZgloszenie()`, `generujRaportZgloszen()`, `eksportujRaport()`, `monitorujStanSystemu()`.

- **Organizacja**  
  - Atrybuty: `id`, `nazwa`, `email`, `opis`, `status`, `dataWeryfikacji`, `zweryfikowanePrzez` (wszystkie prywatne).  
  - Operacje: `zlozDoWeryfikacji()`, `zlozZrodloDoWeryfikacji()`.

- **ZrodloDanych**  
  - Atrybuty: `id`, `nazwa`, `opis`, `tagi`, `wlasciciel`, `dataUtworzenia`, `dataAktualizacji`, `status`, `czyZarchiwizowane` (wszystkie prywatne).  
  - Operacje: `edytujDane()`, `aktualizujDane()`, `sprawdzKompletnosc()`, `eksportujDoRDF()`.

- **Metadane**  
  - Atrybuty: `id`, `idZrodla`, `dataUtworzenia`, `dataAktualizacji`, `osobaKontaktowa`, `emailKontaktowy`, `licencja` (wszystkie prywatne).  
  - Operacje: `walidujMetadane()`, `aktualizujMetadane()`, `generujRaportWalidacji()`, `eksportujMetadane()`.

- **Zgloszenie**  
  - Atrybuty: `id`, `komentarz`, `zalacznik`, `autor`, `status`, `czasRozpatrzenia`, `dataUtworzenia`, `dataModyfikacji` (wszystkie prywatne).  
  - Operacje: `generujZgloszenie()`, `wyswietlListeZgloszen()`, `wyswietlSzczegolyZgloszenia()`, `zaktualizujStatus()`.

- **Ocena**  
  - Atrybuty: `id`, `ocena`, `komentarz`, `autor`, `dataOceny` (wszystkie prywatne).  
  - Operacje: `ocen()`.

- **KopiaZapasowa**  
  - Atrybuty: `id`, `data`, `typ`, `status`, `rozmiar` (wszystkie prywatne).  
  - Operacje: `utworzKopie()`, `zweryfikujKopie()`.

- **RaportZgloszen**  
  - Atrybuty: `id`, `status`, `czasRozpatrzenia`, `dataUtworzenia` (wszystkie prywatne).  
  - Operacje: `generuj()`, `eksportujDoPDF()`, `eksportujDoCSV()`, `zarchiwizujRaport()`.

Relacje między klasami ilustrują następujące zależności:

- **Relacja między Użytkownik a Zgloszenie:**  
  Każdy użytkownik może zgłaszać wiele zgłoszeń, co pozwala na śledzenie problemów i sugestii dotyczących systemu. Zgłoszenia te mogą być przeglądane i zarządzane przez administratorów.

- **Relacja między Użytkownik a Ocena:**  
  Użytkownicy mogą oceniać dane, co umożliwia zbieranie opinii i ocen dotyczących jakości i przydatności danych. Oceny te mogą być używane do poprawy jakości danych.

- **Relacja między Organizacja a ZrodloDanych:**  
  Organizacje mogą dodawać wiele źródeł danych, co pozwala na centralizację i zarządzanie danymi w ramach jednej jednostki. Każde źródło danych jest przypisane do konkretnej organizacji, co ułatwia zarządzanie i kontrolę dostępu.

- **Relacja między Administrator a KopiaZapasowa:**  
  Administratorzy mogą tworzyć kopie zapasowe danych, co jest kluczowe dla zapewnienia bezpieczeństwa i integralności danych. Kopie zapasowe mogą być używane do przywracania danych w przypadku awarii systemu.

- **Relacja między ZrodloDanych a Zgloszenie:**  
  Zgłoszenia mogą dotyczyć konkretnych źródeł danych, co pozwala na identyfikację i rozwiązywanie problemów związanych z danymi. Każde zgłoszenie jest powiązane z jednym lub więcej źródłami danych.

- **Relacja między ZrodloDanych a Ocena:**  
  Każde źródło danych może mieć wiele ocen, co pozwala na zbieranie informacji zwrotnych od użytkowników na temat jakości danych.

- **Relacja między ZrodloDanych a Metadane:**  
  Każde źródło danych posiada dokładnie jedne metadane, które zawierają szczegółowe informacje o źródle, takie jak data utworzenia, aktualizacji, oraz osoba kontaktowa.

- **Relacja między RaportZgloszen a Zgloszenie:**  
  Raporty zgłoszeń mogą zawierać wiele zgłoszeń, co pozwala na generowanie zbiorczych raportów dotyczących problemów i sugestii zgłaszanych przez użytkowników.

Diagram ten pomaga zrozumieć strukturę systemu zarządzania danymi i użytkownikami oraz zależności między różnymi elementami systemu, co jest kluczowe przy projektowaniu systemu opartego na tych encjach.

##### Kod diagramu

```
:[Diagram klas](diagram.klas.puml)
```
