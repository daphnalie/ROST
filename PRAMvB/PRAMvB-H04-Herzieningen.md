# Herzieningen

**In dit hoofdstuk wordt ingegaan op de wijze waarop gedeeltelijke herzieningen
gecodeerd moeten worden en hoe beschikt kan worden over een versie
"geconsolideerd".**

## Gedeeltelijke herziening

Bij een algemene maatregel van bestuur (amvb) of ministeriële regeling (mr) kan
onderscheid worden gemaakt in een besluit dat eenmalig is genomen c.q. wordt
herzien waarbij zij integraal in de plaats komen van een voorgaand besluit en in
een reeds vastgesteld besluit waarvan een gedeelte wordt herzien.

Hetgeen in [Hoofdstuk 4](#H04) van deze praktijkrichtlijn is vermeld, is zowel in het
eenmalige geval als in geval van een integraal herzien besluit volledig van
toepassing.

Op deze wijze wordt al hetgeen een nieuwe amvb besluit betreft gecodeerd en
wordt voldaan aan de wettelijke plicht te beschikken over een objectgericht
besluit.

In het andere geval wordt een gedeelte van de geldende amvb of mr herzien,
waarna de geldende amvb of mr, inclusief hetgeen daarvan herzien is, de nieuwe
geldende amvb of mr wordt. In dit geval worden alleen die aspecten die de
aanpassing betreffen gecodeerd. Onderstaand wordt aangegeven op welke wijze de
objecten en attributen uit [Hoofdstuk 3](#H03) voor een gedeeltelijke herziening dienen
te worden gebruikt. Het resultaat is een aparte dataset die behoort bij de
gedeeltelijke herziening. De dataset wordt vindbaar en toegankelijk gemaakt door
het betreffende departement van het rijk. Het is aan dat departement of de
herziening is hetzelfde dossier of in een los dossier in het manifest wordt
geplaatste.

Als verplicht onderdeel moet het object *Besluitgebied_A* worden gebruikt. De
begrenzing van het plangebied heeft betrekking op de te herziene locatie. Dit
kan afwijken van de begrenzing van het oorspronkelijk plangebied waarop de
herziening betrekking heeft. Verder wordt dezelfde multipliciteit van de
attributen in acht genomen, met dat verschil dat het attribuut
*verwijzingNaarExternPlanInfo* verplicht moet worden ingevuld.

Daartoe worden bij het object *Besluitgebied_A* bij het attribuut
*verwijzingNaarExternPlanInfo* bij de samenstellende attributen respectievelijk
de naam (type) van het plan dat wordt herzien, het idn van het plan dat wordt
herzien en de waarde "ter vervanging van extern plan" ingevuld. Daarmee wordt de
relatie met het plan dat gedeeltelijk wordt herzien vastgelegd.

**Tabel 5 Relatie naar extern plan**

![](media/90aaf91bc643371054a910a887b4198e.png)


Bij het attribuut *verwijzingNaarTekstInfo* worden alle relevante teksten
gevoegd. Daartoe wordt gebruik gemaakt van de domeinwaarden van het domein
*TeksttypeBG_AMB*. De overige attributen spreken voor zich.

Daarnaast kunnen vervolgens alle herziene objecten van de klasse *Besluitvlak_A*
en/of *Besluitsubvlak_A*, met alle (nieuwe of aanpassingen van de) regels, voor
zover dit de herziening betreft, worden gecodeerd. De codering, zoals hier
bedoeld, dient afhankelijk van de concrete situatie te worden aangebracht.
Nadere regels zijn moeilijk te geven gezien de vele mogelijkheden die aard,
omvang en onderlinge samenhang van de te herziene gedeelten van een amvb of mr
met zich meebrengen. Dit betreft uiteraard geen ideale situatie. Zo daar
behoefte aan is kan getracht worden hierover afspraken te maken en een aparte
richtlijn te schrijven.

Het kan praktisch zijn om de objecten die behoren bij de herziening zodanig te
kiezen en te coderen dat er een voordeel ontstaat bij het opstellen van de
versie "geconsolideerd" die verderop aan de orde komt. Uiteraard is het
juridische doel van de herziening maatgevend, maar kan van de ruimte binnen dat
doel gebruik worden gemaakt om te komen tot een ook voor de codering en de
verwerking daarvan in een geconsolideerd besluit praktische oplossing.

Op deze wijze wordt al hetgeen een herziening van een amvb of mr betreft
gecodeerd en wordt voldaan aan de wettelijke plicht te beschikken over een
objectgericht plan, maar ontstaat *geen* compleet overzicht van de nieuwe
geldende situatie. Een oplossing daarvoor is om gebruik te maken van een versie
"geconsolideerd" waarin de gevolgen van de herziening zijn verwerkt. Daarop
wordt hierna onder [4.2](#geldende-situatie-de-versie-geconsolideerd) nader ingegaan.

## Geldende situatie: de versie “geconsolideerd”

De versie “geconsolideerd” van een amvb kent geen wettelijke, dus geen
juridische status. Het gebruik van een geconsolideerd besluit is een keuze van
de bronhouder. Er kan echter behoefte zijn in goed inzicht in gedeeltelijke
herzieningen en de samenhang met de amvb of mr waarvan zij deel uitmaken. Dit
ontstaat slechts wanneer gebruik wordt gemaakt van een aparte geïntegreerde
vorm" van de geldende situatie. Ook kan het voorkomen dat via een apart
inwerkingstredingbesluit delen van de AMvB wel en niet in werking treden.
Hiervoor kan ook een geconsolideerd besluit gemaakt worden. Het is aan de
bronhouder te bepalen welke ruimtelijke plannen in de versie “geconsolideerde”
worden geïntegreerd.

Om de raadpleger van [Ruimtelijkeplannen.nl](#www.ruimtelijkeplannen.nl) meer duidelijkheid te kunnen bieden
over de exacte status en werkingssfeer van de besluiten en het actuele
planologische regime ter plaatse kan het gebruik van een versie “geconsolideerd”
de oplossing zijn. Op die manier is in één oogopslag duidelijk wat de juridische
status van de desbetreffende besluiten is en wat de overige gevolgen ervan zijn,
zoals het vigerende planologische regime ter plaatse. Hierdoor is het niet
(meer) nodig via andere, vaak omslachtige, wegen te zoeken naar die informatie.
Dat geeft duidelijkheid, kost minder tijd en is dus klantvriendelijk naar de
raadpleger.

<u>Let op</u>: het gaat dus niet om een nieuw ruimtelijk plan maar om het samenvoegen
van meerder ruimtelijke plannen om zo een integrale versie, en daardoor een
beter leesbare versie, te tonen. Er vinden dus geen nieuwe ontwikkelingen
plaats. De reden om toch een versie “geconsolideerd” op te stellen is dat de
leesbaarheid van de geldende regelingen door deze versie sterk wordt verbeterd
waardoor ook de interpretatie van deze geldende regelingen een stuk eenvoudiger
zou moeten zijn.

Om de versie “geconsolideerd” te laten onderscheiden van de andere ruimtelijke
plannen wordt het attribuut planstatus bij het object Besluitgebied_A voorzien
van de waarde "geconsolideerd" en als waarde voor het attribuut datum de
inwerkingtredingdatum van de laatste opgenomen gedeeltelijke herziening of
inwerkingtredingsbesluit. Voor een goed begrip zullen naast de bijbehorende
geldende regels ook alle oorspronkelijke toelichtingen moeten worden toegevoegd
bij het attribuut *verwijzingNaarTekstInfo* van het object Besluitgebied_A. Bij
de waarde van het attribuut *verwijzingNaarExternPlanInfo* worden alle besluiten
opgenomen die in deze geconsolideerde versie zijn verwerkt. De waarde bij het
attribuut *rolExternPlan* is in dit geval: ´als mutatie opgenomen´. Het
ruimtelijke plan met de plan status ‘geconsolideerd’ wordt in het manifest met
behulp van de dossierstatus ‘geconsolideerd’ geplaatst.