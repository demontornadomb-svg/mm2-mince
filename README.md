# MM2 Mince 🪙

Osobní projekt pro Windows, který pomocí obrazu hledá mince v Murder Mystery 2 a zkouší k nim ovládat postavu. Rozpoznávání i řízení běží lokálně; Codex ani ChatGPT při používání nepotřebuješ.

**Verze 3.4.0 je experimentální.** Obcházení překážek a skutečné sebrání mince nejsou zaručené. Poslední úpravy prošly offline testy, nikoli novým živým testem v Robloxu.

## Stažení

Na stránce projektu otevři **Releases**, vyber **3.4.0** a v části **Assets** stáhni **MM2-Mince-3.4.0.exe**. Volba „Source code (zip)“ obsahuje soubory této stránky, nikoli hotový program.

Program je zdarma ke stažení. EXE obsahuje potřebný Python a knihovny; nemusíš je zvlášť instalovat. Je určený pro 64bitový Windows. Na jiných počítačích zatím nebyl ověřený.

## Použití

1. Spusť EXE. Po otevření je automatický pohyb vypnutý.
2. Otevři Murder Mystery 2, nech kameru za postavou a zavři herní chat i nabídky. Doporučené nastavení je Classic bez Shift Lock.
3. Zapni sbírání tlačítkem v aplikaci nebo klávesou **F8** ve hře.
4. **F8** přepíná spuštění a pauzu. **F9 nebo Esc** zastaví ovládání. Přepnutí do jiného okna zastaví automatický pohyb také.

Záložka manuálního tréninku umožňuje ukládat vlastní snímky a pozorované vstupy. Samotné zaznamenávání hraní nevytváří naučenou mapu a automaticky nepřepisuje pravidla chůze. Záznamy se ukládají místně do uživatelských dat aplikace, ne dovnitř EXE.

## Co se změnilo ve 3.4.0

- Vybraná mince zůstává cílem při krátkém obcházení překážky přes ověřovaný průchod.
- Při srovnání s průchodem se boční pohyb zastaví; další snímek ověří krok dopředu.
- Staré a opakované snímky nemohou potvrdit úspěšné obejití.
- Změna pohledu kamery ruší předchozí krátkodobou paměť překážky.
- Náhled ukazuje aktuální mezibod průchodu, pokud ho řízení dostatečně podporuje.

## Ověření a omezení

Prošlo **342 automatických testů** a offline test sestaveného EXE ověřil rozpoznání ukázkové mince, inicializaci ovladače a vytvoření skrytého testovacího okna. To neprokazuje správnou chůzi, vyhýbání zdím ani sebrání mincí v živé hře.

V porovnání 22 rozšířených modelových tras dosáhla předchozí i nová verze cílové vzdálenosti v 17 případech. Model používá podněty, které jsou spolehlivější než skutečné rozpoznávání z obrazovky. Program proto zatím není spolehlivý navigátor všech map.

EXE není digitálně podepsané. Windows může spuštění blokovat; nevypínej kvůli tomu Defender ani jiné ochrany. Kontrolní součet **SHA256SUMS.txt** umožňuje ověřit shodu souboru s vydáním, sám o sobě nedokazuje bezpečnost.

## Soukromí

Zpracování herního obrazu probíhá na počítači. Aplikace nevyžaduje přihlašovací údaje k Robloxu. Veřejné vydání neobsahuje moje tréninkové relace, osobní nastavení ani původní videa. EXE obsahuje vestavěný ukázkový herní snímek a obrazové reference mincí.

## Podpora projektu ⭐

Pokud tě projekt zaujal, budu rád za **Star ⭐ vpravo nahoře**. Je to bezplatný způsob, jak projektu na GitHubu vyjádřit podporu. Můžeš také napsat do **Issues**, co nefunguje, a připojit verzi aplikace a stručný popis problému. Do hlášení nevkládej hesla ani osobní údaje.

Díky za vyzkoušení a zpětnou vazbu! Na programu se postupně pracuje.

## Vztah ke hře

Jde o neoficiální osobní projekt, který není spojený s Robloxem ani tvůrci Murder Mystery 2. Herní názvy a obrazové podklady patří příslušným vlastníkům. Možnost stažení není potvrzením, že použití automatizace dovolují pravidla konkrétní hry.
