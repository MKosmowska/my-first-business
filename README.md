# Coasely · Run the numbers before you run the business

Narzędzie do wczesnej prognozy i wyceny pomysłu na biznes: od rynku na prawdziwych danych, przez koszty, podatki i finansowanie, po prognozę na 3 lata i orientacyjną wycenę.

*A tool for early-stage forecasting and valuation of a business idea: real market data, costs, Polish tax and social security, financing, a 3-year forecast and an indicative DCF valuation. Available in Polish and English.*

## Co potrafi

- **Rynek na prawdziwych danych.** Każda gmina w Polsce i dzielnice Warszawy: gęstość zaludnienia, płace w powiecie oraz struktura wieku i płci mieszkańców (GUS, 2025).
- **Konkurencja według rejestru REGON.** Ile firm z danej branży (sekcji PKD) działa w gminie, na 10 tys. mieszkańców, w porównaniu z gminami podobnej wielkości i średnią dla Polski, plus odsetek zawieszonych firm. Wskaźnik nasycenia rynku z regresji na danych wszystkich gmin (mieszkańcy, gęstość, typ gminy, płace w powiecie, miejsca noclegowe) oraz wydatki mieszkańców na daną kategorię w przeliczeniu na jedną firmę. Wynik trafia też do testu pomysłu, sygnałów, raportu i opisu dla AI.
- **Konkurencja z mapy.** Wyszukiwanie w OpenStreetMap firm jednego z ponad 35 rodzajów w promieniu 5 km od adresu, z podziałem na 500 m, 1 km, 2,5 km i 5 km.
- **Koszty, cena i próg rentowności.** Koszty stałe i zmienne, marża pokrycia, limit obsługi zespołu, popyt zależny od ceny i cena dająca najwyższy wynik.
- **Podatki i ZUS (przepisy na 2026 r.).** Porównanie skali podatkowej, podatku liniowego, ryczałtu i spółki z o.o. na liczbach użytkownika, z podpowiedzią najkorzystniejszej formy i wyjaśnieniami po najechaniu kursorem. Etapy ZUS: ulga na start, preferencyjny, pełny.
- **Finansowanie i dźwignia.** Wkład własny, kredyt w równych ratach, amortyzacja, rozkład DuPont (ROE = marża netto × rotacja aktywów × mnożnik kapitału), ROE z kredytem i bez, dźwignia finansowa (DFL).
- **Prognoza na 36 miesięcy.** Rozruch, wzrost klientów, inflacja, zmiany etapów ZUS, podatki liczone rocznie, raty kredytu, stan gotówki i moment zwrotu wkładu.
- **Wycena DCF.** Zdyskontowane przepływy z lat 1–3, wartość po 3. roku (model Gordona), korekta o kredyt. Dwie kwoty: firma razem z pracą właściciela oraz firma, gdyby trzeba było kogoś zatrudnić na jego miejsce.
- **Test pomysłu.** Automatyczny test 11 punktów krytycznych (marża, próg rentowności a rynek i limit obsługi, spadek klientów o 30%, wzrost kosztów o 20%, porównanie z etatem, gotówka na rozruch, zwrot wkładu, kredyt), lista 6 rzeczy do sprawdzenia poza liczbami oraz analiza wrażliwości i scenariusze.
- **Sygnały.** Automatycznie wyliczane ryzyka i szanse, np. brak gotówki w rozruchu, próg rentowności powyżej szacunku rynku, kredyt obniżający ROE, korzystniejsza forma opodatkowania.
- **Analiza AI.** Przygotowuje opis planu z liczbami i otwiera go w Claude albo ChatGPT. Dane trafiają do AI dopiero po kliknięciu.
- **Moje plany.** Zapisywanie wielu planów w przeglądarce i porównanie 2–4 planów obok siebie.
- **Eksport do Excela.** Plik .xlsx z modelem na formułach (żółte pola można zmieniać), prognozą na 36 miesięcy, porównaniem form opodatkowania, scenariuszami i wykresami.
- **Udostępnianie.** Kod lub link do planu i raport do druku lub PDF.
- **O projekcie i metodologia.** Źródła danych, wzory i ograniczenia modelu.
- **Wygląd.** Tryb jasny, ciemny albo zgodny z systemem; paleta granat i bursztyn, zieleń i czerwień tylko dla zysku i straty.

