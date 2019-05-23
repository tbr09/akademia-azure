# Tworzenie usługi App Service.

Po wejściu na portal Azure wybieramy opcję Create a resource, a następnie znajdujemy zasób o nazwie Resource group, który będzie kontenerem na wszystkie usługi jakie stworzymy w ramach tego tutoriala.

![](../../.gitbook/assets/image%20%2899%29.png)

Po kliknięciu na usługę powinniśmy zobaczyć jej opis oraz opcję Create, którą wybieramy.

![](../../.gitbook/assets/image%20%2838%29.png)

Powinniśmy wtedy zobaczyć formularz pozwalający na stworzenie wybranej usługi. Wybieramy subskrypcję w ramach, której chcemy stworzyć usługę, nadajemy nazwę naszej usłudze i wybieramy region w jakim zostanie utworzona oraz tworzymy usługę.

![](../../.gitbook/assets/image%20%2898%29.png)

Następnie ponownie wybieramy opcję Create new resource i znajdujemy usługę o nazwie Web App.

![](../../.gitbook/assets/image%20%287%29.png)

Po jej wybraniu powinniśmy zobaczyć krótki opis i wybieramy opcję Create, aby ją stworzyć.

![](../../.gitbook/assets/image%20%288%29.png)

Mamy tutaj dostępnych kilka opcji dotyczących tworzonej usługi.

![](../../.gitbook/assets/image%20%2835%29.png)

Idąc od góry:

* App name - będzie to nazwa naszej usługi, oraz pod tym adresem \(z sufixem .azurewebsites.net\) będzie dostępna nasza aplikacja
* Subscription - subskrypcja w ramach, której będą naliczane opłaty za naszą usługę
* Resource Group - grupa zasobów w ramach, której będzie stworzona nasza usługa - wybieramy grupę stworzoną na początku tego tutoriala
* OS - system operacyjny, na którym będzie działać nasza usługa \(zostawiamy Windows\)
* Publish - sposób publikowania aplikacji na naszą usługę \(istnieje możliwość publikowania obrazów dockerowych, ale my zostawiamy wybraną opcję Code\)
* App Servie plan/Location

To jest najważniejsza opcja przy tworzenie naszej usługi. Od niej będzie zależeć lokalizacja naszej usługi oraz jej wydajność i cena. Po kliknięciu w nią wybieramy Create new i w formularzu New App Service Plan wybieramy nazwę, lokalizację \(będzie ona miała wpływ na opóźnienia w komunikacji z naszą aplikacją\) i Pricing tier, czyli ile będziemy płacić za naszą usługę i jaką ilość zasobów będzie miała dostępną.

![](../../.gitbook/assets/image%20%2881%29.png)

Po kliknięciu w Pricing tier pojawi się okno z kilkoma możliwościami do wyboru. wybieramy na górze Dev/Test i tier F1, a następnie klikamy Apply.

![](../../.gitbook/assets/image%20%2848%29.png)

Powinniśmy zostać z powrotem przekierowani do poprzedniego okna gdzie klikamy na dole Ok.

![](../../.gitbook/assets/image%20%2853%29.png)

* Application Insights - jest to usługa pozwalająca monitorować naszą aplikację pod kątem błędów, wykorzystania zasobów i komunikacji sieciowej. Po kliknięciu w nią wybieramy Disable, a następnie Apply.

![](../../.gitbook/assets/image%20%2890%29.png)

Powinniśmy teraz z powrotem zobaczyć nasz początkowy formularz. Na samym dole wybieramy w nim opcję Create, aby stworzyć naszą usługę.

![](../../.gitbook/assets/image%20%2897%29.png)

Po wejściu w naszą grupę zasobów:

![](../../.gitbook/assets/image%20%2886%29.png)

Powinniśmy zobaczyć usługi, które stworzyliśmy:

![](../../.gitbook/assets/image%20%2820%29.png)

Po wybraniu usługi o typie App Service powinniśmy zobaczyć opcje jej dotyczące. Interesuje nas przycisk Get publish profile, po którego kliknięciu zostanie pobrany plik z danymi pozwalającymi publikować kod na nasz App Service. Powinniśmy zapisać go w bezpiecznym miejscu i nie dzielić się nim z nikim innym.

![](../../.gitbook/assets/image%20%2871%29.png)

