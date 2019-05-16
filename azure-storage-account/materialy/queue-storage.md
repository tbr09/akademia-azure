# Queue storage

Kolejną usługą jest Azure Queue Storage, która jest po prostu kolejką FIFO \(First In First Out\). Kolejki są najczęściej używane do przesyłania wiadomości pomiędzy serwisami lub tworzenia kolejek mailingowych.

Tworzenie usługi odbywa się identycznie jak dwie poprzednie. Przechodzimy do panelu głównego Storage Account i wybieramy usługę Queues.

![](../../.gitbook/assets/image29.png)

Tworzymy nową kolejkę wybierają Queue.

![](../../.gitbook/assets/image30.png)

Następnie nadajemy kolejce nazwę i zatwierdzamy OK.

![](../../.gitbook/assets/image31.png)

Przechodzimy do nowo stworzonej kolejki.

![](../../.gitbook/assets/image32.png)

Tworzymy nową wiadomość, wpisujemy tekst oraz definiujemy czas wygaśnięcia. Elementy w kolejkach mają swój czas życia, który określa ile czasu wiadomość będzie czekała na odebranie – po minięciu określonego czasu wiadomość zostanie usunięta z kolejki.

![](../../.gitbook/assets/image33.png)

W przypadku, gdy chcemy przekazywać bardziej złożone obiekty niż zwykły tekst, możemy wrzucić obiekt w formacie JSON, następnie z poziomu odbierającego serwisu odebrać i przekonwertować dane.

![](../../.gitbook/assets/image34.png)

