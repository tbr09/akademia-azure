# Mechanizm wyszukiwania

Dodajemy dane do naszej usługi -&gt; tworzymy:

* źródło danych, z którego będziemy czerpać dane do wyszukiwania, 
* indeks, który będzie przechowywać dane do wyszukiwania,
* indekser, który będzie ściągać dane z naszej bazy do indeksu

Aby to zrobić, klikamy Import data

![](../../.gitbook/assets/image%20%2823%29.png)

Przy połączeniu się z bazą danych wybieramy opcję Azure SQL Database

![](../../.gitbook/assets/image%20%2878%29.png)

Wybieramy istniejącą bazę jak na rysunku poniżej

![](../../.gitbook/assets/image%20%2861%29.png)

Wpisujemy nazwę naszego zródła i wpisujemy hasło, zdefiniowane podczas tworzenia serwera. Następnie klikamy Test connection

![](../../.gitbook/assets/image%20%285%29.png)

Gdy wszystkie dane są poprawne wyskakuje nam kolejna opcja do wyboru, mianowicie nazwy tabel lub widoków znajdujących się w naszej bazie. My mamy tylko jedną tabelę \(Article\). Wybieramy ją i przechodzimy dalej.

![](../../.gitbook/assets/image%20%2856%29.png)

Kolejny krok to wykorzystanie Cognitive Services do obsługi Searcha. Dzięki temu możemy wyłapywać różne ciekawe rzeczy w naszej wyszukiwarce typu nazwy organizacji w tekście lub imiona i nazwiska osób. Pomijamy ten krok, nie mamy jeszcze wiedzy o Cognitive Services. Warsztaty ukazują podstawowe możliwośi usługi. Klikamy Skip to: Customize target index.

![](../../.gitbook/assets/image%20%2829%29.png)

W tym kroku definiujemy nasz index, który będzie zawierał dane z naszej bazy. Nadajemy mu unikalną nazwę w przestrzeni naszej usługi, wybieramy pole, które ma być kluczem. Musi być ono unikalne dla każdego rekordu, więc najlepiej jest wybrać pole Id, które jest kluczem głównym tabeli. Następnie mamy pole Suggester name oraz Search mode. Na tych warsztatach nie będziemy z niego korzystać. W skrócie służy ono do stworzenia autocomplete.

W ostatnim kroku definiujemy pola naszego indeksu. Są one domyślnie mapowane z naszej tabeli bazy danych. Ponadto każde z nich ma swój własny typ, który również jest zmapowany na podstawie bazy \(pole klucza indeksu jest zawsze mapowane na String\). Po prawej stronie mamy do wyboru to, co będziemy mogli zrobić z każdym polem w naszej wyszukiwarce.

* Retrievable – czy pole ma być przetwarzane/wyświetlane w wyszukiwarce
* Filterable – czy dane pole będzie mogło być filtrowane
* Sortable – czy po danym polu będzie można sortować
* Facetable – czy będzie można sprawdzać ilość rekordów o danej wartości kolumny
* Searchable – czy po danym polu można wyszukiwać

Na potrzeby warsztatów wybieramy wszystkie opcje i przechodzimy do następnego kroku -&gt; stworzenia indeksera.

![](../../.gitbook/assets/image%20%2855%29.png)

Aby stworzyć indekser wpisujemy jego nazwę, która musi być unikalna w obrębie usługi. Następnie wybieramy częstotliwość jego uruchamiania -&gt; co ile czasu ma ściągać dane z naszej bazy danych do indeksu. W naszym przypadku wybieramy opcję Once. W trakcie trwania warsztatów będziemy go uruchamiać samodzielnie.

![](../../.gitbook/assets/image%20%2851%29.png)

Klikamy opcję dodania indeksera na dole strony i gotowe, nasze dane zostały pobrane do indeksu. Możemy wyszukiwać.

![](../../.gitbook/assets/image%20%2854%29.png)

