# Przygotowanie do stworzenia usługi

1. Należy sklonować  repozytorium, z którego będziemy korzystać: git clone [https://github.com/swislockikacper/AzureSearchWorkshops.git](https://github.com/swislockikacper/AzureSearchWorkshops.git)
2. Logowanie do bazy danych, z której korzystamy na potrzeby warsztatów

* Przechodzimy do panelu stworzonej wcześniej bazy danych i kopiujemy connection string, aby się z nią połączyć

![](../../.gitbook/assets/image%20%2846%29.png)

![](../../.gitbook/assets/image%20%2858%29.png)

* Uruchamiamy program Microsoft SQL Management Studio i wpisujemy dane do połączenia z naszą bazą. Login i Password są danymi uzupełnianymi podczas tworzenia serwera.

![](../../.gitbook/assets/image%20%28101%29.png)

Uwaga! W przypadku, gdy wyświetlony jest poniższy komunikat należy wrócić do portalu Azure i ustawić adresy IP, dla których nasza baza danych będzie dostępna.

![](../../.gitbook/assets/image%20%28103%29.png)

Aby ustawić wspomniane wcześniej adresy należy przejść do panelu naszej bazy danych \(nie serwera\) i kliknąć przycisk Set server firewall

![](../../.gitbook/assets/image%20%2885%29.png)

Na poniższym zdjęciu ustawiono maksymalny zakres adresów. Jest to ustawione na potrzeby warsztatów. Nie zaleca się robienia takich rzeczy produkcyjnie.

![](../../.gitbook/assets/image%20%2861%29.png)

W Microsoft SQL Server Management Studio klikamy kolejny raz Connect i mamy dostęp do naszej bazy, jak na poniższym zdjęciu.

![](../../.gitbook/assets/image%20%2813%29.png)



3. Wykonanie skryptu SQL znajdującego się w folderze SQL -&gt; Create.sql, który tworzy strukturę bazy danych oraz wstawia tam początkowe dane

Klikamy prawym przyciskiem na naszą bazę danych i wybieramy opcję New Query. Następnie kopiujemy kod z pliku Create.sql i klikamy Execute \(lub F5\).

![](../../.gitbook/assets/image%20%28105%29.png)

Nasza tabela została stworzona wraz z początkowymi danymi.

