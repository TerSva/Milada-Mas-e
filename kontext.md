# Milada / Floating Phoenix — kontext projektu (export 19. 8. 2026)

> Tento dokument **nahrazuje** `milada-projekt-kontext-2026-07-24.md`. Od 24. 7. přibyla finální sitemapa, kompletní obsahový plán, copy draft, odpovědi od Milady, a hotový design systém. Kde se něco změnilo oproti staré verzi, je to označené.

---

## 1. Základ projektu

- **Klient:** Milada, soloterapeutka (klasická + terapeutická masáž, Access Consciousness), Karlovy Vary.
- **Umbrella:** Floating Phoenix — sdílený prostor. Cross-link je mělký, jen v sekci "Kde mě najdeš", nikdy textově hlubší.
- **Workflow:** sitemap → obsahový plán → copy → typografie → wireframe → design & build. **Aktuální pozice: obsahový plán, copy draft a design systém hotové. Další krok: wireframe.**
- **Brand name — ZMĚNA:** Prozatím zůstává **"Masáže Milada"** (její vlastní jméno). Shortlist (Serena/Lumina/Sensu/Sense) byl poslán, ale rebrand se aktivně netlačí. Logo zatím nenavrženo.

---

## 2. Sitemap — FINÁLNÍ (krok 5/6 hotový)

One-pager, 6 anchorů v navigaci:

| # | Sekce | Fáze | Poznámka |
|---|---|---|---|
| 1 | Úvod / Hero | Příchod | Tagline, wordmark v nav (Karla, ne Fraunces) |
| 2 | O Miladě / Filozofie | Dotek | Osobní text + "čtyři kroky jedné návštěvy" |
| 3 | Služby | → Proměna | Viz sekce 4 níž — hybridní struktura |
| 4 | Ceník | — | **Není samostatná sekce** — scroll-target na konec Služeb |
| 5 | Kde mě najdeš | — | "Objednávejte se předem" (Milada nemá pevnou dobu) |
| 6 | Rezervace / kontakt | Odchod | Reservio embed + recenze (skryté, dokud nejsou) |

Funkční kotvy a emocionální oblouk (Příchod→Dotek→Proměna→Odchod) jsou dvě nezávislé vrstvy — fáze neběží jako vlastní anchory.

### Struktura sekce Služby — ROZHODNUTO (grilling)
**Hybrid:** 3 "subsection header" fotky (Tělo / Obličej / Access), pod každou čistý textový seznam služeb (název, čas, price-reveal na klik). Pořadí **Obličej → Tělo → Access** (fyziologická logika hlava→tělo→hloubka) potvrzeno jako platné, protože jde o 3 vizuálně oddělené bloky, ne karty bez pořadí.

**Access Consciousness:** Na web jdou jen **2 hlavní položky** — Access Bars a Access Facelift (z původních 12). Sekce se nejmenuje "Access Consciousness" navenek — vlastní lidský název je primární, "(Access Consciousness)" jde jako tichý dodatek v závorce. Stejný vzorec pro obě položky: lidský popis primárně, technický název v závorce.

**Price-reveal:** Každá služba má "cena" label, který se **kliknutím** (ne hoverem) promění v částku. Na mobilu zůstává odhalená natrvalo.

---

## 3. Kompletní seznam služeb (od Milady, 3. 8. 2026)

**Tělo:** Klasická masáž (Relaxační / Regenerační; lze dělit i podle partie — záda/šíje, dolní končetiny, horní končetiny, celotělová), Aromaterapeutická masáž, Lymfatické masáže.

**Obličej:** Ošetření a masáž obličeje, Měkké a mobilizační techniky, Bukální a liftingová masáž obličeje, Masáže obličeje myofasciální techniky a bukální masáž.
> *Poznámka: poslední dvě položky nejsou duplicita — Milada má na ně dva různé kurzy/certifikace, proto podobná jména. Sama je přejmenuje pro jasné odlišení.*

