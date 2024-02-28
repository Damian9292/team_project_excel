Tematyka projektu

MMA (ang. mixed martial arts) to dyscyplina sportowa, która z każdym rokiem zyskuje na popularności. W trakcie walk w formule MMA zawodnicy walczą, wykorzystując duży zakres dozwolonych technik. Rywalizacja między dwoma zawodnikami toczy się w płaszczyźnie stojącej (w tzw. stójce) oraz leżącej (w tzw. parterze) w ośmiokątnym ringu zwanym oktagonem. Zawodnicy przed walką oraz w trakcie przerw stoją w przypisanych do siebie narożnikach (czerwonym i niebieskim). W typowych walkach MMA dozwolone są rzuty, ciosy pięściami, kopnięcia, dźwignie i duszenia.

O wyniku walki decyduje nokaut, poddanie się lub decyzja sędziów (jeżeli walka nie zakończyła się przed czasem). Walkę sędziuje jeden sędzia ringowy i trzech sędziów punktowych, przy czym każdy z nich prowadzi oddzielną punktację, dlatego występują trzy typy decyzji:

jednogłośna (trzech sędziów wskazuje zwycięstwo punktowe tego samego zawodnika)
większościowa (dwóch sędziów wskazuje zwycięstwo punktowe jednego zawodnika, a trzeci sędzia ocenia walkę na remis)
niejednogłośna (dwóch sędziów wskazuje zwycięstwo punktowe jednego zawodnika, a trzeci sędzia ocenia walkę na korzyść jego przeciwnika)
Zawodnicy muszą obligatoryjnie posiadać ochraniacze na zęby i rękawice (zwykle cienkie, które umożliwiają chwytanie przeciwnika).

Zawodnicy walczą między sobą w ramach różnych kategorii wagowych. W praktyce liczba kategorii i limity wagi obowiązujące w danej kategorii mogą się różnić w ramach kraju, a nawet organizacji. Niekiedy organizowane są walki, które odbywają się w umownym limicie (ang. catchweight), jeżeli zawodnicy podchodzą z różnych kategorii, w których walczą na co dzień. W Polsce i na świecie gale walk MMA są organizowane przez wiele podmiotów. Podczas jednej gali walk odbywa się zwykle od kilku do kilkunastu walk. Jedną z najstarszych, a na pewno najbardziej prestiżową na świecie organizacją jest UFC (ang. Ultimate Fighting Championship). UFC powstało w Stanach Zjednoczonych w 1993 roku i zrzesza setki najlepszych zawodników z całego świata.

Cel analizy danych
Tym razem wcielisz się w rolę analityka danych pracującego dla UFC, którego zadaniem jest przygotowanie danych do artykułu o podsumowaniu historii federacji. Artykuł zostanie opublikowany na stronie internetowej federacji ufc.com i będzie dostępny dla wszystkich zainteresowanych kibiców na świecie.

Zlecając nam przygotowanie ciekawych informacji dot. federacji, zarząd UFC przygotował listę 5 punktów z pytaniami, na które musisz odpowiedzieć w ramach analizy danych:

Ilu zawodników do tej pory chociaż raz walczyło w UFC? Ile lat miał najstarszy zawodnik w trakcie walki? Ile wydarzeń (gal) zorganizowano w historii? W którym mieście zorganizowano największą liczbę gal?
Ile walk odbyło się w ramach organizacji UFC w podziale na kategorie wagowe?
Ile walk zakończyło nokautem, decyzją sędziów, poddaniem lub w inny sposób? Jaki procent wszystkich walk zakończył się nokautem (KO) lub technicznym nokautem (TKO)?
Którzy zawodnicy są najlepszymi w historii federacji UFC? Przedstaw TOP10 zawodników (z największą liczbą wygranych). W przypadku zawodników z jednakową liczbą zwycięstw kolejność ustalana jest alfabetycznie (względem zmiennej z imieniem i nazwiskiem zawodnika).
O których zawodnikach możemy powiedzieć, że są najlepszymi uderzaczami (ang. striker) i mają największą liczbę nokautów na koncie?
Oprócz powyższych pytań będziesz mieć okazję na zaproponowanie swoich pomysłów i spostrzeżeń (ang. insights), które mogą okazać się ciekawe dla pasjonatów MMA i znajdą się w artykule.

Opis danych
Dane o historycznych walkach dotyczą okresu od początku powstania organizacji do marca 2021 roku. Zbiór danych składa się z trzech tabel, które przechowują szczegółowe informacje o walkach i ich przebiegu, zawodnikach i lokalizacjach, w jakich odbywały się poszczególne walki.
Poniżej opisujemy znaczenia poszczególnych zmiennych, które pomogą Ci dobrze zrozumieć dane, którymi będziesz dysponować w trakcie projektu końcowego. Niektóre kolumny w danych mają przedrostki r oraz b, co oznacza kolor narożnika, do którego zawodnik był przypisany w trakcie walki, np.:

r_fighter_id – identyfikator zawodnika z narożnika czerwonego

Słownik kolumn
fighter_id – identyfikator zawodnika,
fighter_name – imię i nazwisko zawodnika,
weight_pounds – waga zawodnika w funtach,
date_of_birth – data urodzenia zawodnika,
height_feet + height_inches – całkowity wzrost zawodnika,
kd – liczba nokdaunów (ang. knockdown); opisuje liczbę zdarzeń, w których przeciwnik upadał na matę oktagonu po ciosie,
sig_str – stosunek liczby znaczących ciosów trafionych do liczby wyprowadzonych znaczących ciosów,
total_str – stosunek liczby ciosów trafionych do liczby wyprowadzonych ciosów
td – stosunek liczby udanych obaleń do liczby prób obaleń,
sub_att – liczba prób poddania (np. uduszenia przeciwnika lub założenia dźwigni),
rev – liczba przetoczeń przeciwnika w trakcie walki w parterze ,
ctrl – czas kontroli przeciwnika przez zawodnika walcząc w parterze (w formacie HH:MM:SS, gdzie HH – godziny, MM – minuty, SS – sekundy),
head – stosunek liczby ciosów trafionych w głowę do liczby ciosów wyprowadzonych w głowę,
leg – stosunek liczby ciosów (kopnięć) trafionych w głowę do liczby ciosów (kopnięć) wyprowadzonych na nogi,
distance - stosunek liczby znaczących ciosów trafionych z dystansu do liczby wyprowadzonych znaczących ciosów z dystansu,
clinch - stosunek liczby znaczących ciosów trafionych w klinczu do liczby wyprowadzonych znaczących ciosów w klinczu,
ground - stosunek liczby znaczących ciosów trafionych na ziemi do liczby wyprowadzonych znaczących ciosów na ziemi,
win_by – sposób zakończenia walki,
last_round_time – czas ostatniej z rund, po którego upływie zakończono walkę
format – format walki (liczba rund + czas poszczególnych rund), np. 3 Rnd (5-5-5) oznacza 3 rundy po 5 minut,
format_rounds – liczba rund,
referee – sędzia ringowy pojedynku,
date – data walki,
fight_type – kategoria wagowa, w jakiej toczyła się walka,
location_id – identyfikator lokalizacji walki,
city – miasto, w którym odbyła się walka,
region/district – region lub stan, w którym odbyła się walka,
country – kraj, w którym odbyła się walka,
winner – zwycięzca walki (kolor narożnika).
Powodzenia!