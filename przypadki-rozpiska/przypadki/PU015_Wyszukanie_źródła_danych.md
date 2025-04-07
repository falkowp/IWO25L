# PU015: Wyszukanie źródła danych

#### Autor: Jakub Wypych

## 1. Cel przypadku użycia  
Administrator może przeszukiwać istniejące metadane.

## 2. Aktorzy  
- Administrator

## 3. Przebieg główny  
1. Administrator podaje filtr.  
2. Administrator naciska przycisk "Szukaj".  
3. System pobiera metadane na podstawie filtru.  
4. System wyświetla pobrane metadane.  
5. Administrator może:  
   - Archiwizować metadane (PU016) 
   - Sprawdzić poprawność metadanych (PU017)
   - Usunąć metadane (PU018)
   - Wyświetlić informacje o metadanych (PU019)

## 4. Przebiegi alternatywne  

### 4.1. Reset filtru  
1. Administrator resetuje filtry.  
2. System informuje o resecie i powraca do listy metadanych.

### 4.2. Błąd pobrania metadanych  
1. System napotyka błąd w pobieraniu metadanych.  
2. System informuje o błędzie w pobraniu metadanych i powraca do listy metadanych.

## 5. Warunki początkowe  
- Administrator jest zalogowany do systemu.  
- Administrator znajduje się na liście metadanych (PU011)

## 6. Warunki końcowe  
- Administrator ma wyświetlone metadane na podstawie filtru.

## 7. Wymagania specjalne  
*Nie określono.*

## 8. Rozszerzenia  
- Przejście do operacji na metadanych (PU016–PU019)

## 9. Słownik pojęć dla PU015  

### Filtr  
- **Definicja**: Informacje, na podstawie których będą wyszukiwane metadane — przykładowo atrybuty metadanych  
- **Synonim**: Kryteria wyszukiwania  
- **Użycie**: Administrator ustawia filtr przed przeszukiwaniem metadanych  

### Metadane  
- **Definicja**: Zestaw informacji opisujących źródła danych  
- **Synonim**: Dane opisowe  
- **Użycie**: Metadane są wyszukiwane, wyświetlane i zarządzane przez administratora  
