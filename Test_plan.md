## Plan testów do sklepu internetowego Generic Shop

- ID: PT-Generic Shop_01.1.
- Wersja 1.
- Data: 03.09.
- I. Wprowadzenie SPIS TREŚCI
   - 1. Cel
   - 2. Testowany obiekt
   - 3. Funkcjonalność nietestowana
- II. Podejście do testów
- III. Zakres testów
   - 1. Testy funkcjonalności
   - 2. Testy interfejsu użytkownika
   - 3. Testy regresyjne
- IV. Potrzebne zasoby
   - 1. Zasoby ludzkie
   - 2. Potrzeby szkoleniowe
   - 3. Zasoby programowe
   - 4. Odpowiedzialność za testy
- V. Harmonogram planu testów
- VI. Rezultaty
   - 1. Dzienniki błędów
   - 2. Raporty
- VII. Kryteria zaliczenia
- VIII. Rejestr ryzyk
- IX. Zależności
- X. Zatwierdzenie planu


## I. Wprowadzenie SPIS TREŚCI

### 1. Cel

Celem dokumentu jest nakreślenie ogólnego zarysu testów sprawdzających
poprawność działania aplikacji, a tym samym ułatwienie pracy osobom odpowiedzialnym za
proces testowania oraz ułatwienie całego procesu testowania.

### 2. Testowany obiekt

Testowaniu podlegać będzie aplikacja e-commerce w postaci sklepu internetowego
Generic Shop dostępnego pod adresem: ​http://skleptest.pl/​.

### 3. Funkcjonalność nietestowana

```
Testowanie nie będzie przeprowadzane na urządzeniach mobilnych.
```
## II. Podejście do testów

Testy zostaną przeprowadzone zgodnie z udokumentowanymi przypadkami
testowymi przechowywanymi w Jira Software. Kierownik testów utworzy przebiegi testowe
dla każdego testera. Tester wykona testy w i zaznaczy każdy przypadek jako Pass lub Fail.
Tester powinien zostawić komentarz, jeżeli ma on istotne znaczenie dla odtwarzanego
przypadku.
Gdy testy są oznaczone jako Fail, zostaną automatycznie utworzone raporty o błędach.
Po zakończeniu kierownik testów powinien przejrzeć raporty z przebiegu testów, a
następnie na ich podstawie sporządzić raport, który następnie zostanie przekazany
zespołowi testerskiemu..

## III. Zakres testów

### 1. Testy funkcjonalności

Testy funkcjonalności weryfikują właściwe przyjmowanie, przetwarzanie i
odzyskiwanie danych oraz właściwą implementację wymagań, używając poprawnych i
niepoprawnych danych wprowadzanych do aplikacji podczas testów.
Cel testu Sprawdzenie właściwej funkcjonalności systemu, w tym:
wprowadzanie, przetwarzanie, odzyskiwanie, aktualizację oraz
wyszukiwanie danych.
Technika Zastosowania każdego przypadku użycia wykorzystując zarówno
prawidłowe, jak i nieprawidłowe dane, aby zweryfikować:

- czy wprowadzenie prawidłowych danych spowoduje


```
pojawienie się spodziewanych rezultatów;
```
- czy wprowadzenie nieprawidłowych danych spowoduje
    wyświetlenie się odpowiednich komunikatów;
- sprawdzenie czy każda zasada biznesowa jest poprawnie
    działająca.
Testowane
komponenty
Model, interfejs użytkownika
Metodyka Testowanie ręczne z wykorzystaniem oprogramowania
pomocniczego do testowania.
Wymagania
narzędziowe
- program do konfiguracji systemu;
- narzędzie do wykonywania kopii bezpieczeństwa oraz
narzędzie umożliwiające monitorowanie urządzeń;
- narzędzia pomocne przy obsłudze;
- program do generowania danych.
Kryteria sukcesu - każdy przypadek ze scenariusza użycia przeszedł pomyślnie
test, nie pojawiły się nieprzewidziane błędy.

### 2. Testy interfejsu użytkownika

Testowania interfejsu użytkownika służy do zweryfikowania interakcji z systemem.
Celem tego testu jest sprawdzenie, czy UI zapewnia użytkownikowi właściwy dostęp do
wszystkich funkcji systemu, oraz odpowiednią nawigację przez te funkcje. Dodatkowo dzięki
testowi można sprawdzić czy wszystkie obiekty interfejsu są niezbędne i czy odpowiednie do
standardów.
Cel testu Weryfikacja, czy UI udostępnia użytkownikowi właściwy dostęp do
funkcji systemu
Technika Przeprowadzenie testu umożliwiającego sprawdzenie poprawności
nawigacji przez wszystkie okna oraz obiekty w programie.
Testowane
komponenty
Interfejs użytkownika
Metodyka Test będzie przeprowadzony ręcznie, czyli należy sprawdzić
wszystkie elementy interfejsu użytkownika, czy działają poprawnie.
Wymagane
narzędzia
Programy wspomagające, automatyzujące testowanie.
Kryteria sukcesu Test będzie zakończony sukcesem, gdy wszystkie elementy UI
działają poprawnie. Powinniśmy przeprowadzić test z udziałem
przyszłych użytkowników, aby sprawdzić intuicyjność interfejsu.

### 3. Testy regresyjne

