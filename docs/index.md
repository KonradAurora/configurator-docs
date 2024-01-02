# Konfigurator - instrukcja użytkownika

Niniejsza instrukcja ma na celu pomoc użytkownikom w korzystaniu z konfiguratora służącego do tworzenia złożonych 
i rozbudowanych produktów. <br>
Głównym celem tego rozdziału instrukcji jest dostarczenie informacji umożliwiających szybkie i bezproblemowe korzystanie
z konfiguratora Aurora Creation, dostępnego w postaci modułu Shopware.

W instrukcji znajdziesz kroki oraz informacje, które pomogą Ci stworzyć produkty dostosowane do Twoich potrzeb.

???+ info

    Instrukcja dotyczy wersji konfiguratora **1.0.0** dostępnego dla  **Shopware 6.4.13**

## Wprowadzenie

Konfigurator Aurora Creation jest narzędziem które pozwala na tworzenie bardzo złożonych produktów, składających się
z wielu pomniejszych elementów, wraz z możliwością ich konfiguracji czy personalizacji.
Rozwiązanie to jest uniwersalne i może być wykorzystywane w wielu branżach, w których tworzone są produkty złożone, 
personalizowalne czy konfigurowalne.
Zastosowanie konfiguratora pozwala na proste i szybkie tworzenie takich produktów, skracając czas potrzebny na złożenie
zamówienia, a także eliminując błędy popełniane przy ręcznym składaniu zamówień.<br>
Tworzenie konfiguratora jest proste i intuicyjne, a dostarczone wraz z nim narzędzia pozwalają na szeroką konfigurację
i dokładne dopasowanie do potrzeb klienta.
Konfigurator składa się z kroków które możemy dowolnie dodawać i edytować, a szeroki wybór znajdujących się w nim warunków
pozwala na dokładne określenie jego działania.