**Access Consciousness (na web jen 2):** Access Bars, Access Facelift.

### Čeká se od Milady:
- Přejmenování dvou bukálních procedur
- Časy a ceny ke **všem** procedurám
- Vlastní popisky (lidským jazykem) k Access Bars a Access Facelift

---

## 4. Copy draft (napsáno, čeká na revizi + reálná čísla)

**Hero:** *"Masáže Milada — Místo, které tě najde. Klasická i terapeutická péče pro tělo i mysl, v Karlových Varech."*

**O Miladě:** *"Jsem Milada a masážím s citem pro to, co vaše tělo právě potřebuje — ať je to hluboké uvolnění, nebo cílená regenerace po zátěži. Každé setkání přizpůsobím vám, ne šabloně."*

**Čtyři kroky jedné návštěvy** (beze změny z brand dokumentu):
1. Příchod — Přicházíte zatížení. Tohle místo vás uzemní.
2. Dotek — Ruce pracují. Energie proudí — cítíte to, neřešíte to.
3. Proměna — Uvolní se víc než sval. Jako vzduch po bouřce.
4. Odchod — Odcházíte lehčí. A víte, že se chcete vrátit.

**Kde mě najdeš:** *"Najdete mě v Karlových Varech, v prostoru Floating Phoenix. Objednávejte se předem — bez pevné otevírací doby, ale s časem, který bude patřit jen vám."* + mělký cross-link na Floating Phoenix.

**Rezervace:** *"Odcházíte lehčí. A víte, že se chcete vrátit."* + Reservio CTA.

> Ceny/časy v draftu jsou ilustrační, zakotvené v cenách konkurence (KV region) — čekají na výměnu za realné podklady od Milady.

---

## 5. Design systém — HOTOVO jako samostatný artefakt

Soubor `design-system.html` — živý, interaktivní referenční dokument (ne statický obrázek). Klíčová rozhodnutí:

### Tokeny
- **Grid:** container 1280px, breakpointy mobil <640 / tablet 640–1024 / desktop >1024px.
- **Spacing:** 8px base scale (8/16/24/32/48/64/96), dotykové cíle min. 44×44px.
- **Radius:** **18px jednotně.** Plný pill (999px) vědomě zamítnut jako "AI-first" vzorec.
- **Typografie:** modulární scale 1.25 (12/14/16/20/28/40). **Fraunces jen pro Hero tagline**, nikde jinde — nahrazuje dřívější pravidlo "Fraunces na H1/H2". Vždy v extrémní poloze os, nikdy v pohodlném středu:
  - Dark headline: opsz 64 / wght 680 / SOFT 15 (řezaný, sochařský)
  - Light headline: opsz 14 / wght 300 / SOFT 90 (rozpuštěný, vzdušný)
  - Nav wordmark "Masáže Milada" = Karla, nikdy Fraunces.
- **Barvy — nové semantic dark-mode varianty:** success dark `#86AB66` (6.38:1), error dark `#C9866D` (5.65:1) — doplňují light-mode `#55733F`/`#804739`, které na dark bg nevyhovovaly.
- **Motion:** phase-transition 600–800ms ease-in-out (scroll-linked gradient), hover-micro 150–200ms, price-reveal 250ms (crossfade+slide, ne swap), cta-breathe ~950ms (jednorázový nádech), cta-glow 700ms (teplý halo kolem tlačítka, ne uvnitř — na oranžovém pozadí by byl jinak neviditelný), mobile-menu-expand 350ms.

### Komponenty
- **CTA:** kombinace dýchání (scale+lift) + halo glow. Focus = viditelný outline (WCAG). Disabled = decor barva + tlumený text.
- **Price-reveal row:** klik → crossfade+slide 250ms, revealed stav = tmavý bold text.
- **Subsection header:** foto + text VEDLE (nikdy overlay se scrimem).
- **Mobilní nav:** sticky hamburger s vlastní ikonou (tři vlnky, ne rovné čáry) — odkaz na "Klid" z moodboardu. Rozbalení dolů, 350ms ease-out.

