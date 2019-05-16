# Połączenie Blob Storage z aplikacją

Przejdziemy teraz do połączenia jednej z omawianych usług z przykładową aplikacją webową. Wybrana usługa to Blob ze względu na jej popularność i częste wykorzystanie w tego typu aplikacjach.

Pobieramy/klonujemy kod aplikacji z GitHuba: [https://github.com/tbr09/AzureStorageWorkshops](https://github.com/tbr09/AzureStorageWorkshops)

Otwieramy solucję \(AzureStorage.sln\) w Visual Studio 2017+ lub Visual Studio Code. Nastepnie w oknie Solution Explorer otwieramy plik appsettings.json.

![](../../.gitbook/assets/image35.png)

W pliku mamy dostępne ustawienia niezbędne do połączenia aplikacji z usługą.

![](../../.gitbook/assets/image36.png)

Wprowadzamy Connection String do którego mamy dostęp w sekcji Access keys w Portalu Azure.

![](../../.gitbook/assets/image37.png)

![](../../.gitbook/assets/image38.png)

Następnie uruchamiamy aplikację.

![](../../.gitbook/assets/image39.png)

Po uruchomieniu aplikacji zostanie otwarte okno przeglądarki z naszą aplikacją, przechodzimy do zakładki Avatars \(Blob\), następnie do formularza dodawania Add new.

![](../../.gitbook/assets/image40.png)

Wybieramy plik z dysku do wgrania i zatwierdzamy Upload file.

![](../../.gitbook/assets/image41.png)

Po wgraniu pliku zostaniemy przekierowani do listy, gdzie możemy sprawdzić czy plik wgrał się poprawnie. Inną opcją na sprawdzenie wgrania pliku jest po prostu przejście do programu Azure Storage Explorer.