## Co jest prawdziwe, a co przykładowe

**Prawdziwe dane:** gęstość zaludnienia gmin i dzielnic, płace oraz ludność według wieku i płci w powiatach (GUS 2025), liczba firm według branż i firmy zawieszone w każdej gminie (rejestr REGON, stan na 31.10.2026), konkurenci z OpenStreetMap pobierani na bieżąco, stawki podatków i składek na 2026 r.

**Dane przykładowe:** ceny i koszty w 3 dopracowanych przykładach (salon fryzjerski w Poznaniu, kawiarnia w Gdańsku, kurs online) oraz lista konkurentów w trybie demonstracyjnym.

Model jest uproszczony: bez VAT i sezonowości. Podatki liczone bez ulg rodzinnych, wspólnego rozliczenia i estońskiego CIT. Wyniki są szacunkowe i nie są poradą podatkową ani inwestycyjną.

## Obrazek podglądu linku

Wgraj do repozytorium plik `og.png` (1200×630 px). Strona już na niego wskazuje, więc pojawi się w podglądzie na LinkedIn i w komunikatorach.

## Źródła danych

- GUS, Bank Danych Lokalnych (bdl.stat.gov.pl), dane za 2025 r.
- GUS, Miesięczna informacja o podmiotach gospodarki narodowej w rejestrze REGON, październik 2026 (tablice 3 i 12).
- GUS, Powierzchnia i ludność w przekroju terytorialnym w 2025 r. (tablica 21).
- GUS, Bank Danych Lokalnych: miejsca noclegowe w turystycznych obiektach noclegowych według gmin, 2025.
- GUS, Budżety gospodarstw domowych w 2025 r. (tablice 36 i 37a).
- ZUS i Ministerstwo Finansów: kwoty składek, minimalna składka zdrowotna, limit odliczenia składki zdrowotnej, skala podatkowa na 2026 r.
- Konkurencja: © autorzy OpenStreetMap (licencja ODbL), Nominatim i Overpass API.

## Jak powstał

Projekt i założenia: Maja Kosmowska.

## Technicznie

Jeden plik `index.html` (React 18 i htm z CDN), bez własnego serwera. Strona nie zbiera danych osobowych: odwiedziny liczy anonimowo GoatCounter, bez ciasteczek. Plan zapisuje się tylko w przeglądarce użytkownika. Plany zapisane w starszej wersji otwierają się z ręcznie wpisanym ZUS, więc ich wyniki się nie zmieniają.


## Nazwa i znak Coasely
Nazwa jest hołdem dla Ronalda Coase'a (1910–2013), noblisty z ekonomii, który w eseju „The Nature of the Firm” (1937) zapytał, po co w ogóle zakładać firmę. Coasely stawia to pytanie przy Twoim pomyśle: czy warto zamienić go w firmę? Wymowa: /ˈkoʊs.li/. Richard Cantillon jako pierwszy opisał przedsiębiorcę jako kogoś, kto działa w niepewności; Coasely pomaga tę niepewność zmierzyć. Projekt nie jest powiązany z Ronaldem Coase'em, jego rodziną ani instytucjami jego imienia.

Znak: litera C z pełnych bloków w kolorze #18284A; górne ramię dłuższe od dolnego (wzrost). Pliki: `coasely-logo.svg` i `coasely-logo-dark.svg` (sam znak), `coasely-logo-full.png` i `coasely-logo-full-dark.png` (znak, kreska i nazwa, przezroczyste tło).

Adres strony: https://coasely.com

Domyślny język strony to angielski; wybór PL/EN zapamiętuje się w przeglądarce.