### Ikony — 4 vlastní, hotové
Menu (vlnky), telefon, e-mail, lokace — ručně kreslené v Affinity, vyčištěné (sjednocená stroke-width 12 v 200×200 viewBox, `currentColor`). **Pravidlo: žádná generická knihovna** (Lucide/Feather/Heroicons/FontAwesome/Material — Lucide obzvlášť rizikové, je default v AI-scaffolding nástrojích). Ikony jen pro funkční nutnost (kontakt, nav toggle), nikdy dekorace. Velikosti: content 24px, nav/hamburger 28px.

### Textura
**Grain:** reálná lněná fotka (ne procedurální šum), **18% opacity, blend mode multiply/soft-light** (ne prostá opacity — chrání přísně monochromatickou paletu před šedým nádechem textury). Jen na plochy pozadí servisních sekcí, nikdy přes fotky.
**Organické křivky** (homepage/flow sekce): parkováno jako vlastní kreslený asset — Tereza si to vytvoří sama.

---

## 6. Otevřené body

| Stav | Položka |
|---|---|
| Otevřeno | Access naming pattern — přesná vazba na type scale (caption vs. small) |
| Parkováno | Organické křivky — vlastní kreslený asset (Tereza) |
| Parkováno | Obličej subsection fotka — moodboard nemá dedikovaný snímek |
| Parkováno | Review card — vizuální podoba, čeká na první recenze |
| Parkováno | Reservio wrapper chrome — nízká priorita |
| Parkováno | Mobilní breakpoint chování komponent do detailu — řeší se ve wireframe |

---

## 7. Motion reference

**Antara Spa Wellness** — inspirace pro scroll-triggered rozestup fotek do stran a sticky nav napravo. Adaptováno: výrazně **pomalejší a vzdušnější** timing než Antara (ta je rychlá/tvrdá) — "jako pomalé otevírání závěsu".

---

## 8. Nástroje

- **Affinity Designer** — kreslení ikon (canvas 200×200px, stroke 12px, pozor na pt/px rozdíl při DPI≠72).
- **Claude in Chrome MCP** — screenshoty konkurence.
- **Grilling skill** (vlastní, `/mnt/skills/user/grilling/`) — nelítostný interview pro scoping, použitý na celý design systém.
- **Reservio** — booking systém.

---

## 9. Kompetitivní reference (beze změny z dřívějška)
Angel Luxury (vizuální benchmark), Antara Spa Wellness (motion), TAWAN/Sansei/AURA/Vítězná/Garbo (ceníková struktura, typografický prostor).

---

## 10. Rozhodnutí ze session 19. 8. 2026 (wireframe grill + foto asset plán)

- **Nav:** sticky, průhledný přes Hero, při scrollu získá pozadí (ref. Venetian Nail Spa). CTA "Rezervovat" žije trvale v nav, Hero nemá vlastní CTA tlačítko.
- **Mapa (Kde mě najdeš):** ilustrativní grafika v paletě, ne embed Google Maps.
- **Patička:** minimální. Legal blok odděleně od "Kde mě najdeš":
  - Sídlo/provozovatel: Milada Vondrušová, IČO 69455058, U Hrušky 307/13a, Motol, 150 00 Praha 5
  - Provozovna (tlačítko → scroll na sekci): Karlovy Vary, Floating Phoenix
  - GDPR a obchodní podmínky — potřeba text, doporučeno ověřit s právníkem/GDPR poradcem
  - AI upravované/generované fotky — pravděpodobně vyžaduje disclosure (EU AI Act), přesné znění needěje ověřeno, needelat bez právní konzultace
  - Podpis: Milada nemá k dispozici, nepoužívat
