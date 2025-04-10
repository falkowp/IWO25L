# PU011: Wyświetlenie listy metadanych

#### Autor: Patrycja Falkowska

## 1. Cel przypadku użycia  
Administrator może przeglądać listę dostępnych metadanych w systemie.

## 2. Aktorzy  
- Administrator

## 3. Przebieg główny  
1. Administrator przechodzi do sekcji „Metadane” w panelu administracyjnym.  
2. System wyświetla listę wszystkich metadanych dostępnych w systemie.  
3. Dla każdej pozycji system wyświetla szczegóły, takie jak:  
   - Nazwa  
   - Opis  
   - Data utworzenia / modyfikacji  
   - Status (np. aktywne, zarchiwizowane) 

## 4. Przebiegi alternatywne  

### 4.1. Brak metadanych w systemie  
1. System wyświetla komunikat informujący, że brak dostępnych metadanych do wyświetlenia.

## 5. Warunki początkowe  
- Administrator jest zalogowany do systemu.  
- Administrator posiada dostęp do panelu administracyjnego.

## 6. Warunki końcowe  
- Administrator zapoznał się z listą dostępnych metadanych.  
- Administrator może podjąć dalsze działania na wybranych metadanych.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Wyjątki  
- **Błąd pobierania danych z bazy**  
  - System informuje o błędzie technicznym i proponuje ponowne załadowanie listy.

## 9. Słownik pojęć  

### Metadane  
- Dane opisujące inne dane – zawierają informacje o strukturze, pochodzeniu i przeznaczeniu danych.  

### Panel administracyjny  
- Interfejs umożliwiający zarządzanie zasobami systemu przez uprawnionych użytkowników (administratorów).
