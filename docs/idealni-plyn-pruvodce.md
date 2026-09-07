# Plyn pod lupou – průvodce pro vyučujícího

Spuštění: otevřete `idealni-plyn.html` dvojklikem v běžném prohlížeči. Samotný tento soubor stačí i po zkopírování jinam; nepotřebuje instalaci, server, účet ani připojení. Odkaz na rozcestník funguje, pokud vedle zůstane `index.html`. Pro zveřejnění je soubor připraven ve stávající složce `docs`; během této práce nebylo provedeno publikování.

## Průběh na 2 × 45 minut

| Čas | Činnost | Hlavní ověření |
| --- | --- | --- |
| 0–5 min | Start, orientace a příprava sešitu | Student rozumí postupu odhad → pokus → závěr. |
| 5–20 min | Molekuly, změna T, V, n a plynu | Tlak, rozdělení rychlostí, energie a vₖ. |
| 20–45 min | Stavová rovnice a čtyři výpočty | Kelvin, SI, n/m/N a dva stavy. |
| 45–65 min | Čtyři děje, tři grafy, měření | Co je konstantní, práce jako plocha, Q a ΔU. |
| 65–80 min | Carnotův cyklus a reálné motory | Směr cyklu, chladič, účinnost, pracovní zdvih. |
| 80–90 min | Výstupní příklad a protokol | V₂ = 7,50 l, W = +250 J, Q = +625 J; graf a vlastní vysvětlení. |

Student potřebuje sešit a kalkulačku. Kapitoly lze otevírat v libovolném pořadí. Režim projektoru zvětšuje text i popisky grafů. Posuvníky podporují klávesnici. Animaci lze zastavit; při systémové preferenci omezeného pohybu začíná zastavená.

## Vazba na dodanou prezentaci

| Snímky PDF | Obsah aplikace |
| --- | --- |
| 3–9 | Model ideálního plynu, pohyb, prostorová hustota, Maxwellovo rozdělení, vₖ, translační energie, tlak a fluktuace. |
| 10–13 | Všechny tvary stavové rovnice, n = m/M, N = nNₐ, převody a řešené příklady. |
| 14–27 | Izoterma, izochora, izobara, adiabata, Poissonův zákon, p–V/p–T/V–T grafy, energetické důsledky. |
| 28–40 | Práce plynu, plocha pod křivkou a uvnitř cyklu, Carnotův cyklus, účinnost a druhý zákon. |
| 41–50 | Parní, zážehový, vznětový, dvoudobý, Wankelův motor a plynová turbína; interaktivní fáze čtyřdobého motoru. |

Historická data a videa nejsou předmětem hodnocení. Materiál funguje bez videí a bez externích knihoven. Ilustrace a grafy jsou původní, kreslené přímo v aplikaci.

## Výslovná didaktická rozhodnutí

- Celkem 20 kontrolovaných úloh, bez klasifikační známky a časového stresu. Nesprávné odpovědi mají vysvětlení a lze je opravit. Po změně číselné odpovědi je nutné znovu použít Ověřit.
- Závěrečný příklad je společný pro celou třídu, aby šly porovnat postupy. Samotné číslo nenahrazuje výpočet, graf a vysvětlení v sešitě.
- Číselná tolerance je obvykle 1,5 %, u převodu kelvinů 0,1 %. Podporována je česká desetinná čárka a vědecký zápis, například `2,42e22`.
- Energetické simulace používají jednoatomový plyn: U = 3nRT/2 a κ = 5/3. Student vidí omezení přímo v zadání. Víceatomové molekuly jsou vysvětleny samostatně.
- W je vždy práce vykonaná plynem; ΔU = Q − W. Tím se sjednocují nejednotná znaménka u adiabat v prezentaci. Q₁ a Q₂ u motoru označují kladné velikosti tepla.
- Maxwellova křivka je teoretické 3D rozdělení. Názorná animace je 2D a neřeší vzájemné srážky částic. Tuto skutečnost přiznává studentovi.
- Dvoudobý motor nemá obecně přesně dvojnásobný výkon. Převzata je správná souvislost s četností pracovních zdvihů, nikoli paušální výkonový poměr z prezentace.

## Výsledek a soukromí

Aplikace nezjišťuje jméno, nepoužívá cookies, úložiště prohlížeče, analytiku ani síťová API. Odpovědi jsou jen v paměti otevřené stránky. Obnovením nebo zavřením se ztratí; tato informace je uvedena na začátku i na konci. Student může výsledek s vysvětlením a měřeními exportovat jako text nebo otevřít tiskový dialog. Nápověda nepenalizuje; otevření plného řešení se uvádí v bilanci. Volné vysvětlení se automaticky nehodnotí.

## Provedené ověření

- V prohlížeči prošly všechny kapitoly i všech 20 úloh až do stavu 20/20; testovány byly prázdné odpovědi, nečíselný text, chybné znaménko, Celsia místo kelvinů, záměna Pa/kPa, vědecký zápis a změna již správné odpovědi.
- Vyzkoušena navigace přímo na závěr a zpět, přepínání grafů a dějů, komprese, expanze, návrat do A, zápis měření, limit osmi záznamů i jejich vymazání.
- Projity všechny fáze Carnotova i čtyřdobého motoru. Ověřena změna účinnosti s teplotou chladiče.
- Samostatná kontrola JavaScriptu ověřuje 20 kombinací dějů a koncových stavů, stavovou rovnici, první zákon, kontinuitu Carnotova cyklu a shodu numerické plochy cyklu s prací pro tři dvojice teplot. Ověřen je i obsah serializovaného textového protokolu.
- Při vizuální kontrole byla opravena příliš široká mobilní navigace, zvětšeny popisky pro projektor, rozšířen rozsah rychlostí pro horké helium a odstraněno nepřesné zaokrouhlování dílků os. Tiskový přehled výslovně obsahuje zadané závěrečné hodnoty i jejich stav.
- Testovací vestavěný prohlížeč blokuje URL `file://`, takže vizuální zkoušky proběhly přes dočasný server na adrese 127.0.0.1, zpřístupňující jen vyjmenované soubory projektu. Přímý dvojklik v běžném externím prohlížeči zde nebyl proveden; samostatnost byla ověřena kontrolou všech závislostí (žádné knihovny, importy, síťové požadavky ani načítané fonty).

## Volitelný námět navíc

Před simulací lze zařadit krátký pokus se stříkačkou bez jehly: pomalé a rychlejší stlačení uzavřeného vzduchu. Studenti nejprve odhadnou, zda bude konečný tlak stejný, a potom rozdíl vysvětlí pomocí tepelné výměny. Není to nutná součást aplikace ani hodnocení.
