# Features - Den Perfekta Mackan

> Track features and user stories for världens viktigaste mjukvaruprojekt.

---

## 🚧 In Progress

### Brödval-algoritmen
**Description:** Implementera ett beslutsstödsystem för att välja rätt brödsortstyp baserat på pålägg, humör och veckodag. Systemet väger in kontextuella faktorer som mötesintensitet, väderläge och om det är en måndag — parametrar som visat sig ha signifikant påverkan på brödvalet i interna tester. Rågsurdeg representerar det seriösa, ambitiösa valet och reserveras för tillfällen när man vill signalera att man har ordning på livet. Vitt formbröd är däremot det mjuka, förlåtande alternativet för fredagar och dagar när existensen känns lite tung. Knäckebröd ingår som ett robust fallback-alternativ när brödlådan sviker — det är inte idealiskt, men det är stabilt och dömer inte. Glutenfritt bröd är explicit uteslutet ur scope; projektet måste sätta gränser någonstans för att undvika feature creep.

**Priority:** Kritisk
**Owner:** Magen
**Effort:** 2/5
**Created:** 2026-01-01
**Updated:** 2026-03-02
**Dependencies:** Ingen (bröd är fundamentalt)

**Details:**
- Rågsurdeg för tisdagar och allvarliga möten
- Vitt formbröd för fredagar och existentiell trötthet
- Knäckebröd som fallback när man glömde handla
- Inget glutenfritt (projektet sätter gränser)
- Brödrostning är en separat MVP (fas 2)

**Acceptance Criteria:**
- [ ] Brödet är inte mögligt
- [ ] Rätt antal skivor väljs (2, alltid 2)
- [ ] Algoritmen tar hänsyn till om brödet är slut och föreslår knäckebröd utan att döma

**Notes:** Tekniska skulden är hög efter ett olyckligt incident med hårt bröd och ett ömtåligt tandstift i Q4 2025.

---

## 📋 Planned

### Påläggsdistributions-optimering
**Description:** Säkerställ att pålägg täcker hela brödytan med jämn fördelning, inklusive de fyra hörnen som historiskt sett ignorerats med en likgiltighet som gränsar till förakt. Ojämn smörfördelning är den vanligaste källan till mackmissnöje och utgör projektets mest kritiska UX-skuld. Tomater ska skivas i konsekvent tjocklek; en tomat kastad hel på brödet klassas som ett undantag och triggar en explicit varning i loggarna. Kaviar ur tub behandlas som en premium feature och undantas från de ordinarie täckningskraven — det är ett konstverk och ska hanteras därefter. Smörpålägg över 4 mm tjocklek ska flaggas med en mjuk kardiovaskulär varning, inte ett blockerande fel, för att respektera användarens autonomi. Algoritmen ska kunna hantera kombinerade pålägg, t.ex. smör + ost + tomat, utan att prioriteringskonflikter uppstår.

**Priority:** Hög
**Owner:** Kniven
**Effort:** 1/5
**Created:** 2026-02-01
**Dependencies:** Brödval-algoritmen

**Details:**
- Kant-till-kant-täckning är ett hård krav
- Tomater ska skivas, inte slängas hela
- Kaviar ur tub räknas som en feature, inte en bug
- Implementera varning vid för tjockt smörpålägg (kardiovaskulär teknisk skuld)

**Acceptance Criteria:**
- [ ] Inga nakna brödkanter
- [ ] Smöret är inte fruset
- [ ] Osten hänger inte ut på ena sidan som ett misslyckande

---

### Strukturell integritetstestning
**Description:** Verifiera att mackan håller ihop under transport från tallrik till mun utan katastrofalt sammanbrottscenario, vilket definieras som mer än 15% av påläggsmassa utanför brödytan. Testsviten inkluderar ett standardtransporttest (rak horisontell förflyttning), ett stresstest med vridrörelse över 45 grader, och ett simulerat hungertillstånd med förhöjt greppstryck mot kanterna. Tomaten-glid-koefficienten är den mest volatila parametern och måste understiga 0.4 för att systemet ska anses stabilt — tidigare versioner har haft katastrofala värden uppemot 1.1. Falltest från bordshöjd är ett edge case som tekniskt sett är out of scope, men som ändå dokumenteras eftersom det sker med oroväckande regelbundenhet i produktion. Resultaten ska loggas och mackor med tre på varandra följande strukturella misslyckanden bör flaggas för påläggsrekonfiguration. Inget pålägg på skjortan är ett hårt krav och blockerar release.

**Priority:** Hög
**Owner:** Handen
**Effort:** 1/5
**Created:** 2026-02-10
**Dependencies:** Påläggsdistributions-optimering

