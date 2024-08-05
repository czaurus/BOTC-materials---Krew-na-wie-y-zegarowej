## Cel & problem.

Celem jest utworzenie tzw. Skryptu (aka. Scenariusza, tj. Spisu postaci) w języku polskim.  
Czyli tego papierka, który gracze mają przy sobie w trakcie gry, by móc podglądać jakie postacie są (lub mogą być) w grze.

Istnieje oficjalne narzędzie, które umożliwia tworzenie własnych skryptów - działa ono jednak tylko w języku angielskim.

## Rozwiązania

### Można, ale po co w ten sposób...

Najprostrzym, ale i najbardziej pracochłonnym rozwiązaniem wydaje się być utworzenie "od zera" własnego skryptu w formie np. tabelki w jakimś Wordzie czy innym OpenOffice'owym Writer'rze.  
Podejście takie ma kilka wad, o których nie chce mi się tutaj pisać.  
(Wyliczając na szybko: Podatność na stworzenie literówek/błędów; Żmudność pracy; Po co, skoro już ktoś to zrobił? ; Przy tworzeniu własnych skryptów: Brak automatycznego wykrywania/oznaczania tzw. Jinx'ów)

### Rozwiązanie właściwe

Społeczność utworzyła sporo dodatkowych narzędzi, które umożliwiają w miarę szybkie osiągnięcie wyżej opisanego celu.
Wymaga to jednak trochę wyklikiwania na kilku różnych stronach.
Dodatkowo problematyczna jest obsługa polskich znaków.
Połowa poniższej instrukcji będzie dotyczyć właśnie problemu znaków diaktrycznych (Tj. polskich znaków).
Osiągnięcie efektu, gdzie np. opis postaci wygląda tak "Kazdej nocy dowiadujesz sie, ktorzy gracze moga (...) " jest stosunkowo proste.

#### W skrócie:

1. Stwórz skrypt, zapisz do JSON. www.script.bloodontheclocktower.com
2. Użyj strony (https://botc-scripts.azurewebsites.net/), żeby przetłumaczyć plik JSON.
   - upload
   - download w języku polski (https://botc-scripts.azurewebsites.net/)
3. popraw ewentualne błędy tłumaczeń i polskie znaki.
4. Użyj www.pocketgrimoire.co.uk
   - Select Edition > custom Script > "paste from clipboard"
   - "character sheet"
   - ctrl+p, 87%

#### Szczegółowo Co i jak, krok po kroku:

1. Trzeba skorzystać z oficjalnego narzędzia do tworzenia własnych (Tzw. customowych) skryptów (www.script.bloodontheclocktower.com). Efekty zapisać w formie pliku JSON.
2. Wytworzony w ten sposób JSON jest w języku angielskim (oficjalna strona działa wyłącznie w języku angielskim.)
3. Przedmiotowego JSON'a upload'ujemy na stronę, gdzie ludzie wrzucają swoje skrypty (https://botc-scripts.azurewebsites.net/)
4. Potem możemy ten sam plik pobrać używając opcji wybrania określonego języka (Button "Download JSON" -> menu rozwijane: "polski (Polska)").  
   Na tym etapie następuje automatyczne tłumaczenie.
5. Tłumaczenie odbywa się na podstawie tego pliku https://docs.google.com/spreadsheets/d/183HMp4ZgslxA4NtFVTXhY3xAbg7FIXZdmVnh9-4A_14/edit?gid=1563258844#gid=1563258844 - zakładka "pl_PL".
   Nie posiadam danych jak często następuje synchronizacja narzędzi a poprzedniego punktu z niniejszym plikiem z google-docs. Możliwe, że po prostu ktoś musi zatwierdzić zmiany z pliku google-docs, nie znam się.
6. Pobrany JSON będzie opisy postaci w języku polskim. Najprawdopobniej jednak zabraknie w nim polskich znaków. Te trzeba uzupełnić ręcznie, acz polecam do tego użyć jakiegoś narzędzia. Pierwsze z brzegu, które działa: spolszcz.pl
7. JSON w języku polskim, z poprawionymi polskimi znakami wrzucamy na tzw "grymuar online" tutaj: https://www.pocketgrimoire.co.uk/en_GB/

8. W grymuarze online Button "Select Edition" (na górze strony), sekcja "custom script";
   Opcje "Upload custom script" (tj. wskazanie pliku źródłowego, tj. naszego "spolszczonego JSON'a") oraz "Enter a URL" (tj. wskazania takiego pliku w internetach) najprawdopodbniej nie zadziałają. Wyskoczy komunikat typu "nie rozpoznano pliku/skryptu". Powodem jest to, że pod względem technicznym polskie znaki są bardzo specyficzne i przedmiotowa strona nie obsługuje ich na poziomie plików JSON (walidator nie dziła).
9. ...Dlatego - ciągle będąc w sekcji "custom script" wybieramy opcję trzecią, tj. "Paste from clipboard". Tutaj trzeba wkleić ręcznie całą zawartość pliku JSON.
10. Klimamy przycisk "Select".
11. Teraz dane powinny być już zaczytane.

12. Teraz trzeba znaleźć przycisk "Character Sheet". (Jest na górze strony, obok przycisku "Select Edition" (z pkt 8.))
    Po kliknięciu pojawi się kod QR. Robimy dwuklik lewym przyciskiem myszy na ten kod QR.
13. Powinna wyświetlić się strona, na której będą wypisane opisy wszystkich postaci w języku polskim (oraz z polskimi znakami).
14. Dla znających podstawy podstaw HTML: ctrl+shift+c pozwala na ostatnie poprawki (trafią do druku/pdf)
15. W celu utworzenia pdf: ctrl+P, odpowiednie ustawienia "zapis jako pdf", skala (prawdopodobnie 87%, żeby zmieściło się na jednej stronie).  
    (Przeprowadzone na chrome, v. 127)
16. U mnie działa :)

Załączam screeny obrazujące powyższe instrukcje.
