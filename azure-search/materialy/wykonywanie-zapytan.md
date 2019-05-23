# Wykonywanie zapytań

Przechodzimy do narzędzia Search Explorer umożliwiającego wykonywanie zapytań z poziomu portalu Azure

![](../../.gitbook/assets/image%20%2884%29.png)

Widzimy teraz pole Query string, w który definiujemy nasze zapytanie. Gdy nie wpiszemy nic, traktowane jest to jako wyszukaj wszystko.

![](../../.gitbook/assets/image%20%2895%29.png)

Kolejne zapytanie będzie zawierało tylko tekst wyszukiwania. Wpisujemy lorem w miejscu wyszukiwania

![](../../.gitbook/assets/image%20%2868%29.png)

W kolejnym zapytaniu dołączymy ilość zwróconych wyników pasujących do zapytania. Zapytanie będzie wyglądało następująco: lorem&$count=true \(Uwaga! Przy dodaniu każdego nowego parametru wyszukiwania należy dodać &$\)

![](../../.gitbook/assets/image%20%286%29.png)

Kolejne zapytanie zwróci artykuły, których ocena jest mniejsza bądź równa 4. Skorzystamy z opcji filter używając parametru less equal -&gt; &$filter=Rating le 4

![](../../.gitbook/assets/image%20%2828%29.png)

