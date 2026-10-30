# Obwalden: law history in git

The law of the canton of Obwalden (Kanton Obwalden, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-ow/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

155 acts with 398 versions so far: the cantonal constitution, the cantonal laws (Gesetze) in force and 81 Verordnungen and Reglemente in force, in the order of the systematic collection, added in parts. Other decrees and decisions, intercantonal agreements and repealed acts are not included yet.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `101-0-kantonsverfassung-kv/` | Verfassung des Kantons Obwalden (GDB 101.0) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2018 |
| `111-2-burgerrechtsgesetz-brg/` | Gesetz über den Erwerb und den Verlust des Kantons- und Gemeindebürgerrechts (GDB 111.2) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2023 |
| `122-1-abstimmungsgesetz-ag/` | Gesetz über die Ausübung der politischen Rechte (GDB 122.1) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2023 |
| `122-2-proporzgesetz-pg/` | Gesetz über die Wahl des Kantonsrates (GDB 122.2) | 2 | oldest version available, then each consolidated version: 1 May 2001 to 1 January 2018 |
| `122-3/` | Gesetz über die Einführung des Frauenstimm- und -wahlrechts (GDB 122.3) | 1 | as enacted, 24 September 1972 |
| `130-1-stvg/` | Staatsverwaltungsgesetz (GDB 130.1) | 7 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2027 |
| `130-3-hg/` | Haftungsgesetz (GDB 130.3) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2015 |
| `130-4-behordengesetz-behg/` | Gesetz über die Entlöhnung und Entschädigung von Behörden und Kommissionen (GDB 130.4) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2024 |
| `131-1-publikationsgesetz-kpublg/` | Gesetz über das Amtsblatt und die Gesetzessammlungen (GDB 131.1) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `131-3-offentlichkeitsgesetz-oeg/` | Gesetz über das Öffentlichkeitsprinzip (GDB 131.3) | 1 | as enacted, 1 March 2023 |
| `131-4-kantonales-registerharmonisierungsgesetz-krhg/` | Gesetz über die Harmonisierung der amtlichen Register (GDB 131.4) | 3 | as enacted, then each consolidated version: 15 January 2009 to 1 March 2026 |
| `131-5-kgeoig/` | Geoinformationsgesetz (GDB 131.5) | 1 | as enacted, 1 September 2011 |
| `132-1-kantonsratsgesetz-krg/` | Gesetz über den Kantonsrat (GDB 132.1) | 4 | oldest version available, then each consolidated version: 1 July 2012 to 1 March 2023 |
| `134-1-gog/` | Gesetz über die Gerichtsorganisation (GDB 134.1) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2022 |
| `134-4-anwg/` | Gesetz über die Ausübung des Anwaltsberufes (GDB 134.4) | 1 | one version (the oldest available), 1 January 2011 |
| `137-1-datenschutzgesetz-kdsg/` | Gesetz über den Datenschutz (GDB 137.1) | 2 | as enacted, then each consolidated version: 1 November 2008 to 1 September 2023 |
| `210-1-eg-zgb/` | Gesetz betreffend die Einführung des Schweizerischen Zivilgesetzbuches (GDB 210.1) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2026 |
| `210-2/` | Gesetz betreffend Ergänzung des Einführungsgesetzes zum Schweizerischen Zivilgesetzbuch (GDB 210.2) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 June 2017 |
| `210-3-beurkundungsgesetz-beurkg/` | Gesetz über die öffentliche Beurkundung (GDB 210.3) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2017 |
| `211-4-eg-partg/` | Einführungsgesetz zum Partnerschaftsgesetz (GDB 211.4) | 1 | one version (the oldest available), 1 January 2013 |
| `213-7-schatzungs-und-grundpfandgesetz/` | Gesetz über die amtliche Schätzung der Grundstücke und das Grundpfandrecht (GDB 213.7) | 5 | as enacted, then each consolidated version: 1 January 2007 to 1 January 2025 |
| `310-1-kstr/` | Gesetz über das kantonale Strafrecht (GDB 310.1) | 1 | one version (the oldest available), 1 January 2011 |
| `410-1-big/` | Bildungsgesetz (GDB 410.1) | 7 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `418-1/` | Sportförderungsgesetz (GDB 418.1) | 2 | as enacted, then each consolidated version: 1 August 2011 to 1 January 2021 |
| `451-1-kug/` | Kulturgesetz (GDB 451.1) | 2 | as enacted, then each consolidated version: 1 July 2016 to 1 August 2026 |
| `510-1-polg/` | Polizeigesetz (GDB 510.1) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `510-6/` | Gesetz über den Schutz bei häuslicher Gewalt (GDB 510.6) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2015 |
| `540-1-kbsg/` | Bevölkerungsschutzgesetz (GDB 540.1) | 1 | one version (the oldest available), 1 August 2007 |
| `543-1-zsg/` | Zivilschutzgesetz (GDB 543.1) | 1 | as enacted, 1 January 2005 |
| `546-1-feuerwehrgesetz-fewg/` | Gesetz über den vorbeugenden Brandschutz und die Feuerwehr (GDB 546.1) | 1 | as enacted, 1 January 2009 |
| `610-1-fhg/` | Finanzhaushaltsgesetz (GDB 610.1) | 5 | oldest version available, then each consolidated version: 1 March 2012 to 1 March 2023 |
| `630-1-fiag/` | Finanzausgleichsgesetz (GDB 630.1) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2025 |
| `641-4-stg/` | Steuergesetz (GDB 641.4) | 12 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `643-1-agg/` | Allgemeines Gebührengesetz (GDB 643.1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2017 |
| `651-1-jagdgesetz-jagdg/` | Gesetz über Jagd, Wild- und Vogelschutz (GDB 651.1) | 1 | one version (the oldest available), 1 January 2007 |
| `651-2-fig/` | Fischereigesetz (GDB 651.2) | 1 | one version (the oldest available), 1 January 2011 |
| `661-1-kantonalbankgesetz/` | Gesetz über die Obwaldner Kantonalbank (GDB 661.1) | 2 | as enacted, then each consolidated version: 1 July 2006 to 1 January 2026 |
| `661-2/` | Gesetz über den Bürgschaftsfonds Obwalden (GDB 661.2) | 1 | one version (the oldest available), 1 July 2006 |
| `663-1-ewog/` | Gesetz über das Elektrizitätswerk Obwalden und die Stromversorgung (GDB 663.1) | 3 | oldest version available, then each consolidated version: 1 September 2011 to 1 January 2020 |
| `710-1-pbg/` | Planungs- und Baugesetz (GDB 710.1) | 8 | oldest version available, then each consolidated version: 1 June 2011 to 1 March 2026 |
| `720-3-kantonsstrassengesetz-ksg/` | Gesetz über den Bau und Unterhalt der Kantonsstrassen (GDB 720.3) | 1 | one version (the oldest available), 1 January 2008 |
| `740-1-wasserbaugesetz-wbg/` | Gesetz über den Wasserbau und die Wassernutzung (GDB 740.1) | 5 | oldest version available, then each consolidated version: 1 January 2008 to 1 March 2026 |
| `740-2/` | Gesetz über die Planung, den Bau und die Finanzierung des Projekts Hochwassersicherheit Sarneraatal (GDB 740.2) | 3 | as enacted, then each consolidated version: 1 August 2007 to 1 January 2019 |
| `740-3/` | Gesetz über die Wasserbaumassnahmen an der Sarneraa Alpnach (GDB 740.3) | 3 | as enacted, then each consolidated version: 1 January 2016 to 1 January 2021 |
| `760-1-kentg/` | Gesetz über die Zwangsenteignung (GDB 760.1) | 1 | one version (the oldest available), 1 January 2011 |
| `771-1-kantonales-strassenverkehrsgesetz-eg-svg/` | Einführungsgesetz zum Bundesgesetz über den Strassenverkehr (GDB 771.1) | 1 | as enacted, 15 January 2009 |
| `771-2/` | Gesetz über die Strassenverkehrssteuern (GDB 771.2) | 3 | as enacted, then each consolidated version: 1 January 2009 to 1 January 2020 |
| `772-1-ovg/` | Gesetz über die Förderung des öffentlichen Verkehrs (GDB 772.1) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2015 |
| `772-2/` | Gesetz über den Neubau der Steilrampe der zb Zentralbahn AG (GDB 772.2) | 1 | one version (the oldest available), 1 August 2007 |
| `774-2/` | Gesetz über die Schiffssteuer (GDB 774.2) | 1 | one version (the oldest available), 1 August 2007 |
| `810-1-gesg/` | Gesundheitsgesetz (GDB 810.1) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `811-7-eg-ausbildungsforderung-pflege/` | Einführungsgesetz zum Bundesgesetz über die Förderung der Ausbildung im Bereich der Pflege (GDB 811.7) | 1 | as enacted, 1 July 2024 |
| `818-1-vetg/` | Veterinärgesetz (GDB 818.1) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 December 2024 |
| `818-3/` | Gesetz über das Halten von Hunden und die Hundesteuer (GDB 818.3) | 1 | one version (the oldest available), 1 August 2007 |
| `830-1-spitalg/` | Spitalgesetz (GDB 830.1) | 1 | as enacted, 1 January 2026 |
| `851-1-eg-kvg/` | Einführungsgesetz zum Krankenversicherungsgesetz (GDB 851.1) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 April 2026 |
| `853-1-eg-ahvg/` | Einführungsgesetz zum Bundesgesetz über die Alters- und Hinterlassenenversicherung (GDB 853.1) | 1 | one version (the oldest available), 1 January 2008 |
| `853-2-kelg/` | Gesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (GDB 853.2) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 September 2023 |
| `855-2/` | Gesetz über die steuerbegünstigten Arbeitsbeschaffungsreserven (GDB 855.2) | 1 | as enacted, 7 March 1993 |
| `857-1-kfamzg/` | Gesetz über die Familienzulagen (GDB 857.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2021 |
| `870-1-shg/` | Sozialhilfegesetz (GDB 870.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 8 April 2017 |
| `870-7/` | Gesetz über die familienergänzende Kinderbetreuung (GDB 870.7) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2017 |
| `874-1-kjfg/` | Kinder- und Jugendförderungsgesetz (GDB 874.1) | 1 | as enacted, 1 February 2013 |
| `880-1-kweg/` | Gesetz über die Wohnbau- und Eigentumsförderung (GDB 880.1) | 1 | one version (the oldest available), 1 January 2002 |
| `910-1/` | Gesetz über die regionale Wirtschaftspolitik (GDB 910.1) | 1 | one version (the oldest available), 1 January 2008 |
| `921-1-kantonales-landwirtschaftsgesetz-klwg/` | Einführungsgesetz zum Bundesgesetz über die Landwirtschaft sowie zum bäuerlichen Boden- und Pachtrecht (GDB 921.1) | 2 | as enacted, then each consolidated version: 1 March 2008 to 1 January 2017 |
| `930-1-kantonales-waldgesetz-kwag/` | Einführungsgesetz zum Bundesgesetz über den Wald (GDB 930.1) | 3 | as enacted, then each consolidated version: 1 June 2016 to 1 March 2026 |
| `971-1-ggg/` | Gastgewerbegesetz (GDB 971.1) | 2 | oldest version available, then each consolidated version: 1 January 2007 to 1 September 2018 |
| `971-3-tg/` | Tourismusgesetz (GDB 971.3) | 3 | as enacted, then each consolidated version: 1 July 2012 to 1 January 2027 |
| `971-4/` | Gesetz über das Campieren (GDB 971.4) | 1 | as enacted, 1 March 2015 |
| `975-1/` | Markt- und Reisendengewerbegesetz (GDB 975.1) | 2 | oldest version available, then each consolidated version: 1 August 2007 to 1 January 2021 |
| `975-2-ruhetagsgesetz/` | Gesetz über die öffentlichen Ruhetage (GDB 975.2) | 1 | one version (the oldest available), 1 August 2009 |
| `975-3-eg-bgs/` | Einführungsgesetz zum Geldspielgesetz (GDB 975.3) | 1 | as enacted, 1 January 2021 |
| `975-6-submissionsgesetz-submg/` | Gesetz über das öffentliche Beschaffungswesen (GDB 975.6) | 2 | as enacted, then each consolidated version: 1 February 2004 to 1 March 2023 |
| `111-21-burgerrechtsverordnung-brv/` | Verordnung zum Gesetz über den Erwerb und den Verlust des Kantons- und Gemeindebürgerrechts (GDB 111.21) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2018 |
| `113-11-einwohnerregisterverordnung-erv/` | Verordnung über das Einwohnerregister (GDB 113.11) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2023 |
| `113-21-verordnung-zum-auslanderrecht/` | Vollziehungsverordnung zum Bundesgesetz über die Ausländerinnen und Ausländer sowie zum Asylgesetz (GDB 113.21) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2023 |
| `122-11-abstimmungsverordnung-av/` | Vollziehungsverordnung zum Gesetz über die Ausübung der politischen Rechte (GDB 122.11) | 2 | oldest version available, then each consolidated version: 1 February 2010 to 1 January 2018 |
| `130-41/` | Verordnung über die Entschädigungen der nebenamtlichen Behörden und Beamten (GDB 130.41) | 1 | one version (the oldest available), 1 July 1999 |
| `131-21/` | Verordnung über das Staatsarchiv (GDB 131.21) | 3 | oldest version available, then each consolidated version: 1 July 2005 to 1 January 2026 |
| `133-11-organisationsverordnung-ov/` | Verordnung über die Organisation des Regierungsrates und der kantonalen Verwaltung (GDB 133.11) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `133-21-verwaltungsverfahrensverordnung-vwvv/` | Verordnung über das Verwaltungs- und Verwaltungsbeschwerdeverfahren (GDB 133.21) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `134-13-vwg/` | Verordnung über die Wählbarkeitsvoraussetzungen für Gerichtsbehörden und die Staatsanwaltschaft (GDB 134.13) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2015 |
| `134-14-vgv/` | Verordnung über das Verwaltungsgerichtsverfahren (GDB 134.14) | 1 | one version (the oldest available), 1 January 2011 |
| `134-112-grk/` | Geschäftsreglement für das Kantonsgericht (GDB 134.112) | 3 | as enacted, then each consolidated version: 1 January 2011 to 17 May 2018 |
| `134-113-rbo/` | Reglement über die Besetzung des Obergerichts (GDB 134.113) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 July 2016 |
| `134-114-gro/` | Geschäftsreglement für das Obergericht (GDB 134.114) | 5 | as enacted, then each consolidated version: 1 January 2011 to 1 September 2023 |
| `134-115-rer/` | Reglement über den elektronischen Rechtsverkehr (GDB 134.115) | 1 | as enacted, 1 January 2011 |
| `134-151-revv/` | Reglement über die Entschädigung für die unentgeltliche Verbeiständung und die amtliche Verteidigung (GDB 134.151) | 1 | as enacted, 1 January 2011 |
| `134-411/` | Reglement betreffend die Anwaltsprüfung und das Rechtspraktikum (GDB 134.411) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `141-11-pv/` | Personalverordnung (GDB 141.11) | 5 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `210-31-beurkundungsverordnung-beurkv/` | Verordnung über die öffentliche Beurkundung (GDB 210.31) | 1 | one version (the oldest available), 1 July 2002 |
| `210-351/` | Reglement über die Eignungsprüfung der Notarinnen und Notare (GDB 210.351) | 1 | as enacted, 11 August 2023 |
| `211-11-kzstv/` | Zivilstandsverordnung (GDB 211.11) | 2 | as enacted, then each consolidated version: 1 July 2004 to 1 March 2015 |
| `211-61-ev-kesr/` | Verordnung betreffend die Einführung des Kindes- und Erwachsenenschutzrechts (GDB 211.61) | 7 | as enacted, then each consolidated version: 1 January 2013 to 1 April 2022 |
| `213-11-vvav/` | Vollziehungsverordnung über die amtliche Vermessung (GDB 213.11) | 2 | oldest version available, then each consolidated version: 1 September 2011 to 1 June 2017 |
| `213-31/` | Verordnung betreffend die Viehverpfändung (GDB 213.31) | 1 | one version (the oldest available), 1 January 2011 |
| `213-51-bereinigungsverordnung/` | Verordnung über die Bereinigung der dinglichen Rechte und die Einführung des eidgenössischen Grundbuchs (GDB 213.51) | 2 | oldest version available, then each consolidated version: 1 September 2011 to 1 June 2017 |
| `213-61-grundbuchgebuhrentarif/` | Verordnung über die Grundbuchgebühren (GDB 213.61) | 1 | as enacted, 1 January 2022 |
| `213-71-schatzungs-und-grundpfandverordnung/` | Verordnung über die amtliche Schätzung der Grundstücke und das Grundpfandrecht (GDB 213.71) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2025 |
| `213-72/` | Verordnung über die Schätzungsgebühren (GDB 213.72) | 3 | as enacted, then each consolidated version: 1 April 2012 to 1 January 2024 |
| `213-81/` | Vollziehungsverordnung zum Bundesgesetz über den Erwerb von Grundstücken durch Personen im Ausland (GDB 213.81) | 1 | one version (the oldest available), 1 July 1998 |
| `220-11-ev-or/` | Verordnung über die Einführung des Bundesgesetzes über das Obligationenrecht (GDB 220.11) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2018 |
| `220-21/` | Versteigerungsverordnung (GDB 220.21) | 1 | one version (the oldest available), 1 August 2007 |
| `220-61/` | Vollzugsverordnung zum Bundesgesetz über die Anlagefonds (GDB 220.61) | 1 | one version (the oldest available), 1 January 2011 |
| `310-41-kantonale-ordnungsbussenverordnung-kobv/` | Verordnung über die direkte Bussenausfällung durch die Kantonspolizei und weitere Kontrollorgane (GDB 310.41) | 2 | as enacted, then each consolidated version: 15 December 2007 to 1 March 2015 |
| `330-11-strafvollzugsverordnung-stvo/` | Verordnung über den Straf- und Massnahmenvollzug sowie die Bewährungshilfe (GDB 330.11) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 February 2016 |
| `350-11-vv-ohg/` | Vollziehungsverordnung zum Opferhilfegesetz (GDB 350.11) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2015 |
| `410-11-biv/` | Bildungsverordnung (GDB 410.11) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2026 |
| `410-12-lehrpersonenverordnung-lpv/` | Verordnung über das Anstellungsverhältnis der Lehrpersonen (GDB 410.12) | 10 | as enacted, then each consolidated version: 1 January 2013 to 1 August 2026 |
| `410-13/` | Verordnung über Leistungsangebote in den Bereichen Sozialpädagogik, Sonderschulung und Förderung von Menschen mit einer Behinderung (GDB 410.13) | 1 | one version (the oldest available), 1 February 2013 |
| `410-411/` | Reglement über die Anerkennung von Ausbildungsabschlüssen (GDB 410.411) | 8 | oldest version available, then each consolidated version: 5 December 2012 to 1 February 2023 |
| `412-11-vschv/` | Volksschulverordnung (GDB 412.11) | 5 | oldest version available, then each consolidated version: 1 January 2012 to 1 August 2026 |
| `415-422/` | Personalverordnung der Hochschule Luzern, FH Zentralschweiz (GDB 415.422) | 6 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `415-423-gebuhrenverordnung-hslu/` | Verordnung über die Gebühren an der Hochschule Luzern, FH Zentralschweiz (GDB 415.423) | 4 | as enacted, then each consolidated version: 1 March 2013 to 1 September 2025 |
| `419-11-stipendienverordnung/` | Verordnung über die Ausrichtung von Ausbildungsbeiträgen (GDB 419.11) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2026 |
| `419-311/` | Reglement über den Kathriner-Egger-Fonds (GDB 419.311) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 July 2022 |
| `451-21/` | Verordnung über den Schutz von Bau- und Kulturdenkmälern (Denkmalschutzverordnung, DSV) (GDB 451.21) | 4 | oldest version available, then each consolidated version: 1 July 2008 to 1 November 2026 |
| `530-41/` | Vollziehungsverordnung zum Bundesgesetz über die Wehrpflichtersatzabgabe (GDB 530.41) | 2 | oldest version available, then each consolidated version: 1 January 2005 to 1 March 2015 |
| `540-21-vksd/` | Verordnung über den Koordinierten Sanitätsdienst (GDB 540.21) | 2 | as enacted, then each consolidated version: 1 January 2006 to 1 February 2016 |
| `542-11/` | Verordnung über die wirtschaftliche Landesversorgung (GDB 542.11) | 1 | as enacted, 1 January 2005 |
| `630-51/` | Verordnung über die Beteiligung der Einwohnergemeinden am interkantonalen Finanzausgleich (GDB 630.51) | 1 | as enacted, 1 January 2020 |
| `641-41-stv/` | Vollziehungsverordnung zum Steuergesetz (GDB 641.41) | 8 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `643-11-vagg/` | Verordnung zum Allgemeinen Gebührengesetz (GDB 643.11) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2018 |
| `651-11-jagdv/` | Jagdverordnung (GDB 651.11) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2027 |
| `651-21-fiv/` | Fischereiverordnung (GDB 651.21) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2019 |
| `720-11/` | Strassenverordnung (GDB 720.11) | 2 | oldest version available, then each consolidated version: 1 August 2007 to 1 March 2026 |
| `720-31-strassenbeitragsverordnung/` | Verordnung über die Strassenbeiträge (GDB 720.31) | 3 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2016 |
| `720-51/` | Vollziehungsverordnung zum Bundesgesetz über die Nationalstrassen (GDB 720.51) | 1 | one version (the oldest available), 1 September 2011 |
| `720-71-vv-fwg/` | Vollziehungsverordnung zum Bundesgesetz über Fuss- und Wanderwege (GDB 720.71) | 3 | oldest version available, then each consolidated version: 1 August 2007 to 1 March 2026 |
| `740-11-wbv/` | Wasserbauverordnung (GDB 740.11) | 3 | oldest version available, then each consolidated version: 15 January 2009 to 1 March 2026 |
| `774-11-vsf/` | Verordnung über die Schifffahrt (GDB 774.11) | 2 | as enacted, then each consolidated version: 15 January 2009 to 1 March 2026 |
| `780-11-kantonale-umweltschutzverordnung-vv-usg/` | Vollziehungsverordnung zum Bundesgesetz über den Umweltschutz (GDB 780.11) | 1 | one version (the oldest available), 1 August 2007 |
| `783-11-kantonale-gewasserschutzverordnung-vv-gschg/` | Vollziehungsverordnung zum Bundesgesetz über den Schutz der Gewässer (GDB 783.11) | 1 | one version (the oldest available), 1 January 2008 |
| `783-21/` | Ölwehrverordnung (GDB 783.21) | 1 | one version (the oldest available), 1 January 2009 |
| `786-11-naturschutzverordnung-nsv/` | Verordnung über den Natur- und Landschaftsschutz (GDB 786.11) | 4 | oldest version available, then each consolidated version: 1 January 2008 to 1 March 2026 |
| `786-21/` | Pilzschutzverordnung (GDB 786.21) | 1 | as enacted, 1 July 1997 |
| `810-12/` | Verordnung über eine Fachstelle für Gesellschaftsfragen (GDB 810.12) | 4 | oldest version available, then each consolidated version: 1 February 2013 to 1 January 2019 |
| `816-11/` | Vollziehungsverordnung zum Lebensmittelgesetz (GDB 816.11) | 1 | as enacted, 1 January 2011 |
| `817-11/` | Verordnung über Friedhöfe und Bestattungen (GDB 817.11) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2022 |
| `830-112-taxordnung-kantonsspital/` | Reglement über die Taxen des Kantonsspitals für die stationäre und ambulante Behandlung von Patientinnen und Patienten sowie den Rettungsdienst (GDB 830.112) | 2 | as enacted, then each consolidated version: 1 July 2020 to 1 June 2023 |
| `830-115/` | Reglement über den Fonds für Personen in wirtschaftlicher Notlage (GDB 830.115) | 1 | as enacted, 1 June 2007 |
| `841-11-verordnung-zum-arbeitsgesetz/` | Verordnung zum Bundesgesetz über die Arbeit in Industrie, Gewerbe und Handel (GDB 841.11) | 1 | one version (the oldest available), 1 January 2011 |
| `843-11-vv-avg/` | Vollziehungsverordnung zum Arbeitsvermittlungsgesetz (GDB 843.11) | 1 | one version (the oldest available), 1 January 2011 |
| `851-11-ev-kvg/` | Verordnung zum Einführungsgesetz zum Krankenversicherungsgesetz (GDB 851.11) | 8 | oldest version available, then each consolidated version: 1 January 2012 to 1 June 2026 |
| `853-31/` | Verordnung zum Bundesgesetz über die Invalidenversicherung (GDB 853.31) | 1 | as enacted, 1 January 2012 |
| `855-11-vv-avig/` | Vollziehungsverordnung zum Arbeitslosenversicherungsgesetz (GDB 855.11) | 1 | one version (the oldest available), 1 January 2000 |
| `856-11/` | Verordnung über die berufliche Vorsorge (GDB 856.11) | 2 | oldest version available, then each consolidated version: 1 January 2006 to 1 June 2016 |
| `870-11-shv/` | Sozialhilfeverordnung (GDB 870.11) | 1 | one version (the oldest available), 1 January 2013 |
| `870-12/` | Verordnung über das Inkasso und die Bevorschussung von Unterhaltsbeiträgen (GDB 870.12) | 1 | one version (the oldest available), 1 January 2013 |
| `880-11/` | Verordnung über die Wohnbau- und Eigentumsförderung (GDB 880.11) | 1 | one version (the oldest available), 1 August 2007 |
| `910-11/` | Verordnung über die regionale Wirtschaftspolitik (GDB 910.11) | 1 | as enacted, 1 January 2008 |
| `921-41/` | Vollziehungsverordnung zum Bundesgesetz über die Familienzulagen für landwirtschaftliche Arbeitnehmer und Bergbauern (GDB 921.41) | 1 | one version (the oldest available), 1 August 2007 |
| `971-11-ggv/` | Gastgewerbeverordnung (GDB 971.11) | 2 | oldest version available, then each consolidated version: 1 August 2007 to 1 September 2018 |
| `971-31-tv/` | Tourismusverordnung (GDB 971.31) | 2 | as enacted, then each consolidated version: 1 July 2012 to 1 January 2017 |

## Source

The GDB (systematic collection) of the canton, published by the canton at <https://gdb.ow.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (OGS). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (OGS), with an e-mail address that cannot exist (`<act key>@gdb.ow.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
