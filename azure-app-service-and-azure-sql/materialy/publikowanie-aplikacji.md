# Publikowanie aplikacji na App Service

W ramach tego tutoriala wykorzystamy prostą aplikację internetową typu todolist.

Można ją pobrać jako .zip z [https://github.com/adamskibicki/dotnet-sqldb-tutorial/archive/master.zip](https://github.com/adamskibicki/dotnet-sqldb-tutorial/archive/master.zip)

lub można sklonować repozytorium git: [https://github.com/adamskibicki/dotnet-sqldb-tutorial.git](https://github.com/adamskibicki/dotnet-sqldb-tutorial.git)

Następnie otwieramy plik solucji \(z rozszerzeniem .sln\) pobranej aplikacji.

![](../../.gitbook/assets/image%20%2819%29.png)

A następnie uruchamiamy ją przyciskiem na górze.

![](../../.gitbook/assets/image%20%2863%29.png)

Aby opublikować naszą aplikację z poziomu Visual Studio, w oknie Solution Explorer klikamy prawym przyciskiem na nasz projekt i wybieramy opcję Publish.

![](../../.gitbook/assets/image%20%2853%29.png)

![](../../.gitbook/assets/image%20%28104%29.png)

W nowo otwartym oknie w VS wybieramy opcję Start.

![](../../.gitbook/assets/image%20%283%29.png)

Następnie wybieramy opcję Imort profile i wskazujemy plik pobrany pod koniec poprzedniej części tutoriala \(publish profile dla wcześniej utworzonego App Service'u\).

![](../../.gitbook/assets/image%20%2812%29.png)

Publikowanie powinno rozpocząć się automatycznie i po jakimś czasie powinniśmy zobaczyć naszą aplikację.

![](../../.gitbook/assets/image%20%2844%29.png)

Błąd, który widzimy spowodowany jest ostatnim brakującym elementem naszej aplikacji - bazą danych, którą zajmiemy się w następnej części tej lekcji.

