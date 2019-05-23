# Praca z kodem

### Uruchomienie aplikacji znajdującej się w folderze AzureSearchWorkshopsDemo

Jest to aplikacja MVC Core, w której stworzono prosty model wyszukiwarki.

Omówienie bloków kodu:

* HomeController.cs -&gt; kontroler, który zawiera całą logikę programu.

![](../../.gitbook/assets/image%20%2837%29.png)

Konstruktor kontrolera wraz z niezbędnymi właściwościami i obiektami do połączenia się z usługą. Obiekt typu SearchServiceClient służy do połączenia się z usługą, natomiast ISearchIndexClient umożliwia połączenie się z indeksem w celu wyszukiwania. Obiekty te są udostępniane przez nuget Microsoft.Azure.Search.

Uwaga: apiKey, który obecnie jest ustawiony jako ”PLACEHOLDER” należy skopiować z naszej usługi. Zakładka klucze -&gt; Primary Key \(zdjęcie poniżej\)

![](../../.gitbook/assets/image%20%2849%29.png)

Metoda Search odpowiada za wyszukiwanie, przyjmuje ona parametr query, czyli zapytanie, które do niej wysyłamy. Wysyłamy do  niej obiekt SearchParameter, w którym definiujemy filtry, wybieramy dane, które chcemy zwrócić, itd. W tym przykładzie nie będę pokazywał wszystkich przykładów wykorzystania. Zostawiam to Tobie do przetestowania/zabawy. Jedynym parametrem, który jest ustawiany jest QueryType. Odpowiada on za sposób wyszukiwania. Gdy jest on ustawiony na Full umożliwia wyszukiwanie podobnych słów.

Następnie używamy naszego klienta do wykonania zapytania. Metoda Search klienta przyjmuje wyszukiwaną frazę oraz zdefiniowany wcześniej obiekt searchParameters.

Wyszukiwanie podobnych słów jest możliwe po dodaniu ~1 do każdego ze słów. Wtedy wyszukujemy słowa, które mogą się różnić jedną literą \(maksymalna wartość po ~ to 2\).

![](../../.gitbook/assets/image%20%2826%29.png)

Wyniki, które otrzymujemy są typem słownikowym, więc aby je wypisać, musimy je zdeserializować w taki sposób, aby otrzymać z nich obiekt. Metoda przechodzi przez wszystkie wyniki i wyciąga z nich interesujące nas dane.

![](../../.gitbook/assets/image%20%2824%29.png)

I ostatnia metoda kontrolera, która wywołuje opisane wcześniej metody. Otrzymuje ona z formularza zapytanie, które jest wysyłane do naszej usługi, a następnie zwraca otrzymane dane do widoku.

![](../../.gitbook/assets/image%20%2875%29.png)

Uwaga! Jeżeli chciałbyś/chciałabyś stworzyć własną aplikację w .Necie pamiętaj o wykorzystaniu nugeta Microsoft.Azure.Search

