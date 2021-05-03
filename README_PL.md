# Motywacja

Dlaczego powstałten projekt? Skąd pomysł?

Pewnego dnia zapragnąłem uporządkować swoją książkę adresową i połączyć tę 
z gmaila, lokalnego thunderbirda itd... Okazało się, że jest z tym pewien 
problem. Brakuje spójnego formatu i odpowiednich narzędzi. Dodatkowo brakowało
mi pewnych właściwości w książce adresowej w moim ulubionym kliencie pocztu - 
Thunderbirdzie. Zdecydowałem sią na napisanie własnego klienta. Jednak 
najpierw potrzebowałem porzadnej książki adresowej :) Od niej zacząłem.

Przemyślałem czego oczekuję od książki. Oto moje spostrzeżenia:

* jedna osoba może mieć wiele adresów email (jeden jest domyślny)
* jedna osoba może mieć wiele kluczy publicznych oraz sygnatur
  (jeden powiązany z konkretnym adresem)
* jedna osoba może mieć po prostu jeden klucz publiczny i sygnaturę
* każdy email konkretnej osoby może być oznaczony jako podlegający 
  szyfrowaniu i sygnowaniu głównym kluczem i sygnaturą
* każda osoba w książce powinna mieć możliwość zastosowania awatara 
  (dla łatwiejszej indetyfikacji w kliencie poczty); pamiętając, że 
  dla każdego emaila danej osoby może być zdefiniowany awatar w serwisie
  https://gravatar.org należy ustawić informację, że będzie on mimo wszystko,
  pobierany z głównego profilu w książce adresowej
* dla każdej osoby możemy przechowywać także informacje takie jak:
  * pierwsze imię
  * drugie/trzecie imię
  * nazwisko
  * nickaname
  * nr telefonu (naziemny) - dowolna liczba, jeden domyślny
  * nr telefonu (komórkowego) - dowolna liczba, jeden domyślny
  * dodatkowy opis (do 4kb)
  * dowolna liczba adresów zamieszkania
  * dowolna liczba adresów www 
  * dowolna liczba organizacji, do których należy dana osoba
* na poziomie książki adresowej możemy zdefiniować dowolną liczbę organizacji
  (organizacje będą wykorzystywane w danych użytkowników)
* każda organizacja może zawierać informacje takie jak:
  * awatar organizacji
  * nazwa organizacji
  * adres www
  * adres fizyczny
  * telefon (naziemny) - dowolna liczba, jeden domyślny
  * telefon (komórkowy) - dowolna liczba, jeden domyślny

Każdy wpis dotyczący organizacji oraz osoby w książce dostaje swój własny 
ID (uuid v4). Id organizacji wykorzystujemy w danych poszczególnych osób, 
by móc w łatwy sposób powiązać dowolny kontakt z pozostałymi z konkretnej 
organizacji.

Zdecydowałem, że najlepszym formatem będzie XML zapisany UTF-16. Należy więc
dostarczyć odpowiedni plik XSD, oraz biblioteki ułatwiające korzystanie z książki.
Na początek implementacje dla:

* Clojure (https://clojure.org)
* Java (https://www.oracle.com/java/)
* Kotlin (https://kotlinlang.org)
* Scala (https://scala-lang.org)
* C# (https://docs.microsoft.com/en-us/dotnet/csharp/)
* F# (https://fsharp.org/)
* Ruby (https://www.ruby-lang.org)
* Go (https://golang.org)
* Rust (https://www.rust-lang.org)
* CommonLisp (https://lisp-lang.org)
* Racket (https://racket-lang.org)
* Elixr (https://elixir-lang.org)





