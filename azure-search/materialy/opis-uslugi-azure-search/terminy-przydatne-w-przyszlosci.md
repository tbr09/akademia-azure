# Terminy przydatne w przyszłości

·         Suggester – narzędzie umożliwiające stworzenie autocomplete, z którego możemy korzystać w aplikacji

·         Scoring profile – ocena przypisana dla danego pola indeksu, najlepiej będzie zrozumieć to na przykładzie: Mamy indeks, w którym znajdują się artykuły. Indeks ma dwa pola: tytuł i zawartość. Chcemy wyszukiwać po obydwu z nich, ale chcemy aby tytuł był ważniejszy. Tworząc scoring profile ustawiamy wagi danym polom. Załóżmy, że pole tytułu dostanie wagę 10 a pole zawartości wagę 3. W momencie wyszukiwania wyżej będą się znajdować rekordy, w których wyszukiwana fraza znalazła się w tytule.

W takim przypadku rekord, w którym w zawartości wystąpi wyszukiwana fraza 4 razy wyprzedzi rekord, w którym fraza wystąpiła raz w tytule \(jeżeli w scoring profile ustawimy funkcję sumy do pozycjonowania -&gt; 10 &lt; 4\*3\).

·         OCR – optyczne rozpoznawanie znaków, możliwe do wybrania, gdy pracujemy z plikami i chcemy zczytywać znaki ze zdjęć

