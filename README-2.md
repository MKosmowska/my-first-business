# Mój pierwszy biznes / My First Business

Symulator dla uczniów, który pomaga zaplanować pierwszy biznes krok po kroku: od pomysłu, przez rynek i koszty, po próg rentowności i eksperymenty z ceną.

*A simulator that helps secondary-school students plan a first business step by step: idea, market, costs, break-even and price experiments. Available in Polish and English.*

## Co potrafi

- **Konkurencja z mapy.** Aplikacja wyszukuje w OpenStreetMap firmy danego rodzaju w promieniu 5 km od adresu lokalu i liczy je w promieniach 500 m, 1 km, 2,5 km i 5 km.
- **Rynek na prawdziwych danych.** Wyszukiwarka obejmuje każdą gminę w Polsce i dzielnice Warszawy. Gęstość zaludnienia, płace w powiecie oraz struktura wieku i płci mieszkańców pochodzą z GUS (2025), więc uczeń może dobrać grupę docelową, np. seniorów 65+ albo kobiety 20–34.
- **Koszty i próg rentowności.** Koszty stałe i zmienne, marża pokrycia, limit obsługi zespołu, czas zwrotu inwestycji.
- **Popyt zależny od ceny.** Uczeń zakłada, ilu klientów straci przy podwyżce, a aplikacja liczy elastyczność i pokazuje cenę dającą najwyższy wynik.
- **Scenariusze i zadania.** Wariant ostrożny i optymistyczny oraz pytania liczone na danych ucznia.
- **Udostępnianie.** Kod lub link do planu dla nauczyciela i raport do druku lub PDF.

## Co jest prawdziwe, a co przykładowe

**Prawdziwe dane:**
- gęstość zaludnienia każdej gminy i dzielnicy Warszawy (GUS 2025),
- przeciętne wynagrodzenia oraz ludność według wieku i płci w każdym powiecie (GUS 2025),
- konkurenci z OpenStreetMap, pobierani na bieżąco dla adresu wpisanego przez ucznia.

**Dane przykładowe (do ćwiczeń):**
- ceny, koszty i stawki ZUS w gotowych przykładach (fryzjer, korepetycje, serwis rowerowy, sklep internetowy),
- lista konkurentów w trybie demonstracyjnym.

Aplikacja pokazuje to samo rozróżnienie pod paskiem etapów, zawsze najpierw dane prawdziwe. Model jest uproszczony i miesięczny: bez VAT, podatku dochodowego i sezonowości.

## Źródła danych

GUS, Bank Danych Lokalnych (bdl.stat.gov.pl), dane za 2025 r.:
- ludność na 1 km² według gmin i dzielnic Warszawy,
- przeciętne miesięczne wynagrodzenie brutto według powiatów,
- ludność według wieku (18 grup) i płci według powiatów.

Konkurencja: © autorzy OpenStreetMap (licencja ODbL), wyszukiwanie przez Nominatim i Overpass API, na bieżąco w przeglądarce użytkownika.

## Jak powstał

Projekt i założenia: Maja Kosmowska. Kod napisany z pomocą AI (Claude) na podstawie mojej specyfikacji.

## Technicznie

Jeden plik `index.html` (React 18 i htm z CDN), bez własnego serwera i bez zbierania danych. Wyszukiwanie konkurencji łączy się bezpośrednio z publicznymi serwisami OpenStreetMap. Plan ucznia zapisuje się tylko w jego przeglądarce.
