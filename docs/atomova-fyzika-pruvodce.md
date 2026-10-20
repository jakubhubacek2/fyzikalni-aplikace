# Uvnitř atomu

Otevřete soubor **atomova-fyzika.html** dvojklikem v běžném webovém prohlížeči. Celá aplikace je v tomto jediném souboru; ke spuštění nepotřebuje server, instalaci, účet ani připojení. Při kopírování na jiný počítač nebo mobil stačí předat HTML soubor. Náhledy příloh v některých mobilních aplikacích JavaScript nespouštějí; je potřeba skutečný prohlížeč s podporou místních HTML souborů.

## Co obsahuje

- Otevřenou mapu pěti témat s doporučenou cestou; témata nejsou uzamčená postupem.
- Pět historických představ o atomu, schéma Rutherfordova pokusu a skládání kvantového oblaku z výsledků měření.
- Kontrolu čtveřic kvantových čísel včetně neplatných kombinací, názorné typy orbitalů a úkol s Pauliho principem.
- Animované energetické přechody vodíku: přílet a pohlcení správného fotonu, průchod nesprávného fotonu, emisi a odlet fotonu. Animaci lze pozastavit, zpomalit, krokovat a zopakovat se znovu připraveným počátečním stavem.
- Devět spektrálních vzorků: vodík, sodík, helium, atomární kyslík O, molekulární kyslík O₂, neon, argon, rtuť a vzduch. Srovnávací pohled, dotyková sonda, výběr čar tlačítky a vypínání příspěvků ve schématu vzduchu.
- Kvalitativní model laseru s čerpáním, populační inverzí a vypínáním optické zpětné vazby.
- Deset průběžných a pět závěrečných otázek se zdůvodněním odpovědí, vlastní závěrečné vysvětlení.
- Metodiku, časový plán, vysvětlení zjednodušení a zdroje přímo v části **Pro učitele**.

## Rozhodnutí v otevřených částech zadání

Materiál staví na principu **předpověz → vyzkoušej → vysvětli**. Krátký základní výklad doplňují rozevírací podrobnosti. Ovládání funguje myší, dotykem i klávesnicí; pohyb lze zastavit. Na telefonu zůstává přepínač témat dostupný nahoře.

První hodina: úvod 5 min, modely 15 min, kvantová čísla 20 min, společné shrnutí 5 min. Druhá hodina: světlo 15 min, spektra 15 min, laser 10 min, závěrečné propojení 5 min. Doporučená je práce ve dvojicích se střídáním rolí.

Z dodané prezentace byly využity pouze snímky 1–39. Odborné doplnění vychází ze zdrojů OpenStax a NIST uvedených v aplikaci. Zpřesněno je datování Thomsonova modelu, role Sommerfeldova rozšíření, rozdíl orbital/orbit, zápis |ψ|² a rozlišení s od mₛ. Jaderná fyzika a radioaktivita nejsou zahrnuty.

Simulace jsou didaktické, nikoli výzkumné výpočty. Jejich omezení jsou uvedena u každého pokusu, zejména neměřítkové diagramy, rozšířené spektrální čáry, výběrová pravidla a kvalitativní práh laseru.

## Animace a rozšířená spektra

Přechod má tři fáze: přípravu/přílet fotonu, interakci a výsledek. Změna kvantového stavu je znázorněna zhasnutím značky v jednom a rozsvícením v druhém dovoleném stavu, nikoli spojitou dráhou elektronu. Základní animace trvá přibližně tři sekundy; skutečný děj je mnohem rychlejší. Barvy UV a IR fotonů jsou symbolické. Nastavení rychlosti ½×, 1× a 2× ovlivňuje jen názornost. Při pozastaveném pohybu nebo preferenci omezeného pohybu lze pokus dokončit tlačítkem Další krok. Během přechodu se nepřijímají další příkazy k absorpci či emisi; odchod do jiného tématu pokus přeruší bez změny původního stavu.

U sedmi atomových vzorků jsou uloženy vybrané vlnové délky neutrálních atomů z tabulek NIST. Jednotka Å byla převedena na nm dělením deseti. Šířky, barvy a stejné jasnosti čar jsou úprava pro obrazovku, nikoli měřené intenzity. Párový emisní/absorpční přehled idealizuje stejné přechody; skutečná absorpce navíc vyžaduje vhodné obsazení výchozích stavů.

