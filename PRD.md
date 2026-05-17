# Handmade Poland — Dokument wymagań produktu (PRD)

*Wyjaśnienia skrótów i pojęć użytych w dokumencie znajdują się w sekcji „Słownik skrótów i pojęć" na końcu PRD.*

## Wprowadzenie

Handmade Poland to internetowy marketplace z rękodziełem wytwarzanym w Polsce. Łączymy twórców (rzemieślników, artystów, hobbystów) z kupującymi szukającymi unikalnych, ręcznie robionych produktów.

**Problem.** Polscy twórcy rękodzieła nie mają taniego, dedykowanego kanału sprzedaży: rodzime platformy pobierają wysokie prowizje (Pakamera ~24,5%, Artillo ~25%), a Etsy nie jest zoptymalizowane pod polski rynek i twórców. Kupujący nie mają jednego zaufanego miejsca z polskim rękodziełem.

**Wizja.** Najuczciwsza prowizyjnie i najbardziej zaufana platforma rękodzieła w Polsce — niska, przejrzysta prowizja dla twórców i gwarancja autentyczności „handmade" dla kupujących.

**Dokumenty powiązane:** [monetyzacja.md](monetyzacja.md) (analiza wysokości prowizji).

## Cele i metryki sukcesu

**Cel nadrzędny (North Star):** miesięczny GMV (łączna wartość zrealizowanych zamówień) — mierzy jednocześnie zdrową podaż, popyt i zaufanie.

**Cele biznesowe:**
1. Zbudować płynny marketplace (oferta szybko znajduje kupującego).
2. Utrzymać przewagę „uczciwej prowizji" względem polskiej konkurencji.
3. Zagwarantować autentyczność „handmade" jako fundament zaufania.

**Kluczowe metryki:**

| Obszar | Metryka | Cel MVP (do ustalenia) |
|---|---|---|
| Podaż | Aktywni sprzedawcy (≥1 oferta) | np. 100 w 3 mies. |
| Podaż | Liczba aktywnych ofert | np. 1 000 |
| Popyt | Miesięczni kupujący | np. 500 |
| Płynność | % ofert sprzedanych w 30 dni | ≥ 15% |
| Konwersja | Wizyta → zakup | ≥ 1,5% |
| Wartość | Średnia wartość koszyka (AOV) | 80–150 zł |
| Wartość | Miesięczny GMV | do ustalenia |
| Retencja | Powracający kupujący (90 dni) | ≥ 20% |
| Zaufanie | Wskaźnik sporów / zamówień | ≤ 2% |
| Zaufanie | Wskaźnik zwrotów | ≤ 5% |
| Jakość | % ofert zweryfikowanych „handmade" | 100% (warunek konieczny) |

**Kryterium sukcesu MVP:** marketplace uznajemy za zwalidowany, gdy przez 2 kolejne miesiące osiągamy docelową płynność (≥15% ofert sprzedanych/30 dni) przy ≥100 aktywnych sprzedawcach — co dowodzi rozwiązania problemu chicken-and-egg.

## Persony i rynek docelowy