<figure markdown>
  ![implementacja](https://i.ibb.co/Zz0kqNh/wstep1.png){ width="800" }
  <figcaption>Implementacja konfiguratora w branży fotograficznej</figcaption>
</figure>

## Zastosowanie

Ze względu na swoją uniwersalność konfigurator może być wykorzystywany w wielu branżach, w których tworzone są produkty
złożone, personalizowalne czy konfigurowalne.<br>
Konfigurator pozwala nam na stworzenie wieloetapowej konfiguracji produktu, w której każdy etap może być dowolnie
konfigurowany i personalizowany. Określane mogą być warunki, które muszą zostać spełnione aby dany etap był dostępny,
a także wymagalność każdego poszczególnego kroku. <br>
Każdy krok ma również wpływ na ostateczną cenę produktu, która jest wyliczana na podstawie wybranych opcji oraz
konfiguracji produktu. <br>

<figure markdown>
  ![implementacja2](https://i.ibb.co/jLwXjXq/wstep2.png){ width="800" }
  <figcaption>Implementacja konfiguratora w branży fotograficznej</figcaption>
</figure>

## Konfiguratory

Moduł konfiguratora dostępny jest z menu Shopware, pod zakładką 'Treści'.<br>
Dodane są tam dwie karty:  <br>

![menu](https://i.ibb.co/ccrZ4Fr/konfigurator1.png){ align=right width="500" }


- **Konfigurator** - zawiera listę wszystkich utworzonych konfiguratorów
- **Elementy konfiguratora** - zawiera listę wszystkich dostępnych elementów, które mogą zostać wykorzystane w konfiguratorach

W karcie **Konfigurator** znajduje się lista wszystkich utworzonych konfiguratorów, oraz przycisk umożliwiający dodanie
nowego konfiguratora. <br>

Karta **Elementy konfiguratora** zawiera listę wszystkich dostępnych elementów, które mogą zostać wykorzystane 
do budowy konfiguratorów, a także przycisk umożliwiający nam dodanie nowego elementu <br>



### Budowa konfiguratora

Z poziomu kartoteki konfiguratorów możemy przejść do edycji poszczególnych konfiguratorów aby zobaczyć i ewentualnie 
zmienić ich ustawienia i konfigurację. <br>

<figure markdown>
  ![konfigurator](https://i.ibb.co/VgvzN11/warunki.png)
</figure>

Budowa konfiguratorów jest bardzo prosta i intuicyjna:   <br>

1. **Kroki** - po lewej stronie ekranu znajduje się lista kroków, które składają się na konfigurator. Klikając na jeden 
z nich możemy przejść do jego ustawień. <br>
2. **Elementy** - po wybraniu kroku oraz przejściu do karty *Elements* możemy zobaczyć listę elementów które znajdują się 
w danym kroku. Jeden krok może mieć wiele elementów, jednak nie wszystkie z nich muszą być widoczne. O wyświetlaniu poszczególnych 
elementów decydują *warunki wyświetlania* określone w każdym elemencie. <br>
3. **Warunki** - każdy element posiada warunki które muszą zostać spełnione aby element został wyświetlony. <br>
4. **Budowa warunku** - warunki składają się z kilku elementów:  
    *  **Step** - określa krok, w którym warunek ma zostać sprawdzony. <br>
    *  **Element** - wskazuje na element którego warunek ma dotyczyć. <br>
    *  **Value** - dotyczy wartości jaką musi przyjąć element <br>
    *  **Condition** - pozwala na wybranie czy wartość musi zostać wybrana aby warunek był spełniony <br>

Każdy krok, oraz poszczególne elementy w zależności od spełnionych warunków, widoczne są w Naszym sklepie. <br>

<figure markdown>
  ![front](https://i.ibb.co/WGrQ44w/konfigurator-front.png)
  <figcaption>Kroki konfiguratora widoczne na sklepie</figcaption>
</figure>

W zależności od wybranych opcji widoczne są kolejne elementy konfiguratora. <br>

<figure markdown>
  ![brak-opcji](https://i.ibb.co/Yk26Jt3/grawer-brak.png){ width="800" }
  <figcaption>Brak wybranej opcji</figcaption>
</figure>

<figure markdown>
  ![wybrana-opcja](https://i.ibb.co/yqpw55g/grawer-wybrany.png){ width="800" }
  <figcaption>Wybrana opcja grawerowania</figcaption>
</figure>


### Elementy konfiguratora

Z poziomu kartoteki elementów konfiguratorów możemy przejść do edycji poszczególnych elementów konfiguratorów które mogą 
zostać przypisane do poszczególnych kroków. <br>
Element konfiguratora może być prostym formularzem z przyciskami do wyboru odpowiednich wartości, ale mogę to być również 
bardziej złożone pola pozwalające na wprowadzanie własnych wartości, bądź po prostu uwagi dla klienta wyświetlające się 
po spełnieniu odpowiednich warunków. <br>

<figure markdown>
  ![elementy](https://i.ibb.co/pZqftpN/elementy.png){ width="800" }
  <figcaption>Różne typy elementów</figcaption>
</figure>

Na powyższym zdjęciu przedstawione są elementy:  <br>
1. **Warning** - wyświetlający uwagę dla klienta dotyczącą danego kroku czy elementu <br>
2. **Button** - pozwalający na dokonanie wyboru opcji w formie przycisków <br>
3. **Text field** - służący do wprowadzania własnych wartości przez klienta<br>


Po wybraniu konfiguratora z kartoteki elementów, oraz przejściu do jego edycji zobaczymy poniższe opcje:   <br>

<figure markdown>
  ![elementykonfiguratora](https://i.ibb.co/tqHMtxM/elementkonfiguratora.png)
  <figcaption>Edycja elementu konfiguratora</figcaption>
</figure>


Na powyższym zdjęciu przedstawione są elementy:  <br>
1. **Główne** - karta zawierająca główne informacje o elemencie, takie jak jego nazwa, nazwa wyświetlana na sklepie, opis
 czy zdjęcie. <br>
2. **Dostępne komponenty** - lista komponentów które mogą zostać dodane do danego elementu <br>
3. **Lista komponentów** - zawierająca aktualnie przypisane i skonfigurowane dla danego elementu komponenty<br>
4. **Konfiguracja komponentu** - widoczna po wybraniu jednego z komponentów konfiguracja opisująca dane komponent, jego 
wyświetlanie się na sklepie, oraz wpływ na końcową cenę produktu. <br>


### Komponenty

Narzędzie konfiguratora dostarcza Nam kilka komponentów które pozwalają Nam na skonfigurowanie i przygotowanie Naszych elementów. <br>

<figure markdown>
  ![komponenty](https://i.ibb.co/sbFMbvC/dostepnekomponenty.png)
  <figcaption>Dostępne komponenty</figcaption>
</figure>

Na powyższym zdjęciu przedstawione są elementy:  <br>
1. **Button** - pozwalający na wybranie wartości w formie przycisku, przypisanie każdej z opcji ceny czy dodanie obrazka. 
<figure markdown>
   ![imagebutton](https://i.ibb.co/LnbrNnp/buttons.png){ width="600" }
</figure> <br> 
2. **Numeric input** - pole pozwalające na wybranie wartości liczbowej, odpowiadające np. ilości elementów. Konfiguracja
   pozwala również na określenie minimalnej oraz maksymalnej wartości którą można wybrać, ilość darmową, oraz cenę jednstkową
   za każdą kolejną sztukę.  <br>
<figure markdown>
  ![numeric1](https://i.ibb.co/1XHZCZQ/numeric.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure>
<figure markdown>
  ![numeric2](https://i.ibb.co/jhHYPxZ/numeric2.png){ width="600" }
<figcaption>Konfiguracja</figcaption>
</figure> <br>
3. **Input** - pozwalający na wpisywanie własnych wartości przez klienta. Od strony konfiguracji pozwala na dodanie wyrażenia
regularnego określającego co może zostać wpisane, oraz minimalną i maksymalną długość tekstu.<br>
<figure markdown>
  ![input1](https://i.ibb.co/6ndYdN2/text.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure>
<figure markdown>
  ![numeric2](https://i.ibb.co/4sfYkXk/text2.png){ width="600" }
<figcaption>Konfiguracja</figcaption>
</figure><br>
4. **File upload** - pole pozwalające na dodanie przez klienta własnych plików. <br>
<figure markdown>
  ![file1](https://i.ibb.co/k6mCH3S/file.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure><br>
5. **Text field** - komponent pozwalający na dodanie pole z tekstem które zostanie wyświetlone na sklepie. <br>
6. **Product** - pozwala na dodanie komponentu odpowiadającego całemu produktowi. Mogą to być kolejne sztuki właśnie 
konfigurowanego produktu, z taką samą konfiguracją. <br>
<figure markdown>
  ![dobor1](https://i.ibb.co/MCYDpbP/dobor.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure><br>
7. **Font** - pozwala na dodanie komponentu odpowiadającego wyborowi czcionki. <br>
<figure markdown>
  ![font11](https://i.ibb.co/w01yDz2/font.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure><br>
8. **Font preview** - pozwala na dodanie komponentu odpowiadającego podglądowi wybranej czcionki. <br>
<figure markdown>
  ![font21](https://i.ibb.co/7zYM0WL/font2.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure><br>
9. **Warning** - pozwala na dodanie komponentu odpowiadającego wyświetleniu uwagi dla klienta. 
<figure markdown>
  ![font21](https://i.ibb.co/74GrzWH/warning.png){ width="600" }
<figcaption>Widok na sklepie</figcaption>
</figure><br><br>
10. **Dodatkowe komponenty** - w zależności od potrzeb na zamówienie mogą dodać dodatkowe komponenty, z własną, wyjątkową 
funkcjonalnością. Przykładowo mogą to być komponenty działające wraz z zewnętrznymi integracjamii. <br>

## Przykłady

Lorem ipsum dolor sit amet, consectetur adipiscing elit.