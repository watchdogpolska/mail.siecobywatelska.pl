Wprowadzenie
#############

Zaistniała konieczność przygotowania nowej wersji aplikacji `mail.siecobywatelska.pl <mail.siecobywatelska.pl>`_, która byłaby otwarta na skuteczny rozwój i rozbudowę. Mogę ją przygotować całkiem sam, a można ją przygotować w zespole z KNI Genbit, a dodatkowo podjąć formalną współpracę zewnętrzną. 

Aplikacja ma służyć do zarządzania wiadomościami urlopowymi oprogramowania DirectAdmin. DirectAdmin to najpopularniejszy panel administracyjny dla hostingów do zarządzania domenami, pocztą, kontami FTP, wiadomościami urlopowymi itd. Posiada API.

Niestety, nawet wiadomości o urlopie (automatyczne odpowiedź w e-mailu) są możliwe do wprowadzenia tylko przez administratora. Powinny być jednak możliwe do wykonania przez użytkownika samemu sobie.

Z założenia stworzone oprogramowanie ma mieć charakter open-source i być dostępne dla każdego zainteresowanego bez dodatkowych opłat.

Funkcje:

 * logowanie wykorzystujące uwierzytelnianie [1]_ w oparciu o zewnętrzny serwer SMTP,
 * wyświetlenie listy istniejących skrzynek pocztowych (dla administratora),
 * zarządzanie wiadomościami urlopowymi:

     * wyświetlenie listy wiadomości urlopowych danego użytkownika,
     * dodanie wiadomości urlopowej z wykorzystaniem API,
     * usunięcie wiadomości urlopowej z wykorzystaniem API,

 * zarządzanie skrzynkami poczty elektronicznej:

     * utworzenie skrzynki poczty elektronicznej,
     * wyświetlenie listy aliasów istniejących dla danej skrzynki poczty elektronicznej,
     * utworzenie zlecenia archiwizacji skrzynki poczty elektronicznej,

 * edycja statycznej treści strony głównej,
 * edycja odnośników menu nawigacyjnego,
 * zarządzanie serwerami DirectAdmin,
 * przedstawienie instrukcji połączenia z różnymi programami pocztowymi.

.. [1] Ponieważ pojęcie "uwierzytelnianie" sprawia kłopoty warto zacytować fragment z `Tomasz Mielnicki, Franciszek Wołowski, Marek Grajek, Piotr Popis, Identyfikacja i uwierzytelnianie w usługach elektronicznych, Przewodnik Forum Technologii Bankowych przy Związku Banków Polskich, Warszawa, 2013 <http://zbp.pl/public/repozytorium/dla_bankow/rady_i_komitety/technologie_bankowe/publikacje/Przewodnik_Identyfikacja_i_uwierzytelnianie_strona_FTB.pdf>`_:
    
        Usługi elektroniczne zakładające interakcję z użytkownikiem wymagają zwykle identyfikacji użytkownika i jego uwierzytelnienia. Zgodnie z terminologią, identyfikację rozumie się jako nadanie (przypisanie) identyfikatora do osoby oraz deklarację (stwierdzenie) tożsamości osoby poprzez przedstawienie indentyfikatora. Taki identyfikator jednoznacznie tą osobę identyfikuje i stanowi elektroniczną tożsamość użytkownika w tymże środowisku. Sama identyfikacja pozwala zatem na stwierdzenie „o kogo chodzi”, ale nie potwierdza, że użytkownik danej e-usługi jest faktycznie tą osobą, która została zadeklarowana i zidentyfikowana. Do tego potwierdzenia służy właśnie uwierzytelnienie, polegające na dostarczeniu dowodów, że użytkownik jest właśnie tą zidentyfikowaną osobą (nikt się nie podszywa). W szczególnych przypadkach identyfikacja i uwierzytelnienie może przebiegać jednocześnie (np. gdy nasz identyfikator jest tajny, stanowiąc jednocześnie „hasło”), ale zasadniczo są to dwa różne procesy. Z kolei pod pojęciem autoryzacji (często mylonej z uwierzytelnieniem i niepoprawnie nazywanej „autentykacją”) rozumie się proces nadania określonych uprawnień, z których następnie poprawnie zidentyfikowana i uwierzytelniona osoba będzie mogła korzystać.