**Details:**
- Stresstest: snabb vridrörelse > 45 grader
- Kanttryck-analys (hårt grepp vid hunger)
- Tomaten-glid-koefficient måste understiga 0.4
- Falltest från bords höjd (edge case: man tappar mackan)

**Acceptance Criteria:**
- [ ] Mackan överlever förflyttning till soffan utan dekonstruktion
- [ ] Inget pålägg landar på skjortan
- [ ] Tomaten sitter kvar (stretch goal)

---

### Post-konsumtions-viloprotokollet
**Description:** Dokumentera det vetenskapligt optimala viloförloppet efter mackkonsumtion, baserat på aggregerad fältdata och en djup respekt för matsmältningens egna tidslinjer. Forskning inom projektet pekar på ett intervall på 12–17 minuter horisontellt läge som den optimala digestionsperioden, med signifikant ökad risk för ånger och uppblåsthet utanför detta fönster. Direktkontakt med e-post eller Slack under de första tio minuterna är kontraindikerat och har i interna tester visat sig öka stressnivåerna med upp till 40% utan motsvarande produktivitetsvinst. En kalenderintegration med Outlook ska automatiskt blockera 12:00–12:30 för att skydda perioden från mötesintrång av opportunistiska kollegor. Ljudmiljön under vilan specifieras till tyst eller lättpodcast — inga nyheter, inget som kräver aktiv tankeverksamhet. Den viktigaste funktionen i hela protokollet är att nästa macka ska börja planeras mentalt redan under vilan, vilket skapar en självförstärkande flywheel-effekt i mackekosystemet.

**Priority:** Låg
**Owner:** Soffan
**Effort:** 5/5
**Created:** 2026-02-15
**Dependencies:** Alla ovanstående features

**Details:**
- 12–17 minuters horisontellt läge rekommenderas
- Undvik direkt e-postkontroll under digestionsperioden
- Integrera med Outlook-kalender för att blockera möten 12:00–12:30
- Ljud: tyst, eller podcast om händelsen är vardaglig

**Acceptance Criteria:**
- [ ] Ingen ångrar mackan
- [ ] Nästa macka planeras redan under vilan (flywheel-effekt)

---

## ✅ Done

### Bröd inhandlat
**Description:** Genomförde en lyckad expedition till ICA och anskaffade bröd av godkänd kvalitet efter ett noggrant beslutsprocess vid brödavdelningen. Initialt föredrogs vitt formbröd på grund av ett pågående kampanjpris, men rågsurdeg valdes ändå — ett beslut som retrospektivt klassas som korrekt och som ingen ångrar. Brödets mjukhet verifierades manuellt i butik via lätt kläming, utan att förorsaka öppet åtagande gentemot omgivande kunder. Utgångsdatum granskades och godkändes med marginal; projektet har strikta policys mot teknisk skuld i form av halvmöglat bröd. Expeditionen avslutades inom 23 minuter, vilket understiger projektets SLA på 30 minuter för enklare upphandlingsärenden. Brödet förvaras nu korrekt i brödlåda och är redo för konsumtion vid nästa triggad macksekvens.

**Completed:** 2026-03-01
**Owner:** Benen
**Effort:** 1/5

**Notes:** Tog rågsurdeg trots att vitt formbröd hade kampanjpris. Ingen ångrar det.

---

## ❌ Cancelled/Rejected

### Mackan som en tjänst (MaaS)
**Description:** Prenumerationsmodell där mackor levereras via ett REST API med konfigurerbart pålägg som query-parametrar och brödval som request body. Konceptet bedömdes initialt som lovande och attraherade intern entusiasm under ett tidigt planning-möte som saknade agenda. Djupare analys avslöjade att logistiklagret saknas fullständigt — det finns inget leveranslager, ingen förpackningsmodul, och mackan försämras märkbart under REST-callens latens. Integrationstestning mot ICA:s sortiment visade att deras API inte stödjer halvkilos rågsurdeg som JSON-payload, vilket är ett fundamentalt blockerande beroende. Projektet pausades formellt i januari 2026 och arkiverades med kommentaren "återkommer i fas 3", vilket är projektets konvention för idéer man tycker om men inte tänker genomföra. Kundunderlaget (1 person) ansåg beslutet vara rimligt.

**Cancelled:** 2026-01-20
**Reason:** Verkligheten stödjer inte detta use case ännu. Återkommer i fas 3.

---

<!-- Effort legend: 1/5 = minuter, 2/5 = 1 timme, 3/5 = hela eftermiddagen, 4/5 = dagen, 5/5 = odefinierat men troligen resten av dagen -->
