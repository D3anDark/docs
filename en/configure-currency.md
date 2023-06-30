
# Konfigurowanie waluty

![](../assets/v19.gif)

Każdym użytkownikiem można zarządzać indywidualnie za pomocą poleceń wymienionych poniżej. Polecenia te umożliwiają dostosowanie
saldo walutowe określonego użytkownika, co może być przydatne do celów administracyjnych lub do nagradzania użytkowników za ich
użytkowników za ich wkład w serwer.

## /economy add <użytkownik> <ilość pieniędzy> [lokacja przelania]

Komenda `/economy add` jest komendą administracyjną, która pozwala autoryzowanym użytkownikom na dodawanie wirtualnych pieniędzy do konta określonego użytkownika.
konto użytkownika. Wspominając lub podając identyfikator docelowego użytkownika i określając kwotę, która ma zostać dodana,
administratorzy mogą odpowiednio dostosować salda użytkowników. Opcjonalny argument `lokalizacja przelania` może być dostarczony w celu określenia, czy
pieniądze powinny zostać dodane do banku lub portfela. Domyślnie do banku.

## /economy remove <użytkownik> <ilość pieniędzy> [lokalizacja przelania]

Komenda `/economy remove` umożliwia autoryzowanym użytkownikom odejmowanie wirtualnych pieniędzy z konta konkretnego użytkownika. Poprzez
lub podając identyfikator docelowego użytkownika i określając kwotę do usunięcia, administratorzy mogą odpowiednio dostosować
odpowiednio dostosować salda użytkowników. Opcjonalny argument `lokalizacja przelania` może być podany w celu określenia, czy pieniądze powinny być
potrącane z banku lub portfela. Domyślnie z banku.

## /economy set <użytkownik> <ilość pieniędzy> [lokalizacja przelania]

Komenda `/economy set` pozwala autoryzowanym użytkownikom na ustawienie określonej kwoty wirtualnych pieniędzy dla konta użytkownika. Poprzez
podając identyfikator docelowego użytkownika i określając żądane saldo, administratorzy mogą bezpośrednio modyfikować salda użytkowników.
mogą bezpośrednio modyfikować salda użytkowników. Opcjonalny argument `lokalizacja przelania` może być podany w celu określenia, czy pieniądze 
powinny być ustawione w banku lub portfelu. Domyślnie w banku.

## Ustawienia serwera

![](../assets/v9.png)

### Symbol waluty

Symbol waluty jest wizualną reprezentacją wirtualnej waluty używanej w systemie ekonomicznym bota. Jest on wyświetlany
w różnych poleceniach i komunikatach, aby zapewnić użytkownikom wyraźne wskazanie używanej waluty. Domyślnym
symbol waluty to `$`, ale można go zmienić na dowolny wybrany emoji.

### Początkowa kwota pieniędzy

Początkowa kwota pieniędzy to ilość wirtualnej waluty, którą użytkownicy otrzymają po pierwszym dołączeniu do serwera.
Zapewnia to użytkownikom punkt wyjścia do zaangażowania się w system ekonomiczny i zarabiania większej ilości pieniędzy za pomocą różnych poleceń i działań.
i działania.

Należy pamiętać, że to ustawienie dotyczy tylko nowych użytkowników, którzy dołączają do <serwera po zmianie ustawienia. Istniejący użytkownicy
nie otrzymają początkowej kwoty pieniędzy. Można jednak użyć polecenia `/economy add`, aby ręcznie dodać pieniądze do kont istniejących użytkowników.
istniejących kont użytkowników.

### Resetowanie pieniędzy użytkownika po opuszczeniu serwera

To ustawienie określa, czy wirtualne pieniądze użytkowników będą resetowane po opuszczeniu serwera. Jeśli to ustawienie jest
włączone, użytkownicy stracą wszystkie swoje wirtualne pieniądze po opuszczeniu serwera. Może to być przydatne do zniechęcania użytkowników.
do opuszczenia serwera, ponieważ stracą oni wszystkie swoje postępy w systemie ekonomicznym.

### Separator grup cyfr

Separator grup cyfr to wizualny separator, który służy do rozdzielania cyfr na grupy po trzy. Zapewnia to
bardziej przejrzystą reprezentację dużych liczb i ułatwia użytkownikom odczytanie i zrozumienie kwoty pieniędzy, którą
pieniędzy.

### Pozycja walutowa

Pozycja waluty określa miejsce wyświetlania symbolu waluty w wiadomościach. Domyślnym ustawieniem jest `po
po prawej stronie`, co oznacza, że symbol waluty będzie wyświetlany po kwocie pieniędzy. Można również zmienić
na `po lewej`, co spowoduje wyświetlanie symbolu waluty przed kwotą pieniędzy.
