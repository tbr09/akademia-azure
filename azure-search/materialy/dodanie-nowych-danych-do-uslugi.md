# Dodanie nowych danych do usługi

* Wykonanie skryptu SQL znajdującego się w folderze SQL -&gt; NewData.sql, który dodaje nowe dane do bazy

![](../../.gitbook/assets/image%20%2847%29.png)

* Uruchomienie indeksera, który wciąga dane z naszej bazy do indeksu usługi Search

Musimy teraz uruchomić nasz indekser, aby wciągnąć nowe dane do naszego indeksu z bazy danych. Przechodzimy do portalu i w podsumowaniu usługi Searcha klikamy Indexers

![](../../.gitbook/assets/image%20%2882%29.png)

Wybieramy indexer, który nas interesuje

![](../../.gitbook/assets/image%20%2841%29.png)

Wybieramy opcję Run

![](../../.gitbook/assets/image%20%28101%29.png)

Po odświeżeniu strony lista wywołań indeksera powinna powiększyć się o 1

![](../../.gitbook/assets/image%20%2869%29.png)

Jeżeli mamy komunikat o sukcesie, nasze dane powinny zostać wciągnięte do indeksu.

* Wykonanie zapytania, sprawdzającego, czy wszystkie dane zostały wciągnięte

Przechodzimy po raz kolejny do Search Explorer

![](../../.gitbook/assets/image%20%2849%29.png)

Wpisujemy zapytanie, zawierające dane dotyczące nowych rekordów dodanych do naszej bazy. Wyszukamy artykuły po słowie New

![](../../.gitbook/assets/image%20%2887%29.png)

Rekordy zostały zwrócone, wszystko działa tak, jak powinno.