**Zasięg (MVP):**
- **Sprzedawcy:** wyłącznie twórcy z Polski (wymóg „made in Poland" jest rdzeniem produktu).
- **Kupujący:** Polska. Sprzedaż zagraniczna (diaspora, UE) — poza zakresem MVP, w roadmapie.
- **Język:** polski. **Waluta:** PLN.

**Persony — sprzedawcy:**

1. **Hobbystka „dorobkowa" (Ania, 34)** — robi rękodzieło po godzinach, sprzedaje nieregularnie, technicznie niezaawansowana. Potrzebuje: prostego wystawienia oferty, niskiej prowizji, braku opłat stałych. Ból: wysokie prowizje Pakamery/Artillo zjadają jej marginalny zarobek.
2. **Profesjonalna twórczyni (Marta, 41)** — rękodzieło to jej główny dochód, ma działalność, większy wolumen. Potrzebuje: zarządzania zamówieniami, szybkiego payoutu, wiarygodności platformy. Ból: brak taniego, dedykowanego kanału w PL; Etsy słabo dopasowane do rynku PL.

**Persony — kupujący:**

3. **Kupujący prezent (Tomek, 38)** — szuka czegoś unikalnego na okazję, kieruje się zdjęciami i zaufaniem. Potrzebuje: pewności że to autentyczne handmade, szybkiej dostawy, łatwego zwrotu. Ból: ryzyko trafienia na masówkę udającą rękodzieło.
4. **Świadoma kupująca (Kasia, 29)** — ceni lokalne, ręcznie robione, etyczne; kupuje do domu i na prezenty. Potrzebuje: historii twórcy, kategorii, opinii innych. Ból: rozproszenie oferty po Instagramie i wielu sklepach.

**Rynek:** polskie platformy rękodzieła pobierają 19–25% prowizji (szczegóły i źródła: [monetyzacja.md](monetyzacja.md)). Luka: brak taniej, zaufanej, dedykowanej platformy PL.

## Model biznesowy i prowizja

**Zasady podstawowe:**
- **Wystawianie ofert jest darmowe** — brak opłat za listing.
- **Brak abonamentów i opłat stałych** dla sprzedawców.
- **Przychód wyłącznie z transakcji** — platforma pobiera prowizję od każdej zrealizowanej sprzedaży.

**Wysokość prowizji** (rekomendacja z [monetyzacja.md](monetyzacja.md)):
- Model **rozdzielony**: prowizja platformy **7–8%** + przeniesiony koszt płatności (**~2–3%**). Komunikacja na zewnątrz: „**~10% i nic poza tym**".
- **Opłatę minimalną** od transakcji (np. 2–3 zł) — przyjmujemy, by małe koszyki nie były stratne (dokładna kwota: do ustalenia).
- **Prowizję płaci sprzedawca** — potrącana z payoutu (standard marketplace), niewidoczna dla kupującego w cenie.
- **Jednolita stawka** w MVP — bez różnicowania per kategoria (rozważane w roadmapie).

**Promocja startowa:** 0% prowizji platformy dla pierwszych N sprzedawców / przez pierwsze 3 miesiące — narzędzie rozruchu podaży (powiązane z Sekcją 13, cold start). Parametry: do ustalenia.

**Otwarte do potwierdzenia (TODO):** dokładna stawka w paśmie 7–8%, kwota opłaty minimalnej, N i czas trwania promocji startowej.

*Przepływ pieniędzy i payout (escrow vs szybka wypłata) — Sekcja „Płatności, payout, escrow".*

## Definicja „handmade" i weryfikacja

Autentyczność rękodzieła jest fundamentem zaufania platformy. Ta sekcja jest nadrzędna wobec decyzji produktowych — w razie konfliktu wygrywa ochrona autentyczności.

**Co kwalifikuje się jako „handmade":**
- Produkt **zaprojektowany i wykonany ręcznie przez sprzedawcę** (lub jego małą pracownię/zespół).
- Dopuszczalne narzędzia i maszyny prowadzone przez twórcę (maszyna do szycia, koło garncarskie, piec, toczak) — o ile kluczowy wkład jest manualny i twórczy.
- Produkty na zamówienie / personalizowane wykonane przez twórcę.

**Co NIE kwalifikuje się:**
- Towar odsprzedawany, niewykonany przez sprzedawcę.
- Produkcja masowa / fabryczna, dropshipping.
- Czysta odsprzedaż vintage/antyków (brak wkładu wytwórczego).
- Zestawy montowane bez twórczego przekształcenia.

**Weryfikacja — etapy:**
1. **Onboarding sprzedawcy:** akceptacja Polityki Handmade, deklaracja, opis warsztatu/procesu, zdjęcia „zza kulis".
2. **Tworzenie oferty:** obowiązkowe pola — materiały, opis procesu wykonania, zdjęcie etapu pracy/warsztatu.
3. **Moderacja prewencyjna:** pierwsze N ofert nowego sprzedawcy zatwierdzane ręcznie przed publikacją.
4. **Moderacja bieżąca:** losowo-ryzykowa + zgłoszenia od kupujących (reverse image search vs katalogi typu AliExpress).

**Egzekwowanie (eskalacja):** ostrzeżenie → usunięcie oferty → wstrzymanie payoutu spornego zamówienia → zawieszenie konta → trwały ban. Polityka Handmade jest częścią Regulaminu (Sekcja „Zgodność prawna PL/UE").

**Decyzje otwarte (TODO):**
- (a) Dopuszczalność biżuterii/produktów z gotowych komponentów przy twórczym przekształceniu i własnym projekcie.
- (b) Dopuszczalność print-on-demand z autorskim wzorem.
- (c) Liczba N ofert objętych moderacją prewencyjną nowego sprzedawcy.

## Zakres funkcjonalny: MVP vs. później + przepływy

**MVP — kupujący:**
- Strona główna, przeglądanie kategorii, widok kategorii
- Wyszukiwarka + podstawowe filtry (kategoria, cena)
- Strona produktu (zdjęcia, opis, materiały, opis procesu, info o twórcy)
- Koszyk i checkout
- Konto kupującego: historia i status zamówień
- Zgłoszenie oferty / spór (Sekcja „Zaufanie i bezpieczeństwo")

**MVP — sprzedawca:**
- Rejestracja i onboarding z akceptacją Polityki Handmade (Sekcja „Definicja »handmade«")
- Panel: lista zamówień, „Moje produkty", „Dodaj/edytuj produkt" (pola obowiązkowe handmade)
- Obsługa zamówienia: oznaczenie „wysłane" + numer przesyłki
- Podgląd payoutu i rozliczeń (Sekcja „Płatności, payout, escrow")
- Publiczny, udostępnialny link do sklepu sprzedawcy — działa bez płynności marketplace (wartość single-player, Sekcja „Go-to-market i cold start")

**MVP — platforma/operator:**
- Kolejka moderacji ofert (Sekcja „Definicja »handmade«")
- Panel admina: zarządzanie sprzedawcami/ofertami, eskalacje

**Poza MVP (roadmapa):** wiadomości kupujący–sprzedawca, lista życzeń, prowizja różnicowana, sprzedaż zagraniczna, aplikacja mobilna, zaawansowane filtry.

*Landing page i artefakty pre-launch — patrz Sekcja „Wersje i roadmapa".*

**Kluczowe przepływy (MVP):**
1. **Onboarding sprzedawcy:** rejestracja → akceptacja polityki → dodanie oferty → moderacja prewencyjna → publikacja.
2. **Zakup:** odkrycie → produkt → koszyk → checkout → płatność → potwierdzenie zamówienia.
3. **Realizacja:** sprzedawca wysyła → kupujący potwierdza odbiór (lub upływ czasu) → zwolnienie payoutu (Sekcja „Płatności, payout, escrow").
4. **Spór:** zgłoszenie kupującego → wstrzymanie payoutu → rozstrzygnięcie operatora (Sekcja „Zaufanie i bezpieczeństwo").

## Płatności, payout, escrow

**Operator płatności:** zewnętrzny dostawca z gotowym modelem marketplace / split payment (np. PayU Marketplace, Przelewy24, Tpay, Stripe Connect, Mangopay). Platforma **nie staje się instytucją płatniczą** — środki rozlicza dostawca. Wybór konkretnego: do ustalenia.
- **Metody płatności (MVP):** BLIK, karta, szybki przelew (pay-by-link). Apple/Google Pay — roadmapa.
- **Waluta:** PLN.

**Przepływ środków (model escrow-light):**
1. Kupujący płaci całość przy zamówieniu; środki trafiają na rachunek powierniczy/split dostawcy.
2. Sprzedawca wysyła i oznacza „wysłane" + numer przesyłki.
3. **Zwolnienie payoutu:** po potwierdzeniu odbioru przez kupującego **lub** automatycznie po X dniach od oznaczenia „wysłane" (co nastąpi pierwsze), pomniejszone o prowizję (Sekcja „Model biznesowy i prowizja").
4. Otwarty spór (Sekcja „Zaufanie i bezpieczeństwo") **wstrzymuje** payout do rozstrzygnięcia.

**Wypłaty:** przelew na konto sprzedawcy; harmonogram (np. tygodniowy) i próg minimalny — do ustalenia.

**Zwroty i chargebacki:**
- Zwrot środków z kwoty zatrzymanej; jeśli payout już zwolniony — potrącenie z kolejnych payoutów (clawback).
- **Koszt chargebacku za niedostarczenie / niezgodność z opisem ponosi sprzedawca.** Chargeback z tytułu oszustwa płatniczego (nie z winy sprzedawcy) absorbuje platforma/dostawca.

**Otwarte do potwierdzenia (TODO):** wybór dostawcy płatności, liczba X dni do automatycznego zwolnienia payoutu, harmonogram i próg minimalny wypłat.

*VAT, faktury i obowiązki podatkowe sprzedawcy — Sekcja „Zgodność prawna PL/UE".*

## Wysyłka i zwroty

**Model wysyłki (MVP):** sprzedawca wysyła towar bezpośrednio do kupującego. Platforma nie obsługuje logistyki ani magazynowania.
- **Metody (PL):** Paczkomaty InPost, kurier, Poczta Polska, opcjonalny odbiór osobisty.
- **Koszt dostawy:** ustala sprzedawca per metoda (stawka stała lub progi); opcja darmowej wysyłki. Integracja etykiet/nadań (InPost/Furgonetka) — roadmapa.
- **Czas realizacji:** sprzedawca deklaruje czas przygotowania na ofercie (rękodzieło bywa na zamówienie).
- **Tracking:** sprzedawca podaje numer przesyłki przy „wysłane" — uruchamia timer payoutu (Sekcja „Płatności, payout, escrow").

**Zwroty i prawo odstąpienia:**
- Konsument ma **14-dniowe prawo odstąpienia** (sprzedaż na odległość, prawo PL/UE).
- **Wyjątek: produkty personalizowane / wykonane na indywidualne zamówienie** są ustawowo wyłączone z prawa odstąpienia. Oferty takie muszą być **wyraźnie oznaczone** przy zakupie. Szczegóły prawne: Sekcja „Zgodność prawna PL/UE".
- **Koszt zwrotu** ponosi kupujący, chyba że towar wadliwy/niezgodny z opisem (wtedy sprzedawca).
- **Proces:** zgłoszenie zwrotu → akceptacja → odesłanie → zwrot środków z kwoty zatrzymanej lub clawback (Sekcja „Płatności, payout, escrow").

**Uszkodzenie/zaginięcie w transporcie:** odpowiedzialność po stronie sprzedawcy do momentu doręczenia; reklamacja u przewoźnika po stronie sprzedawcy, wsparcie operatora w sporze.

## Zaufanie i bezpieczeństwo

**Opinie i oceny (MVP):**
- Ocena wyłącznie po **zweryfikowanym zakupie**; kupujący ocenia sprzedawcę/produkt po doręczeniu.
- Sprzedawca może odpowiedzieć na opinię. Opinie podlegają moderacji (mowa nienawiści, dane osobowe, treści bezprawne).
- W MVP ocena jednokierunkowa: kupujący → sprzedawca.

**Weryfikacja sprzedawcy (KYC):**
- Weryfikacja tożsamości i rachunku bankowego przez dostawcę płatności (warunek payoutu, Sekcja „Płatności, payout, escrow") + podstawowa weryfikacja na onboardingu.

**Rozstrzyganie sporów:**
- Powody: niedostarczone / niezgodne z opisem / uszkodzone.
- Przepływ: zgłoszenie → wstrzymanie payoutu → odpowiedź sprzedawcy w SLA → mediacja operatora → rozstrzygnięcie (zwrot / zwolnienie / częściowy zwrot). SLA: do ustalenia.

**Moderacja treści i produkty zakazane:**
- Moderacja ofert (zdjęcia, opisy) — wspólna z weryfikacją handmade (Sekcja „Definicja »handmade«").
- **Produkty zakazane:** broń, treści nielegalne, podróbki/naruszenia IP, żywność i kosmetyki podlegające regulacjom, materiały niebezpieczne, wyroby z gatunków chronionych.

**Przeciwdziałanie nadużyciom:** wykrywanie powielonych zdjęć (reverse image search, Sekcja „Definicja »handmade«"), nadużycia chargeback po stronie kupującego, brak wysyłki po stronie sprzedawcy. Zgłaszanie ofert/sprzedawców/opinii → kolejka moderacji (Sekcja „Zakres funkcjonalny").

**Naruszenia IP:** procedura zgłoszenia i zdjęcia oferty na wniosek uprawnionego (notice-and-takedown).

*Bezpieczeństwo techniczne (dane, hasła, płatności) — Sekcja „Wymagania niefunkcjonalne".*

## Zgodność prawna PL/UE

*Sekcja definiuje wymagania; ostateczne dokumenty i interpretacje wymagają radcy prawnego — PRD nie jest opinią prawną.*

**Dokumenty platformy:** Regulamin (osobne warunki dla sprzedawcy i kupującego), Polityka Prywatności, Polityka Cookies, Polityka Handmade (załącznik, Sekcja „Definicja »handmade«"), Polityka Zwrotów (Sekcja „Wysyłka i zwroty").

**RODO / dane osobowe:** platforma jako administrator; podstawy przetwarzania, umowy powierzenia z podprocesorami (płatności, hosting, przewoźnicy), realizacja praw podmiotów, polityka retencji, baner zgody cookies.

**Prawa konsumenta (ustawa o prawach konsumenta):** obowiązki informacyjne przedkontraktowe, 14-dniowe odstąpienie i jego **wyłączenie dla produktów personalizowanych/na zamówienie** (Sekcja „Wysyłka i zwroty"), rękojmia i ścieżka reklamacji.

**Status sprzedawcy i podatki:**
- Dopuszczamy sprzedawców jako **osoby prywatne (działalność nierejestrowana)** i **podmioty z działalnością/VAT**. Status deklarowany na onboardingu; odpowiedzialność podatkową ponosi sprzedawca, platforma informuje o progach.
- **DAC7 (obowiązkowe):** zbieranie danych identyfikacyjnych i dochodowych sprzedawców (PESEL/NIP/dane) na onboardingu i **roczne raportowanie do KAS**. Bez kompletu danych payout zablokowany.
- **Faktury:** dokument sprzedaży dla kupującego wystawia sprzedawca; platforma wystawia sprzedawcy fakturę za prowizję (Sekcja „Model biznesowy i prowizja").

**Obowiązki platformy pośredniczącej:**
- **DSA:** notice-and-action (Sekcja „Zaufanie i bezpieczeństwo"), identyfikowalność sprzedawcy-przedsiębiorcy, punkt kontaktowy, przejrzysty Regulamin.
- **Dyrektywa Omnibus:** oznaczanie opinii „zweryfikowany zakup" i ich autentyczność (Sekcja „Zaufanie i bezpieczeństwo"), transparentność cen/promocji.
- **GPSR (bezpieczeństwo produktów):** dane wytwórcy i zgodność dla kategorii ryzykownych (świece, kosmetyki, zabawki, biżuteria).

## Role i uczestnicy

**Uczestnicy główni:**
- **Sprzedawca (twórca)** — niezależny rzemieślnik/artysta z Polski publikujący i sprzedający własne rękodzieło. Onboarding z akceptacją Polityki Handmade i danymi DAC7 (Sekcje „Definicja »handmade«", „Zgodność prawna PL/UE").
- **Kupujący** — klient szukający unikalnych, ręcznie robionych produktów z Polski; konto z historią zamówień (Sekcja „Zakres funkcjonalny").

**Role operacyjne (po stronie platformy):**
- **Operator platformy** — właściciel biznesowy: polityki, prowizja, decyzje produktowe, panel admina (Sekcja „Zakres funkcjonalny").
- **Moderator** — weryfikacja ofert (Sekcja „Definicja »handmade«"), obsługa zgłoszeń i kolejki moderacji (Sekcja „Zaufanie i bezpieczeństwo").
- **Obsługa klienta / support** — rozstrzyganie sporów, pomoc kupującym i sprzedawcom (Sekcja „Zaufanie i bezpieczeństwo").

**Uczestnicy zewnętrzni:** dostawca płatności (rozliczenia, KYC, payout — Sekcja „Płatności, payout, escrow"), przewoźnicy (Sekcja „Wysyłka i zwroty"), podprocesorzy danych (Sekcja „Zgodność prawna PL/UE").

**MVP:** role operacyjne (operator, moderator, support) pełni ten sam mały zespół — rozdział ról i uprawnień w panelu admina przewidziany w roadmapie.

## Wymagania niefunkcjonalne

**Wydajność:** szybkie ładowanie stron produktu i kategorii oraz wyszukiwarki (cele liczbowe, np. LCP < 2,5 s — do ustalenia). Wydajność jest też wymogiem SEO.

**Dostępność (uptime):** priorytet dla ścieżki checkout/płatność; docelowy SLA — do ustalenia.

**Bezpieczeństwo:**
- Dane kart **nie są przechowywane** — obsługuje je dostawca płatności (PCI po jego stronie, Sekcja „Płatności, payout, escrow").
- HTTPS wszędzie, hashowanie haseł, ochrona przed OWASP Top 10, rate limiting, ochrona danych osobowych (Sekcja „Zgodność prawna PL/UE").

**Dostępność cyfrowa:** zgodność z **WCAG 2.1 AA** (również wymóg Europejskiego Aktu o Dostępności dla e-commerce w UE).

**SEO (krytyczne dla pozyskania kupujących):**
- Strony produktów i kategorii **indeksowalne**, dane strukturalne (schema Product/Offer), mapy strony, czytelne URL-e.
- Obecne `noindex,nofollow` w [index.html](index.html) i `Disallow: /` w [robots.txt](robots.txt) obowiązują **wyłącznie przed startem** — muszą zostać zdjęte na produkcji.

**Mobile:** podejście mobile-first (kupujący przeglądają na telefonach); aplikacja natywna — roadmapa (Sekcja „Wersje i roadmapa").

**i18n:** architektura gotowa na wielojęzyczność; MVP wyłącznie PL/PLN (Sekcja „Persony i rynek docelowy").

**Analityka i monitoring:** zdarzenia i lejki pod metryki z Sekcji „Cele i metryki sukcesu", monitoring błędów i alerty.

## Go-to-market i cold start

**Problem chicken-and-egg:** marketplace potrzebuje jednocześnie podaży (twórcy) i popytu (kupujący); żadna strona nie przychodzi bez drugiej.

**Strategia: supply-first.** Najpierw budujemy podaż — twórcy rękodzieła mają własną publiczność (Instagram/Facebook), więc przyciągają też pierwszy popyt.

**Pozyskanie podaży:**
- Targetowanie twórców niezadowolonych z prowizji Pakamera/Artillo (~25%) — pozycjonowanie „uczciwa prowizja" ([monetyzacja.md](monetyzacja.md)).
- **Promocja startowa 0% prowizji** dla pierwszych N sprzedawców / 3 mies. (Sekcja „Model biznesowy i prowizja").
- Asystowany onboarding pierwszych twórców (white-glove), kuracja oferty startowej.

**Pozyskanie popytu:**
- SEO jako główny kanał długoterminowy (Sekcja „Wymagania niefunkcjonalne").
- Twórcy przyciągają własnych odbiorców — udostępnialny link do sklepu sprzedawcy działa też **bez płynności marketplace** (wartość „single-player").
- Treści/social/PR wokół narracji „uczciwa prowizja".

**Gęstość zamiast szerokości:** start z **wąskim zestawem kategorii** (większa gęstość oferty i konwersja) zamiast rozproszenia po wszystkich.

**Sekwencja startu:** zamknięta beta sprzedawców (invite) → soft launch → otwarty start. Kryteria przejścia powiązane z metrykami płynności i liczbą aktywnych sprzedawców (Sekcja „Cele i metryki sukcesu").

## Pozycjonowanie i konkurencja

**Pozycjonowanie:** najuczciwsza prowizyjnie i najbardziej zaufana platforma polskiego rękodzieła — dla twórców oddających dziś ~1/4 ceny konkurencji i dla kupujących, którzy chcą mieć pewność, że kupują prawdziwe handmade.

**Filary różnicujące:**
1. **Gwarancja autentyczności handmade** — weryfikacja i moderacja (Sekcja „Definicja »handmade«"). Główny, trudny do skopiowania wyróżnik.
2. **Uczciwa, przejrzysta prowizja** — ~10% all-in vs 19–25% u polskiej konkurencji (Sekcja „Model biznesowy i prowizja", [monetyzacja.md](monetyzacja.md)).
3. **Dedykacja rynkowi PL** — język, płatności (BLIK), wysyłka (Paczkomaty), wsparcie po polsku — w przeciwieństwie do globalnego Etsy.

**Krajobraz konkurencyjny** (dane i źródła: [monetyzacja.md](monetyzacja.md)):
- **Polskie platformy handmade** (Pakamera, Artillo, Decobazaar, Art-Madam) — drogie (19–25%).
- **Etsy** — globalny, obecnie najtańszy dla polskich twórców, ale nieoptymalizowany pod rynek PL.
- **Allegro Lokalnie** — ogólny, nie dedykowany rękodziełu, brak gwarancji autentyczności.
- **Instagram / własne sklepy twórców** — rozproszone, brak zaufania, płatności i ochrony transakcji.

**Uczciwość pozycjonowania:** wobec Etsy przewagą NIE jest sama cena (Etsy bywa tańsze), lecz dedykacja PL + gwarancja handmade. Komunikacja nie może opierać się wyłącznie na „najtańsi".

## Ryzyka, założenia, zależności

**Ryzyka (z mitygacją):**

| Ryzyko | Waga | Mitygacja |
|---|---|---|
| Cold start się nie domyka (brak podaży/popytu) | Egzystencjalne | Supply-first, promocja 0%, single-player (Sekcja „Go-to-market i cold start") |
| Erozja autentyczności (masówka/odsprzedaż przechodzi) | Egzystencjalne | Weryfikacja i egzekwowanie (Sekcje „Definicja »handmade«", „Zaufanie i bezpieczeństwo") |
| Nierentowność przy niskim AOV (10% − PSP za mało) | Wysoka | Opłata minimalna, kontrola kosztów (Sekcja „Model biznesowy i prowizja") |
| Niezgodność prawna (DAC7/RODO/DSA/konsument) blokuje start | Wysoka | Wymagania Sekcji „Zgodność prawna PL/UE" + radca prawny |
| Status instytucji płatniczej | Wysoka | Split/marketplace u dostawcy (Sekcja „Płatności, payout, escrow") |
| SEO nie dowozi popytu → CAC rośnie | Średnia | Twórcy wnoszą publiczność, single-player (Sekcja „Go-to-market i cold start") |
| Odpływ sprzedawców po końcu promocji 0% | Średnia | Utrzymanie przewagi cenowej, retencja (Sekcje „Model biznesowy i prowizja", „Cele i metryki sukcesu") |
| Ręczna moderacja/support nie skaluje się | Średnia | Moderacja ryzykowo-reaktywna, roadmapa automatyzacji (Sekcje „Definicja »handmade«", „Zaufanie i bezpieczeństwo", „Role i uczestnicy") |

**Założenia:** twórcy są dość wrażliwi cenowo, by przejść z Pakamera/Artillo; wnoszą własną publiczność; take rate ~10% jest akceptowalny i rentowny; zakres MVP (tylko PL) wystarcza do walidacji; ręczna moderacja/support jest wykonalna w skali MVP.

**Zależności:** dostawca płatności z modelem marketplace + KYC + obsługą DAC7 (Sekcje „Płatności, payout, escrow", „Zgodność prawna PL/UE"); radca prawny (Sekcja „Zgodność prawna PL/UE"); integracje przewoźników (Sekcja „Wysyłka i zwroty", roadmapa); hosting/infrastruktura.

## Poza zakresem (non-goals)

Świadomie **nie** robimy w MVP (zapobiega rozjazdowi zakresu; każdy punkt wynika z decyzji w sekcjach):

- **Sprzedaż zagraniczna**, kupujący spoza PL, wielojęzyczność, waluty inne niż PLN (Sekcje „Persony i rynek docelowy", „Wymagania niefunkcjonalne").
- **Logistyka platformy**: magazynowanie, fulfillment, własne etykiety i integracja przewoźników (Sekcja „Wysyłka i zwroty").
- **Aplikacja natywna mobilna** — tylko web mobile-first (Sekcje „Zakres funkcjonalny", „Wymagania niefunkcjonalne").
- **Wiadomości kupujący–sprzedawca, lista życzeń, oceny dwukierunkowe** (Sekcje „Zakres funkcjonalny", „Zaufanie i bezpieczeństwo").
- **Prowizja różnicowana per kategoria** — jednolita stawka (Sekcja „Model biznesowy i prowizja").
- **Własny escrow / status instytucji płatniczej** — wyłącznie przez dostawcę (Sekcja „Płatności, payout, escrow").
- **Platforma jako strona umowy sprzedaży** — pozostajemy pośrednikiem; sprzedaż i faktura po stronie twórcy (Sekcja „Zgodność prawna PL/UE").
- **Automatyczna/AI weryfikacja handmade** — w MVP ręcznie i reaktywnie (Sekcje „Definicja »handmade«", „Zaufanie i bezpieczeństwo").
- **Subskrypcje, opłaty za listing, płatne wyróżnienia/reklamy** — model wyłącznie prowizyjny (Sekcja „Model biznesowy i prowizja").
- **Społeczność/treści** (blog, forum) poza minimalnym PR (Sekcja „Go-to-market i cold start").

## Wersje i roadmapa

**Prototypy a MVP:** [v1/index.html](v1/index.html) (strona statyczna) i [v2/index.html](v2/index.html) (klikalny prototyp: sklep + panel sprzedawcy) to **eksploracja UX**, nie kod docelowy. Zakres produktu wiążąco definiuje Sekcja „Zakres funkcjonalny". Obecne [index.html](index.html) to wewnętrzny selektor wersji (noindex), **nie** docelowy landing page.

**Fazy:**
- **Faza 0 — Prototypy i walidacja UX** *(w toku, niezakończona)*: v1/v2 jako eksploracja przepływów; walidacja jeszcze nieukończona. Faza bieżąca.
- **Faza 1a — Landing + zamknięta beta podaży:**
  - **Marketingowy landing page** — propozycja wartości „uczciwa prowizja", zapis twórców na listę oczekujących/onboarding. **Potrzebny i wcześniej niż marketplace** — supply-first (Sekcja „Go-to-market i cold start") wymaga miejsca do rekrutacji sprzedawców i startu SEO (Sekcja „Wymagania niefunkcjonalne"), zanim istnieje płynność.
  - Minimalne strony prawne wymagane przed jakąkolwiek rejestracją: Regulamin, Polityka Prywatności, Polityka Handmade (Sekcje „Definicja »handmade«", „Zgodność prawna PL/UE").
  - Analityka i lejek zapisu (Sekcja „Cele i metryki sukcesu").
- **Faza 1b — MVP marketplace** *(zakres: Sekcja „Zakres funkcjonalny")*: pełny sklep + panel sprzedawcy + transakcje; sekwencja zamknięta beta → soft launch → otwarty start; bramki = kryterium sukcesu MVP (Sekcje „Cele i metryki sukcesu", „Go-to-market i cold start").
- **Faza 2+ — Roadmapa post-MVP** (kierunkowa, zależna od walidacji MVP): sprzedaż zagraniczna / wielojęzyczność / wielowalutowość; integracja przewoźników i etykiety; aplikacja natywna mobilna; wiadomości kupujący–sprzedawca, lista życzeń, oceny dwukierunkowe; prowizja różnicowana; automatyzacja/AI weryfikacji handmade; granularne role w panelu admina; Apple/Google Pay, zaawansowane filtry.

Roadmapa kierunkowa — bez twardych dat; priorytety po walidacji MVP.

## Słownik skrótów i pojęć

**Skróty:**

- **PRD** — Product Requirements Document; dokument wymagań produktu.
- **MVP** — Minimum Viable Product; produkt o minimalnej koniecznej funkcjonalności do walidacji.
- **GMV** — Gross Merchandise Value; łączna wartość brutto zrealizowanych zamówień.
- **AOV** — Average Order Value; średnia wartość zamówienia (koszyka).
- **CAC** — Customer Acquisition Cost; koszt pozyskania klienta.
- **KYC** — Know Your Customer; weryfikacja tożsamości sprzedawcy/klienta.
- **PSP** — Payment Service Provider; dostawca usług płatniczych.
- **PCI (PCI DSS)** — Payment Card Industry Data Security Standard; standard bezpieczeństwa danych kart płatniczych.
- **DAC7** — unijna dyrektywa (2021/514) nakładająca na operatorów platform cyfrowych obowiązek zbierania i raportowania danych sprzedawców do administracji skarbowej.
- **RODO** — Rozporządzenie o Ochronie Danych Osobowych; unijne ogólne rozporządzenie o ochronie danych (ang. GDPR).
- **DSA** — Digital Services Act; unijny Akt o usługach cyfrowych (obowiązki platform pośredniczących).
- **GPSR** — General Product Safety Regulation; unijne rozporządzenie o ogólnym bezpieczeństwie produktów.
- **KAS** — Krajowa Administracja Skarbowa.
- **VAT** — podatek od towarów i usług (Value Added Tax).
- **NIP** — Numer Identyfikacji Podatkowej.
- **PESEL** — numer ewidencyjny osoby fizycznej.
- **WCAG** — Web Content Accessibility Guidelines; wytyczne dostępności cyfrowej.
- **EAA** — European Accessibility Act; Europejski Akt o Dostępności.
- **SEO** — Search Engine Optimization; optymalizacja widoczności w wyszukiwarkach.
- **LCP** — Largest Contentful Paint; metryka szybkości ładowania (Core Web Vitals).
- **OWASP** — Open Worldwide Application Security Project; „OWASP Top 10" to lista najczęstszych podatności aplikacji webowych.
- **HTTPS** — szyfrowany protokół przesyłania danych w sieci.
- **i18n** — internacjonalizacja; przygotowanie architektury pod wiele języków.
- **UX** — User Experience; doświadczenie użytkownika.
- **PR** — public relations; działania komunikacyjno-wizerunkowe.
- **AI** — sztuczna inteligencja.
- **BLIK** — polski system płatności mobilnych.

**Pojęcia:**

- **North Star (metryka)** — pojedyncza, nadrzędna metryka kierunkowa dla całego produktu.
- **Chicken-and-egg** — problem „jajko i kura": brak popytu bez podaży i odwrotnie.
- **Supply-first** — strategia rozruchu marketplace od strony podaży (najpierw sprzedawcy).
- **Single-player (wartość)** — użyteczność produktu dla pojedynczego użytkownika, działająca bez efektu sieci.
- **Escrow / escrow-light** — rachunek powierniczy; „light" = zwolnienie środków po potwierdzeniu odbioru lub po upływie czasu.
- **All-in (prowizja)** — stawka łączna obejmująca wszystkie składniki (prowizja platformy + koszt płatności).
- **Chargeback** — obciążenie zwrotne; cofnięcie płatności kartą przez bank kupującego.
- **Clawback** — potrącenie wcześniej wypłaconych środków z kolejnych wypłat sprzedawcy.
- **Notice-and-takedown / notice-and-action** — procedura zgłoszenia i usunięcia bezprawnej treści/oferty.
- **Pay-by-link** — płatność szybkim przelewem realizowana przez wygenerowany link.
- **White-glove (onboarding)** — indywidualne, asystowane wdrożenie pierwszych sprzedawców.
- **Reverse image search** — wyszukiwanie wstecz po obrazie (wykrywanie zdjęć skopiowanych z katalogów).
