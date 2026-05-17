# Monetyzacja — analiza wysokości prowizji

> Uzupełnienie do [PRD.md](PRD.md). PRD mówi „we earn a margin on each completed sale" / „takes a commission",
> ale nie podaje liczby. Ten dokument proponuje konkretną stawkę w oparciu o benchmarki rynkowe.
> Dane zebrane: 2026-05-17.

## TL;DR — rekomendacja

**Prowizja docelowa: ~10% wartości zamówienia (all-in), w modelu: 7–8% prowizji platformy + przeniesiony koszt płatności (~2–3%).**

- Rynek polskich platform handmade jest **drogi** (Pakamera ~24,5%, Artillo ~25%, Decobazaar ~19%). To jest realna przewaga konkurencyjna do wykorzystania.
- Globalny benchmark efektywny (Etsy all-in) to ~10–12%.
- ~10% pozwala być **wyraźnie tańszym od polskiej konkurencji** i jednocześnie pokryć koszty operacji i płatności. Schodzenie poniżej ~8% all-in zagraża rentowności przy niskich kwotach koszyka typowych dla rękodzieła.

## Benchmarki rynkowe (2026)

### Platformy globalne

| Platforma | Prowizja od transakcji | Płatności | Inne | Efektywnie all-in |
|---|---|---|---|---|
| Etsy | 6,5% | ~4% + €0,30 (EU) | $0,20 / listing co 4 mies. | ~11–13% |
| Amazon Handmade | 15% (referral, flat) | wliczone | listing free | ~15% |
| eBay | ~13% | wliczone | — | ~13% |
| Allegro Lokalnie | 7,9% | zależnie | — | ~8–11% |

### Platformy polskie (rękodzieło) — źródło: Bankier

| Platforma | Prowizja |
|---|---|
| Artillo.pl | ~25% |
| Pakamera.pl | ~24,5% brutto |
| Decobazaar.pl | ~19% brutto |
| Art-Madam.pl | ~18,7% netto |
| Etsy (dla polskich twórców) | najtańsza opcja na rynku PL |

Wniosek: polscy gracze handmade biorą **2–3× więcej niż Etsy**. Twórcy oddają nawet 1/4 ceny produktu. To jest dokładnie ta bolączka, na której można zbudować pozycjonowanie „uczciwa prowizja".

## Czego nie wolno pominąć — koszt płatności

Prowizja brutto ≠ marża. Z każdej transakcji trzeba pokryć operatora płatności (Przelewy24 / Stripe / PayU w PL): zwykle **~1,5–3% + opłata stała**. Jeśli prowizja platformy wynosi np. 8%, a płatności zjadają 2,5%, realna marża to ~5,5% — i z tego trzeba sfinansować zwroty, chargebacki, obsługę sporów i hosting.

Dwa możliwe modele:
1. **All-in 10%** — kupujący/sprzedawca widzi jedną stawkę, platforma absorbuje koszt PSP. Prościej komunikować.
2. **Prowizja platformy 7–8% + payment processing osobno (~2–3%)** — przejrzyste, model Etsy. Łatwiej utrzymać marżę, gdy rosną koszty PSP.

Rekomendacja: **model 2** (przejrzysty, odporny na wzrost kosztów płatności), komunikowany na zewnątrz jako „~10% i nic poza tym".

## Uzasadnienie rekomendowanego ~10%

- **Konkurencyjność:** ~2,5× taniej niż Pakamera/Artillo → mocny argument akwizycyjny dla sprzedawców (kluczowe przy problemie chicken-and-egg z PRD).
- **Rentowność:** po odjęciu PSP zostaje ~7–8% na pokrycie kosztów i marży — wystarczająco przy świadomej kontroli kosztów.
- **Spójność z PRD:** model „listing free, revenue from transactions" działa tylko jeśli take rate pokrywa też koszt darmowych, nieskonwertowanych listingów. ~10% to robi; 5% prawdopodobnie nie.
- **Niskie koszyki rękodzieła:** przy zamówieniu 60–150 zł opłaty stałe (PSP) silnie obciążają — argument za niezbyt niską stawką procentową i ewentualną opłatą minimalną.

## Otwarte decyzje do podjęcia (poza tym dokumentem)

1. **All-in vs. rozdzielone** prowizja + płatności (rekomendacja: rozdzielone).
2. **Opłata minimalna** od transakcji (np. min. 2–3 zł), by małe koszyki nie były stratne.
3. **Kto płaci prowizję** — potrącana sprzedawcy z payoutu (standard marketplace) vs. doliczana kupującemu.
4. **Stawki różnicowane?** Niższa prowizja dla kategorii premium / wyższych koszyków, by przyciągnąć wartościowych sprzedawców.
5. **Przepływ pieniędzy / payout** — escrow do potwierdzenia dostawy vs. szybka wypłata; polityka zwrotów i chargebacków. (To wykracza poza prowizję, ale determinuje realny koszt.)
6. **Promocja startowa** — np. 0% prowizji dla pierwszych N sprzedawców / przez pierwsze 3 mies., żeby rozruszać podaż.

## Źródła

- [Etsy Seller Fees 2026 — Craftybase](https://craftybase.com/blog/the-complete-guide-to-etsy-fees)
- [Etsy Fees Explained 2026 — Printify](https://printify.com/blog/how-much-does-etsy-take-per-sale/)
- [Amazon Handmade vs Etsy 2026 — Printify](https://printify.com/blog/amazon-handmade-vs-etsy/)
- [Etsy vs eBay Fees 2026 — Webgility](https://www.webgility.com/blog/etsy-vs-ebay)
- [Prowizje platform handmade PL — Bankier.pl](https://www.bankier.pl/wiadomosc/Jaka-prowizja-w-Pakamera-pl-Decobazaar-pl-Art-Madam-pl-Etsy-com-Artillo-pl-7777156.html)
- [Prowizje Allegro 2026 — sky-shop.pl](https://blog.sky-shop.pl/prowizje-allegro-wszystko-co-musisz-wiedziec/)
