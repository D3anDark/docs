
# Administrator: Konfigurowanie elementów

Po przeczytaniu poprzedniej sekcji z pewnością masz już pomysły na to, jakie elementy chcesz utworzyć. Ale zanim
zacząć tworzyć elementy, ważne jest, aby zrozumieć różne dostępne opcje konfiguracji. Przy odrobinie
kreatywności i wyobraźni, można tworzyć elementy, które są unikalne i dostosowane do motywu i dynamiki serwera.
Poniższe sekcje poprowadzą cię przez proces konfigurowania przedmiotów i używania ich do ulepszania ekonomii serwera.
ekonomię serwera.

## Polecenie /economy backpack add

Polecenie `/economy backpack add <user> <item>` jest narzędziem administracyjnym, które pozwala autoryzowanym użytkownikom na dodawanie przedmiotów
bezpośrednio do plecaka użytkownika. Polecenie to jest przydatne do rozwiązywania problemów, nagradzania użytkowników lub zarządzania specjalnymi wydarzeniami.
Za pomocą tego polecenia można dostarczać przedmioty użytkownikom bez przechodzenia przez zwykły proces pozyskiwania.

## /economy backpack remove Polecenie

Polecenie `/economy backpack remove <user> <item>` umożliwia autoryzowanym użytkownikom usuwanie przedmiotów bezpośrednio z plecaka użytkownika.
użytkownika. Polecenie to może być pomocne w przypadku duplikacji przedmiotów, próśb o usunięcie lub rozwiązywania problemów związanych z określonymi przedmiotami.
z określonymi przedmiotami. Za pomocą tego polecenia można w razie potrzeby usunąć przedmioty z ekwipunku użytkownika.

## /economy backpack clear Polecenie

Polecenie `/economy backpack clear <user>` pozwala autoryzowanym użytkownikom na wyczyszczenie całego plecaka użytkownika, usuwając wszystkie
przedmioty naraz. Komenda ta może być wykorzystana do karania użytkowników lub w sytuacjach, które wymagają zresetowania ekwipunku użytkownika.
zresetowania. Używając tego polecenia, można zapewnić czyste konto dla kolekcji przedmiotów użytkownika. To polecenie jest nieodwracalne,
więc należy jej używać ostrożnie. Zaleca się użycie komendy `/economy backpack remove`, aby usunąć określone przedmioty zamiast
zamiast czyszczenia całego plecaka. Zapobiegnie to przypadkowemu usunięciu przedmiotów i pozwoli rozwiązać problemy bez
bez wpływu na cały ekwipunek użytkownika.

## Utwórz przedmiot

![](../assets/v1.gif)

Przedmioty można tworzyć bezpośrednio z pulpitu nawigacyjnego. Aby utworzyć nowy przedmiot, przejdź do strony "Przedmioty" i kliknij przycisk
plus. Zostaniesz poproszony o wprowadzenie nazwy elementu, typu i innych opcji konfiguracji opisanych poniżej.

## Konfiguracja wyświetlania elementu

![](../assets/v2.png)

### Nazwa elementu

Nazwa przedmiotu. Będzie ona wyświetlana w sklepie i ekwipunku użytkownika.

### Typ przedmiotu

Typ przedmiotu. Określa zachowanie i efekty przedmiotu.

- Jest to domyślny i najprostszy typ przedmiotu,
  którego jedynym celem jest wykonanie jakiejś akcji (zazwyczaj jest to nadanie roli serwera).
  Nie można ustawić go do robienia interesujących rzeczy, takich jak dawanie pieniędzy za pomocą /collect-income, ponieważ jest on używany natychmiastowo
  i nie są zapisywane w plecaku.

- **Zapisz przedmiot w plecaku:** Ten typ przedmiotu jest zapisywany w plecaku użytkownika i może być użyty z komendą /use-item
  . Pozwala to na tworzenie przedmiotów, które mogą być używane wielokrotnie i mają bardziej złożone efekty.

### Sticky

Jeśli opcja ta jest włączona, użytkownik nie będzie mógł zwrócić tego przedmiotu za pomocą komend /give-item lub /market.

### Automatycznie zniszcz ten przedmiot:

Czasami chcesz tworzyć przedmioty dające pewne wzmocnienie przez ograniczony czas. Ta opcja pozwala automatycznie zniszczyć
ten przedmiot po upływie określonego czasu. Na przykład, możesz stworzyć przedmiot, który daje +10% do levelowania przez 24 godziny.

### Ogranicz liczbę przedmiotów w plecaku:

