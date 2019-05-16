# Azure Storage Account

Warsztaty wprowadzą Cię do konta Storage Account, które składa się z 4 usług – blob, queue, table oraz files. Podczas warsztatów skupimy się tylko na trzech pierwszych usługach, pomijając Azure Files.

Podczas warsztatów dowiesz się jak działają wspomniane wcześniej usługi oraz w jakich sytuacjach mogą okazać się niezwykle pomocne lub wręcz niezbędne. Następnie wspólnie stworzymy każdą z tych usług oraz jedną z nich połączymy z przykładową aplikacją webową.

W tych materiałach masz dostęp do kolejnych czynności, które będziemy wspólnie wykonywać podczas warsztatów – w przypadku problemów zawsze możesz tutaj zajrzeć. Materiały są stworzone w taki sposób, aby w przypadku gdy nie będziesz nadążał/a lub nie byłeś/aś obecny/a – możesz spokojnie przerobić je na nowo w domu.

Na końcu materiałów znajdują się zadania domowe, których wykonanie pozwoli Ci utrwalić zdobytą wiedzę – bo przecież nic nie uczy tak dobrze jak wykorzystanie teorii w praktyce.

## O usłudze

Na Azure Storage Account składają się cztery usługi:

* Blob
* Queue
* Table
* Files

### **Azure Blob Storage**

Jest to magazyn pozwalający na przechowywanie dowolnego rodzaju plików w chmurze. Tworząc usługę pliki umieszczamy w tzw. kontenerach – jedna usługa może mieć wiele takich kontenerów. Przykładem zastosowania może być magazyn przechowujący zdjęcia lub dokumenty użytkowników dla określonego systemu czy aplikacji.

### **Azure Table Storage**

Magazyn danych NoSQL pozwalający na przechowywanie dużych ilości danych zawierających pewną strukturę. Prościej mówiąc - możemy stworzyć tabele tak, jak w przypadku tabeli SQL z tą różnicą, że tabele Azure Storage są przeznaczone do przechowywania nierelacyjnych danych. Przykładem zastosowania może być każda tabela nie mająca relacji z innymi – np. tabela logów w aplikacji. Najważniejszymi cechami tabel Azure Storage jest wysoka skalowalność oraz szybki dostęp do danych.

### **Azure Queue Storage**

Usługa pozwalająca na tworzenie kolejek danych. Najczęściej wykorzystywana do kolejkowania komunikatów pomiędzy dwoma różnymi modułami aplikacji lub całymi aplikacjami. Kolejki Azure Storage są dostosowane do dużych obciążeń oraz zapewniają komunikację niezależnie od tego czy działają w chmurze, serwerze lokalnym czy urządzeniu przenośnym.

### **Azure Files**

Link dla ciekawskich do poczytania na przyszłość: [https://docs.microsoft.com/en-us/azure/storage/files/storage-files-introduction](https://docs.microsoft.com/en-us/azure/storage/files/storage-files-introduction)

