# Azure SQL Database

Teraz stwórzmy naszą bazę danych i połączmy ją z naszą aplikacją.

Wejdźmy na portal Azure i stwórzmy nową usługę SQL Database.

![](../../.gitbook/assets/image%20%2841%29.png)

![](../../.gitbook/assets/image%20%2822%29.png)

W formularzu wybieramy subskrypcję, grupę zasobów i nazwę naszej bazy danych. Następnie mamy do wyboru serwer. Wybieramy pow nim opcję Create new.

W formularzu po prawej stronie wypełniamy wszytkie pola: nazwę serwera, dane admina \(to tymi danymi będziem logować się do usługi Azure SQL Server, którą tworzymy\), lokalizację. Jest tu też checkbox Allow Azure services to access server, który zostawiam zaznaczony. Następnie na dole klikamy Select.

![](../../.gitbook/assets/image%20%2833%29.png)

W ramach jednej usługi Azure SQL Server można mieć wiele baz danych \(usługa Azure SQL Database\).

Wracając do formularza z naszą bazą danych. Mamy tu opcję Compute + Storage, która określa tier naszej bazy danych \(cena, wielkość i dostępne zasoby\). Wybieramy opcję Configure Database.

![](../../.gitbook/assets/image%20%2849%29.png)

Teraz mamy do wyboru opcje dotyczące warstwy cenowej naszej bazy danych. Po prawej można zobaczyć ile zapłacimy za miesiąc działania naszej bazy danych. Wybieramy tier Basic i ustawiamy wielkość bazy na 100 MB oraz zatwierdzamy Apply.

![](../../.gitbook/assets/image%20%2823%29.png)

Następnie w formularzy wybieramy Create + Review, aby zobaczyć podsumowanie naszej usługi. 

![](../../.gitbook/assets/image%20%287%29.png)

Teraz wybieramy Create, aby w końcu stworzyć bazę danych.

![](../../.gitbook/assets/image%20%2840%29.png)

Po utworzeniu bazy danych znajdujemy ją w naszej grupie zasobów. Możemy tu zobaczyć podsumowanie naszej usługi i dostępne opcje konfiguracyjne. Nas interesuje zakładka Connection strings po prawej.

![](../../.gitbook/assets/image%20%2836%29.png)

Po wejściu w nią kopiujemy naszego connection string zamieniając w nim fragmenty {your\_username} na nazwę admina stworzonej wcześniej usługi SQL Server i {your\_password} na hasło, które wcześniej ustawiliśmy. Tak spreparowany connection string zapisujemy sobie w bezpiecznym miejscu - będzie nam za chwilę potrzebny.

![](../../.gitbook/assets/image%20%2817%29.png)

Teraz wracamy do naszej usługi App Service i znajdujemy zakładkę Configuration.

![](../../.gitbook/assets/image%20%288%29.png)

Wybieramy tu opcję New connection string i w otwartym formularzu jako Name podajemy MyDbConnection, jako Value - przygotowany wcześniej connection string, a jako Type - SQL Server i klikamy Update.

![](../../.gitbook/assets/image%20%2815%29.png)

Następnie na górze wybieramy opcję Save.

![](../../.gitbook/assets/image%20%2842%29.png)

Teraz nasza aplikacja powinna działać już poprawnie.

![](../../.gitbook/assets/image%20%2847%29.png)