- **Foto sada (F1, real assets místo placeholderů):**
  - Hero: atmosféra — len/textilie s protisvětlem, rozostřené lehátko v rohu (kontext bez popisnosti), bez textu v obrázku
  - O Miladě: reálný portrét (upravený, teplé světlo)
  - Služby/Tělo: detail rukou na zádech, s ručníkem
  - Služby/Obličej: detail rukou/prstů u hlavy a ucha
  - Služby/Access: detail jedné ruky, jen špičky prstů na spánku (ne propletené ruce — AI limitace)
  - Napříč sadou: konzistentní francouzská manikúra, teplý filmový grading (`#291B10`/`#D4821E`/`#FFC564`), žádné vyhlazené AI ruce/pleť
  - Fotky nahrává Tereza sama přímo do repozitáře.
- `wireframe.html` (needschválený pokus) smazán, nebyl uchováván jako referenční.

---

## 11. F1 stavba — `wireframe.html` na branch `claude/prvni-faze` (19.–20. 8. 2026)

Skeleton se skutečným obsahem (reálné fotky, texty, nav) — struktura hotová, čeká na F2 (tokeny/typografie z design systému).

**"AI-first" pravidlo — trvale platí napříč projektem:**
- Žádné dlouhé pomlčky (—) v copy. Nikdy.
- Žádné dekorativní šipky (→, ↓) — ani scroll cue, ani cross-link, ani na tlačítkách.
- Žádné číslované/kruhové bubliny pro kroky nebo číslované seznamy — obecně žádné "AI landing page" komponentové vzory (feature card grid, numbered steps in circles, seznam-řádek+tlačítko jako pricing table).
- Kroky "Příchod/Dotek/Proměna/Odchod" — bez čísel vůbec (ani jako tichá typografická číslice). Otevřeno, jak přesně vizuálně odlišit čtyři kroky bez číslování — řeší se ve F2.
- Parochí paralelismy v copy ("cítíte to, neřešíte to") jsou OK, pokud je píše Tereza/Milada — Claude podobný vzor sám negeneruje.
- Rozdíl "co to dělá" vs. "jak to vypadá": mechaniky (price-reveal na klik, sticky nav s fade při scrollu) zůstávají — byly grillované, obhájené. Řeší se jen vizuální balení, ne zahazovat mechaniku kvůli tomu, že vizuál byl generický.

**Rozhodnuto v rámci F1 gril kola (foto/UI úpravy):**
- Fotky ve Službách bez rámečku/border-radius — editorial, foto leží v ploše, ne v "kartě".
- Kontaktní ikony v Rezervaci zvětšené (34px) — vlastní kresba nese váhu, ne layout.
- Patička: jeden tichý sloupec, bez podtržených odkazů jako menu, legal obsah jako poznámka pod čarou.
- Nápad "ceník jako oboustranná karta" (foto vlevo, ceník vpravo, tištěný vzhled) zvážen a zamítnut — nekompatibilní s tím, že ceny jsou skryté za klikem (tištěný ceník ukazuje ceny rovnou). Zůstává současný stackovaný seznam, jen užší (max 640px), ať cena není daleko od názvu služby.

**Otevřené:** vizuální řešení "kroky bez čísel", přesný tvar sub-header karet a footeru ve F2.

---

## 12. Workflow pravidlo — struktura souborů a sdílené komponenty (20. 8. 2026)

**Kontext:** Tereza staví PULS v Angularu, kde komponentová knihovna přirozeně brzdí přílišnou AI kreativitu — nová komponenta se netvoří ad hoc, táhne se z knihovny. Tenhle projekt Angular nepotřebuje (jednostránkový web), ale stejná disciplína musí platit jinak.

**Oprava (20. 8. 2026):** fyzické rozdělení do `wireframe.html` + `styles.css` bylo špatný výklad tohohle pravidla — stránka se pak nedala jen tak otevřít a vidět fungovat, potřeba mít oba soubory pohromadě (stejný problém jako s fotkami, co se nezobrazovaly). Tereza to upřesnila: **stránka má být jeden kompletní dokument**, komponenty mají být oddělené jen **organizačně** — jasně pojmenované, přehledně komentované bloky CSS uvnitř jednoho `<style>` v `wireframe.html`, ne fyzicky rozdělené soubory. `styles.css` smazán, CSS zpátky v `wireframe.html`.