O₂ ukazuje jen příklad molekulární absorpce. Pásy B přibližně u 687 nm a A přibližně u 760 nm vycházejí z MPI-Mainz UV/VIS atlasu a NASA/JPL. Ve vzduchu se při absorpci přidává názorná obálka vodní páry kolem 720 nm. Při emisi vzduchu se ukazuje jiná situace: excitované N₂, N₂⁺ a atomy O. Není to zrcadlový doplněk absorpce běžné atmosféry. Tvar pásů, jejich šířky a podíly složek jsou záměrně schématické a nejde o předpověď konkrétního výboje nebo skutečné atmosférické propustnosti. Primární zdroje jsou odkazované v části Pro učitele.

Pro základních 15 minut u spekter stačí vybrat tři badatelské úkoly. Srovnávání dalších vzorků lze využít jako volitelné rozšíření.

## Grafické sjednocení se školními aplikacemi

Vzhled vychází ze společného souboru `docs/spsei-theme.css`, který je v projektu označen jako odvozený z manuálu identity SPŠEI. Používá stejné základní hodnoty: modrou #47657d, tmavě modrou #213c50, limetkovou #dbf82a, světle šedou mřížku, hranaté panely a tlačítka, školní označení e1 a stejnou rodinu písma s místními náhradami. Soubor písma Lilex ve složce není; prohlížeč proto použije dostupné místní písmo ze společného seznamu (například Consolas).

Potřebné styly jsou vložené přímo v HTML, aby materiál zůstal přenositelný v jediném souboru. Sdílený styl ani jiné aplikace nebyly měněny. Barvy spektrálních čar a rozlišení správných a chybných odpovědí zachovávají svůj výukový význam.

Po sjednocení bylo znovu ověřeno všech osm obrazovek při šířkách 320, 390, 768, 1024 a 1280 px (40 kombinací), bez vodorovného přetékání celé stránky. Znovu byly vyzkoušeny neplatný i platný kvantový stav, odmítnutí nesprávného fotonu, správná absorpce, přepínání spekter a laser. Ovládání a výuková logika zůstaly zachované.

## Soukromí

Žádné sledování, analytika, síťová volání ani externí knihovny. Aplikace nevyžaduje jméno. V místním úložišti si pamatuje jen vyřešené otázky a závěrečnou poznámku, které lze vymazat v části Pro učitele. Pokud prohlížeč místní úložiště nepovolí, běží dál bez trvalého uchování. Vnější odkazy na zdroje se otevřou jen po výslovném kliknutí.

## Ověření a opravy

Celá aplikace byla 20. 10. 2026 projita v prohlížeči přes dočasný místní HTTP náhled. Automatizační prohlížeč nepovoluje adresy file://, takže samotný dvojklik nebyl přímo ověřen. Soubor neobsahuje importy, načítání dalších souborů ani funkce vyžadující server; připraven je pro přímé offline otevření.

Ověřeno:

- Všech pět historických modelů a jejich tlačítka.
- Neplatná l, mₗ i mₛ; platné 1s a 3d; opakované vložení stejného spinu a vyprázdnění orbitalu.
- Nesprávný foton 500 nm pro 2 → 3, prázdný vstup, správná absorpce, emise zpět, opakované kliknutí bez změny stavu a ultrafialový přechod 1 → 2.
- Všechny typy spekter, původní dva vzorky, oba směry pozorování a sonda; rozšíření na devět vzorků je ověřeno samostatně níže.
- Laser se slabým čerpáním, s inverzí a se zpětnou vazbou i bez ní.
- Všech 45 odpovědních možností v 15 otázkách; správné vyhodnocení, oprava odpovědi a ochrana proti opakovanému přičítání bodů.
- Uložení odpovědí a poznámky po obnovení stránky, vymazání a nový průchod.
- Všech osm obrazovek při šířkách 320, 390 a 768 px, bez vodorovného přetékání celé stránky; také běžné počítačové zobrazení.
- Přeskakování témat, mobilní přepínač a pozastavení pohybu.

Po kontrole byly opraveny barvy spojitého spektra vůči ose vlnových délek, drobné mobilní písmo, měřítko popisků diagramů, poměr stran laserového obrázku, stavový text laseru, odkaz Přejít k obsahu a plynulé posouvání, které mohlo kolidovat s rychlým přecházením mezi ovladači.

## Samostatný námět pro výuku

Navázat skutečným pozorováním spekter přes školní spektroskop a porovnáním s virtuální laboratoří. Jde o doplněk k aplikaci; není pro její použití nutný.