Przydatna funkcja, która pozwala ograniczyć liczbę przedmiotów, które może posiadać jeden użytkownik.

## Konfiguracja sklepu

Podczas tworzenia przedmiotu istnieje możliwość dodania go do sklepu. Sklep jest miejscem, w którym użytkownicy mogą przeglądać i kupować przedmioty
za pomocą wirtualnej waluty. Poniżej znajdują się opcje konfiguracji przedmiotów w sklepie.

- **Wyświetl przedmiot w sklepie:** Włącz to pole wyboru, aby udostępnić przedmiot do zakupu w sklepie.

Jeśli przedmiot zostanie wyświetlony w sklepie, pojawią się następujące opcje:

![](../assets/v3.png)

### Opis przedmiotu

Wprowadź opis przedmiotu, który będzie wyświetlany w sklepie. Podaj informacje o jego efektach lub
specjalnych cechach.

### Cena przedmiotu

Ustaw cenę przedmiotu w sklepie.

### Cena przedmiotu dla poszczególnych ról

Jeśli chcesz zaoferować różne ceny dla określonych ról, możesz ustawić cenę dla każdej roli za pomocą tej opcji. To
Pozwala to na tworzenie zniżek lub promocji dla poszczególnych ról.

### Ogranicz liczbę artykułów w magazynie

Jeśli chcesz ograniczyć dostępność produktu, możesz ustawić limit liczby produktów, które można kupić w sklepie.
w sklepie.

### Kategoria artykułu

Przypisz kategorię do przedmiotu, aby uporządkować swój sklep. Użytkownicy mogą przeglądać przedmioty według kategorii, co ułatwia znalezienie
łatwiej znaleźć to, czego szukają.

![](../assets/v4.png)

### Właściciel przedmiotu

Jeśli chcesz, aby dochód z tej pozycji był rozdzielany między wielu właścicieli, możesz wybrać role lub indywidualnych użytkowników, którzy będą uważani za właścicieli.
użytkowników, którzy będą uważani za właścicieli. Dochód zostanie równomiernie rozdzielony pomiędzy wybranych właścicieli.

### Wymagania dotyczące zakupu przedmiotu

Jeśli chcesz ustawić określone wymagania dla użytkowników, aby mogli zakupić przedmiot, możesz wybrać role lub poszczególnych użytkowników, którzy
indywidualnych użytkowników, którzy muszą spełnić te wymagania. Użytkownicy, którzy nie spełnią tych wymagań, nie będą mogli kupić przedmiotu.
elementu.

### Szansa na oszustwo

Określ procentową szansę, że przedmiot nie zostanie dostarczony użytkownikowi po zakupie. Dodaje to element ryzyka
do zakupu i może stworzyć element zaskoczenia dla użytkowników.

## Konfiguracja zachowania /use-item

Ta część konfiguracji pozwala skonfigurować zachowanie bota po użyciu przedmiotu za pomocą polecenia `/use-item`.

![](../assets/v5.png)

### Zniszcz przedmiot po jego użyciu

Jeśli włączone, przedmiot zostanie usunięty z plecaka użytkownika po jego użyciu.

### Dodawanie tymczasowych ról

Możesz wybrać role, które zostaną tymczasowo dodane do użytkownika po użyciu przedmiotu. Role te zostaną automatycznie usunięte
po upływie określonego czasu.

### Dodaj role

Można wybrać role, które zostaną dodane do użytkownika po użyciu elementu. Role te będą obowiązywać do momentu ich ręcznego usunięcia.

### Usuń role

Wybierz role, które mają zostać usunięte z użytkownika po użyciu elementu. Role te nie będą już powiązane
z użytkownikiem.

### Dodaj pieniądze

Określ kwotę wirtualnej waluty, która zostanie dodana do salda użytkownika po użyciu przedmiotu.

### Dodaj XP

Jeśli korzystasz z systemu XP naszego bota, możesz określić ilość punktów XP, które zostaną dodane do doświadczenia użytkownika po użyciu przedmiotu.
po użyciu przedmiotu.

### Usuń wszystkie ostrzeżenia użytkownika

Włącz tę opcję, aby usunąć wszystkie ostrzeżenia powiązane z użytkownikiem. Może to być przydatne do
może być przydatna do zapewnienia czystego konta lub zresetowania niektórych atrybutów użytkownika.

### Niestandardowa wiadomość po użyciu tego elementu

Wprowadź niestandardową wiadomość, która zostanie wyświetlona użytkownikowi po użyciu elementu.
elementu. Możesz podać dodatkowe instrukcje lub informacje związane z działaniem elementu.