**Struktura zdroje pravdy:**
- `wireframe.html` — jeden kompletní dokument (struktura i vzhled), CSS uvnitř organizované po jasně pojmenovaných komponentách (nadpisy sekcí v komentářích)
- `design-system-2.html` — samostatný referenční dokument (jako Storybook) pro tokeny (barvy, spacing, radius, typografie) — zůstává oddělený záměrně, není to "stránka", je to knihovna, ze které se čte, ne mění

**Pravidlo pro budoucí změny komponent — platí natrvalo:**
Než se změní cokoliv sdíleného (třída v `styles.css`, token v design systému), **musí se nejdřív zeptat**, jestli je změna:
- **globální** — má platit pro komponentu všude, kde se používá → mění se sdílený soubor, nebo
- **lokální/jednorázová** — platí jen pro jednu konkrétní situaci → nesmí se sáhnout na sdílenou komponentu (to by to nechtěně změnilo všude jinde), řeší se lokálním override na místě.

Tohle se netýká jen CSS — platí obecně, kdykoli se upravuje cokoliv, co je použité na víc než jednom místě.

---

## 13. F2+F3 build — tokeny, komponenty, motion (20. 8. 2026)

Sloučeno do jednoho kroku (Tereza: fáze jsou u tohoto rozsahu zbytečně přísné, obojí bylo už kompletně specifikované). F4 (polish/QA) zůstává samostatný závěrečný průchod.

**"Kroky" zrušeny jako komponenta.** Tereza: "je to nepřirozené, ten příběh poneseme stránkou jinak." Čtyřfázový oblouk se nezobrazuje jako číslovaný seznam — nese ho copy a struktura stránky (sekce už mají fázové labely Příchod/Dotek/Proměna/Odchod). O Miladě sekce přejmenována na **"Něco málo o mně"**, text nahrazen finální Miladinou/Terezinou verzí (viz `wireframe.html`).

**Natažené komponenty z `design-system-2.html`** (čtení, zdroj se neměnil): CTA (`.cta-btn`/`.cta-wrap`/`.cta-halo`/`breathe` keyframe), price-reveal (`.price-row`/`.price-reveal`/`.pr-label`/`.pr-value` — nahradilo dřívější "cena ▸" tlačítko, jeden z identifikovaných AI-generic vzorů), hamburger (44×44px, radius 12px, `menu.svg` inline jako SVG kvůli `currentColor`), plná paleta/typografie/spacing/radius tokeny.

**Zdokumentovaná lokální výjimka:** foto ve Službách nemá radius/rámeček (design systém jinak definuje kartu s radius 18px přes `.subsection-demo`) — Miladin web se od něj v tomhle jednom bodě vědomě odchyluje, design-system-2.html zůstal beze změny.

**Ikony (Rezervace) přepsány z `<img src>` + `filter:invert(1)` na inline SVG** — `currentColor` funguje jen takhle, invert byl provizorní hack z F1.

**Motion — jen schválený bookend oblouk:** kinetická typografie na Hero H1 (per-word stagger, stejná logika jako motion demo), paralax vrstva O Miladě (Dotek, 0.25×) a Rezervace (Odchod, 0.85×), Hero beze motion (Příchod = nejtěžší/nejtišší fáze). `prefers-reduced-motion` respektováno.

**Mimo scope, zůstává otevřené:** paralax ve Službách (rozhodnuto už dřív že ne), třetí vrstva pro Proměnu, přesné tempo kinetického reveal per fáze, obousměrnost efektu, mobilní performance test. Ceny v `pr-value` jsou ilustrační placeholder, čekají na reálná čísla od Milady.

**Zbývá F4:** kontrast, focus stavy, touch targets ověřit v prohlížeči, reduced-motion test, responsivita 360/640/1024.