Testy te będa wykonywanie po włączeniu każdego nowego komponentu w celu sprawdzenia
czy nie spowodowało to nowych błędów.
Cel testu Sprawdzenie czy poszczególne części systemu właściwie ze sobą


```
współpracują po dokonanych zmianach.
Technika Przeprowadzenie tych samych testów, które były dokonane przed
każdą iteracją i porównanie wyników
Testowane
komponenty
Wszystkie
Metodyka Testowanie ręczne z wykorzystaniem oprogramowania
pomocniczego do testowania.
Wymagane
narzędzia
Programy wspomagające, automatyzujące testowanie.
Kryteria sukcesu Testy przeszły pomyślnie, nie pojawiły się nieprzewidziane błędy.
```
## IV. Potrzebne zasoby

### 1. Zasoby ludzkie

```
Zespół testowy w projekcie będzie składać się z :
a. kierownika testów (podlega Kierownikowi Projektu);
b. analityka testów (podlega kierownikowi testów, zadania: analiza wymagań,
uczestniczenie w inspekcji dokumentów i kodu, projektowanie testów,
współpraca z kierownikiem testów w zakresie raportowania i monitorowania
postępów);
c. 2 testerów (podlegają kierownikowi testów, zadania: automatyzacja
wykonania testów przez tworzenie skryptów testowych, przeprowadzanie
testów, uczestnictwo w inspekcji dokumentów i kodu, ścisła współpraca z
analitykiem testów).
Kwalifikacje zespołu są potwierdzone odpowiednimi szkoleniami.
```
### 2. Potrzeby szkoleniowe

Przydzieleni testerzy powinni posiadać podstawową wiedzę na temat funkcjonowania
platformy e-commerce.

### 3. Zasoby programowe

```
System operacyjny Windows, MacOS.
Przeglądarka internetowa: ​Chrome 83+, Firefox 78+, Safari 11+
W celu przeprowadzenia miarodajnych testów potrzebne będzie łącze internetowe.
```
### 4. Odpowiedzialność za testy

Zespół programistyczny jest odpowiedzialny za całkowite wdrożenie aplikacji.
Kierownik Projektu ponosi odpowiedzialność za zarządzanie dostępnością testerów,
harmonogram prac oraz dokonanie analizy pod kątem potrzeb szkoleniowych. Testerzy


powinni być poinformowani o oczekiwaniach związanych z terminem zakończenia prac oraz
poziomem jakości. Wszelkie zagrożenia powinny być podawane do informacji na bieżąco.

## V. Harmonogram planu testów

```
Czas trwania projektu: 1.09.2020-30.11.2020.
```
1. tydzień - włączenie do testów bazy danych;
2. tydzień -testy integralności bazy danych;
3. tydzień - facility testing - testowanie założeń (opisanie sposobu działania każdej
    funkcji, przetestowanie każdej funkcji zgodnie z planem);
4. tydzień - testy regresyjne
5. tydzień - testy interfejsu użytkownika;
6. tydzień - testy konfiguracji;
7. tydzień - testy regresyjne;
8. tydzień - testy funkcjonalności;
9. tydzień - testowanie całości;
10.tydzień - ostateczne testy;
11.tydzień - wdrożenie całości.

## VI. Rezultaty

### 1. Dzienniki błędów

Dla każdego testu będą generowane raporty testów, które będą zawierały
najważniejsze informacje: id testu, wykryte usterki. Raporty będą w postaci plików
tekstowych.

### 2. Raporty

```
Usterki wykryte w czasie testowania będą rejestrowane w Jira Software.
```
## VII. Kryteria zaliczenia

Każdy etap, przez jaki przejdzie testowany projekt, ma na celu wykrycie
ewentualnych błędów i wad. Zaliczeniem danego etapu jest wygenerowanie raportu,
obejmującego wyszczególnione błędy. Za zaliczony etap uważa się taki wygląd projektu,
który będzie dopuszczony przez Kierownika Projektu.
Wszystkie procedury testowe muszą zakończyć swoje wykonanie bez wystąpienia
awarii o statusie “krytyczny”, a użytkownik końcowy musi być w stanie wykonać cały cykl
biznesowy bez żadnych błędów.

## VIII. Rejestr ryzyk

1. ryzyko produktowe:


- interfejs niewygodny dla użytkownika - testy akceptacyjne
- niepełna lub błędna informacja na ekranie - testowanie czarnoskrzynkowe, inspekcja
    kodu
- problemy z wyświetleniem komunikatu
2. ryzyko projektowe:
- zakres prac źle zdefiniowany - szczegółowa inspekcja projektu wysokiego poziomu,
    akceptacja projektu przez klienta;
- niewystarczające zasoby ludzkie - dokładne szacowanie parametrów projektu,
    wykorzystanie wielu technik estymacji, zgłaszanie problemów na bieżąco,
- niejednoznaczne wymagania klienta - ścisły kontakt z klientem, zaangażowanie
    klienta w proces inspekcji.

## IX. Zależności

```
Testy zależne są od następujących czynników:
● Członkowie zespołu - aktywność i umiejętności wymagane do testów;
● Testerzy zewnętrzni - ich aktywność oraz podejście do testów;
● Sprzęt - jego sprawność;
● kod - jego przejrzystość w przypadku poważnych błędów.
```
## X. Zatwierdzenie planu

```
Kierownik Projektu .................., podpis ............................ data.....................
```
