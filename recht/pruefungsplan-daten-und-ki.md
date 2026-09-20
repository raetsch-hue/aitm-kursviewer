---
artefakt: Prüfungsplan — rechtliche Anforderungen an Daten- und KI-Integration
datum: 2026-09-20
status: **zweite Fassung.** 39 Prüfpunkte in sieben Rechtsgebieten, fünf Lücken offen benannt
zweck: die rechtlichen Anforderungen in prüfbare Punkte zerlegen — je Punkt Rechtsgrundlage, Auslöser, Nachweis
geltung: **firmenunabhängig.** Kein Fallwert, kein Mandantenbezug
herkunft: **überwiegend [Sekundär].** Fundstellen über öffentliche Aufbereitungen belegt, Abrufdatum 2026-09-20. **Ausnahme:** § 15 AGG und § 61b ArbGG sind am amtlichen Volltext gelesen. **Kein Unionsrechtsakt im Volltext am Amtsblatt geprüft.** Keine Quelle stammt aus dem Kursmaterial
vorbehalt: Keine Rechtsberatung. Ordnet, entscheidet nicht
---

# Prüfungsplan · Rechtliche Anforderungen an Daten- und KI-Integration

> **Belegstatus vorweg.** Jeder Prüfpunkt nennt **Rechtsakt und Fundstelle**. Die Datumsangaben und
> Verordnungsnummern sind am **20.09.2026** über öffentliche Aufbereitungen belegt und **nicht am
> Amtsblatt im Volltext verifiziert** — wer daraus eine Entscheidung ableitet, prüft die Fundstelle
> nach. **Zwei Ausnahmen:** § 15 AGG und § 61b ArbGG (Prüfpunkt 1.6) sind am amtlichen Volltext
> gelesen und als **[Primär]** gekennzeichnet. **Keine Quelle stammt aus dem Kursmaterial:** Ein Kurs referiert Recht, er setzt es nicht,
> und `coursebook/woche-5/5.0` führt selbst drei Korrekturen an seinem eigenen Material.

## Wie dieser Plan benutzt wird

**Nicht von vorn nach hinten.** Die Prüfung beginnt mit Teil 0 — vier Fragen, die entscheiden,
welche Abschnitte überhaupt einschlägig sind. Wer sie überspringt, prüft Anforderungen, die ihn
nicht treffen, und übersieht die, die ihn treffen.

Je Prüfpunkt: **was zu prüfen ist · woraus es folgt · woran man erkennt, dass es erfüllt ist.**
Ein Punkt gilt erst als erfüllt, wenn der Nachweis **existiert**, nicht wenn er möglich wäre.

---

## Teil 0 · Die vier Vorfragen

| | Frage | Wenn ja, dann einschlägig |
|---:|---|---|
| **V1** | Werden **personenbezogene Daten** verarbeitet? | Abschnitt 1 vollständig |
| **V2** | Wird ein **KI-System** eingesetzt oder entwickelt? | Abschnitt 2 · dazu V3 |
| **V3** | Wirkt das System auf **Beschäftigung, Bildung, Kreditwürdigkeit, Strafverfolgung, Migration, Justiz, kritische Infrastruktur oder Biometrie**? | Abschnitt 2 als **Hochrisiko**; Anhang III |
| **V4** | Wird ein **Produkt mit digitalen Elementen** in Verkehr gebracht oder ein **vernetztes Produkt** betrieben? | Abschnitt 3 und 4 |

> **Die häufigste Fehleinschätzung sitzt bei V3.** Die acht Hochrisikobereiche werden in
> Anbietermaterial regelmäßig auf zwei verkürzt (Medizintechnik, kritische Infrastruktur). Wer sich
> darauf verlässt, rechnet sich heraus. Gegenprobe:
> [`bibliothek/eu-ai-act.md`](../bibliothek/eu-ai-act.md) § 3 führt alle acht.

---

## 1 · Datenschutz

**Rechtsgrundlage:** Verordnung (EU) 2016/679 (DSGVO), unmittelbar geltend seit 25.05.2018 ·
ergänzend BDSG · für Endgeräte­zugriffe TDDDG.

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **1.1** | **Rechtsgrundlage je Verarbeitung** benannt und dokumentiert | Art. 6 DSGVO | Verarbeitungsverzeichnis mit Zuordnung je Zweck |
| **1.2** | **Auftragsverarbeitungsvertrag** mit jedem Dienstleister, der Daten verarbeitet | Art. 28 DSGVO | Unterzeichneter AVV **vor** der ersten Verarbeitung |
| **1.3** | **Datenschutz-Folgenabschätzung**, wenn die Verarbeitung voraussichtlich hohes Risiko birgt | Art. 35 DSGVO | DSFA-Dokument, vor Inbetriebnahme |
| **1.4** | **Meldung von Verletzungen** binnen 72 Stunden an die Aufsicht, ggf. an Betroffene | Art. 33, 34 DSGVO | Meldeprozess mit benannter Rolle und Erreichbarkeit |
| **1.5** | **Betroffenenrechte** technisch erfüllbar: Auskunft, Berichtigung, Löschung, Widerspruch | Art. 15–21 DSGVO | Nachweisbare Löschung, nicht nur Löschkonzept |
| **1.6** | **Aufbewahrungsmatrix liegt vor, bevor gelöscht wird** — je Datenart: Zweck, Frist, Rechtsgrund, und was nach Fristende geschieht | Art. 17 Abs. 3 lit. b und lit. e DSGVO · § 15 Abs. 4 AGG · § 61b Abs. 1 ArbGG | **Eine Matrix, kein Satz.** Je Datenart eine Zeile; Löschen **oder** Sperren ist je Zeile entschieden, nicht pauschal |
| **1.7** | **Besondere Kategorien** nur auf tragfähiger Grundlage | Art. 9 DSGVO | Gesonderte Prüfung, dokumentiert |
| **1.8** | **Automatisierte Einzelentscheidung** mit rechtlicher Wirkung nur unter engen Bedingungen | Art. 22 DSGVO | Nachweis menschlicher Beteiligung, die die Entscheidung **ändern kann** |
| **1.9** | **Zugriff auf Endgeräte** (Cookies, Tracking) nur mit Einwilligung | § 25 TDDDG | Einwilligungsnachweis |

> **Der Punkt, an dem KI-Projekte am häufigsten scheitern, ist 1.8 — nicht 1.3.** Art. 22 verlangt
> keine Beteiligung, sondern eine **wirksame**. Ein Mensch, der bestätigt, ist keine Beteiligung;
> ein Mensch, der die Reihenfolge ändern kann, ist eine.

> **1.5 und 1.6 gehören zusammen, und 1.6 kommt zuerst.** 1.5 verlangt, dass gelöscht werden
> *kann*. 1.6 verlangt zu wissen, **was nicht gelöscht werden darf** — und das ist der Punkt, an dem
> ein sauber abgearbeiteter Plan Schaden anrichtet: Wer die Betroffenenrechte technisch scharf
> stellt, ohne die Aufbewahrungsfristen daneben zu legen, löscht rechtmäßig genau die Unterlagen weg,
> mit denen er sich später verteidigen müsste. **Art. 17 Abs. 3 lit. e** nimmt die Geltendmachung und
> Verteidigung von Rechtsansprüchen vom Löschanspruch aus; **lit. b** tut dasselbe für gesetzliche
> Aufbewahrungspflichten — dort ist die Folge **Sperren statt Löschen**, nicht Löschen.
>
> Die Fristen dafür stehen nicht in der DSGVO, sondern im Fachrecht. Beispiel Bewerbungsunterlagen:
> **§ 15 Abs. 4 AGG** gibt zwei Monate für die schriftliche Geltendmachung eines
> Entschädigungsanspruchs, **§ 61b Abs. 1 ArbGG** danach drei Monate für die Klage — daraus folgt die
> in der Praxis übliche Aufbewahrung von **rund sechs Monaten** (zwei plus drei plus Zustellpuffer).
> Die sechs Monate sind eine **Ableitung aus zwei Fristen**, keine im Gesetz genannte Zahl; wer sie
> übernimmt, übernimmt die Ableitung mit. Andere Datenarten haben andere Fristen — deshalb Matrix.

**Belegt für 1.6 über:** **[Primär]** [gesetze-im-internet.de · § 15 AGG](https://www.gesetze-im-internet.de/agg/__15.html) ·
[gesetze-im-internet.de · § 61b ArbGG](https://www.gesetze-im-internet.de/arbgg/__61b.html) — beide am amtlichen Volltext gelesen, die Zwei- und die Drei-Monats-Frist stehen dort wörtlich.
**[Sekundär]** [datenschutz-grundverordnung.eu · Art. 17](https://datenschutz-grundverordnung.eu/dsgvo/art-17-dsgvo-recht-auf-loeschung-recht-auf-vergessenwerden/) ·
[dr-datenschutz.de · Löschpflicht und Verjährungsfristen](https://www.dr-datenschutz.de/loeschpflicht-und-verjaehrungsfristen/) ·
[dr-datenschutz.de · Aufbewahrungsfrist Bewerbungen](https://www.dr-datenschutz.de/aufbewahrungsfrist-wann-sind-bewerbungen-zu-loeschen/) — Abruf 20.09.2026.

---

## 2 · Künstliche Intelligenz

**Rechtsgrundlage:** Verordnung (EU) 2024/1689 (KI-Verordnung), geändert durch **Verordnung (EU)
2026/1744** (*Digital Omnibus on AI*), Amtsblatt 24.07.2026, in Kraft 27.07.2026.
**Belegt über:** [TÜV Rheinland Consulting](https://consulting.tuv.com/aktuelles/ki-im-fokus/digital-omnibus-ki-verordnung-fristen) ·
[Deloitte Deutschland](https://www.deloitte.com/de/de/issues/innovation-ai/eu-ai-act-digital-omnibus.html) ·
[activeMind.legal](https://www.activemind.legal/de/guides/aenderungen-ki-verordnung/) — Abruf 20.09.2026.
**Vertiefung im Repo:** [`bibliothek/eu-ai-act.md`](../bibliothek/eu-ai-act.md).

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **2.1** | **Risikoklasse bestimmt** — verboten, hoch, transparenzpflichtig, minimal | Art. 5, 6, 50 | Schriftliche Einstufungsentscheidung |
| **2.2** | **Rolle bestimmt**: Anbieter oder Betreiber — und geprüft, wann sie kippt | Art. 3, 25 | Rollenfeststellung je System. **Wer wesentlich umzweckt, wird Anbieter** |
| **2.3** | **Ausnahme nach Art. 6 Abs. 3** dokumentiert, **bevor** das System in Betrieb geht | Art. 6 Abs. 3 | Dokumentierte Bewertung. **Anbieterpflicht** — als Vertragsbedingung verlangen, nicht selbst erstellen |
| **2.4** | **Verbotene Praktiken** ausgeschlossen — u. a. Emotionserkennung am Arbeitsplatz und in Bildungseinrichtungen, Social Scoring | Art. 5 | Negativprüfung, dokumentiert |
| **2.5** | **KI-Kompetenz** der Beschäftigten, die mit dem System arbeiten | Art. 4 | Schulungsnachweis. **Gilt seit 02.02.2025, unabhängig von der Risikoklasse** |
| **2.6** | **Transparenz gegenüber Menschen**, die mit KI interagieren oder KI-Ausgaben erhalten | Art. 50 | Hinweistext, Kennzeichnung synthetischer Inhalte. **Gilt seit 02.08.2026, von der Fristverschiebung unberührt** |
| **2.7** | **Menschliche Aufsicht** mit **Eingriffsbefugnis** bei der Person, die sie trägt | Art. 14 | RACI mit benannter Person — und der Befugnis, das System anzuhalten |
| **2.8** | **Protokollierung** über die Lebensdauer | Art. 12, 19 | Aufbewahrungskonzept |
| **2.9** | **Registrierung und Konformitätsbewertung** vor Inbetriebnahme eines Hochrisikosystems | Art. 43, 49 | Eintrag in der EU-Datenbank |

> **Zwei Pflichten hängen nicht an der Fristverschiebung und gelten heute: 2.5 und 2.6.** Wer die
> Verschiebung als Entwarnung liest, übersieht genau die beiden, die sofort greifen.

---

## 3 · Datenrecht

**Rechtsgrundlage:** Verordnung (EU) 2023/2854 (**Data Act**), in Kraft 11.01.2024, **anwendbar seit
12.09.2025**. Die Pflicht zum Datenzugang **ab Werk** (*Access by Design*) gilt für vernetzte
Produkte, die **nach dem 12.09.2026** in Verkehr gebracht werden.
**Belegt über:** [Datenschutzkanzlei](https://www.datenschutzkanzlei.de/der-data-act-welche-pflichten-kommen-auf-unternehmen-zu/) ·
[SRD Rechtsanwälte](https://www.srd-rechtsanwaelte.de/blog/data-act-regelungen) ·
[Dentons](https://www.dentons.com/de/insights/alerts/2025/april/29/eu-data-act) — Abruf 20.09.2026.
*Die Dentons-Seite antwortet automatisierten Abrufen mit 403; im Browser erreichbar.*

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **3.1** | **Nutzerzugang zu Produktdaten** vernetzter Produkte ermöglicht | Data Act, Kap. II | Technische Schnittstelle, dokumentiert |
| **3.2** | **Access by Design** bei Produkten, die nach dem 12.09.2026 in Verkehr gebracht werden | Data Act | Architekturnachweis |
| **3.3** | **Faire Vertragsbedingungen** für Datenzugang und -weitergabe | Data Act, Kap. IV | Vertragsprüfung gegen die Missbrauchskontrolle |
| **3.4** | **Cloud-Wechsel** ohne unangemessene Hürden | Data Act, Kap. VI | Exit-Klausel, Portabilitätsnachweis |

> **Der Data Act wird in KI-Projekten regelmäßig übersehen**, weil er nicht nach KI klingt. Er
> entscheidet aber darüber, **an welche Daten man überhaupt herankommt** — und damit über die
> Datengrundlage, auf der jedes Modell steht.

---

## 4 · Informationssicherheit

**Rechtsgrundlage A:** Richtlinie (EU) 2022/2555 (NIS2), in Deutschland umgesetzt durch das
**NIS2-Umsetzungsgesetz (NIS2-RLUG)** — Bundesgesetzblatt **05.12.2025**, in Kraft **06.12.2025**,
**ohne Übergangsfrist**. Rund **29.500 Unternehmen** in **18 Sektoren**.
**Belegt über:** [OpenKRITIS](https://www.openkritis.de/it-sicherheitsgesetz/nis2-umsetzung-gesetz-cybersicherheit.html) ·
[RA Ferner](https://www.ferner-alsdorf.de/nis2-umsetzung-in-deutschland-2026/) — Abruf 20.09.2026.

**Rechtsgrundlage B:** Verordnung (EU) 2024/2847 (**Cyber Resilience Act**), in Kraft 10.12.2024.
**Die Meldepflichten gelten seit dem 11.09.2026** — auch für Produkte, die **vorher** auf dem Markt
waren. Volle Anwendbarkeit **11.12.2027**.
**Belegt über:** [Kanzlei Kramarz](https://kanzlei-kramarz.de/cyber-resilience-act-meldepflicht-software/) ·
[IHK Rhein-Neckar](https://www.ihk.de/rhein-neckar/recht/datenschutz-itrecht-internetrecht/it-sicherheit/cyber-resilience-act-pflichten-hersteller-6755242) — Abruf 20.09.2026.

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **4.1** | **Betroffenheit nach NIS2 geprüft** — Sektor, Größe, Schwellenwerte | NIS2-RLUG | Dokumentierte Einstufung |
| **4.2** | **Registrierung beim BSI** | NIS2-RLUG | Registrierungsbestätigung |
| **4.3** | **Risikomanagement** nach dem Stand der Technik | NIS2-RLUG | Maßnahmenkatalog, überprüft |
| **4.4** | **Meldekette für Sicherheitsvorfälle** eingerichtet | NIS2-RLUG | Erreichbarkeit rund um die Uhr, benannte Rolle |
| **4.5** | **Geschäftsleitung geschult und in der Pflicht** | NIS2-RLUG | Schulungsnachweis. **Die Haftung ist persönlich** |
| **4.6** | **CRA-Meldung**: 24 Stunden Frühwarnung, 72 Stunden vollständiger Bericht bei aktiv ausgenutzten Schwachstellen | CRA | Meldeprozess — **gilt seit 11.09.2026** |
| **4.7** | **CE-Kennzeichnung** für Produkte mit digitalen Elementen ab 11.12.2027 | CRA | Konformitätsnachweis |

> **4.6 ist der Punkt mit der kürzesten Vorlaufzeit im ganzen Plan.** Er gilt seit neun Tagen und
> erfasst **Bestandsprodukte**. Eine Meldefrist von 24 Stunden lässt sich nicht nachträglich
> organisieren.

---

## 5 · Haftung

**Rechtsgrundlage:** Richtlinie (EU) 2024/2853 (**Produkthaftungsrichtlinie**, Neufassung), in Kraft
09.12.2024, **Umsetzungsfrist bis 09.12.2026**. **Software, KI-Systeme und digitale Fertigungsdateien
gelten ausdrücklich als Produkte.**
**Belegt über:** [SKW Schwarz](https://www.skwschwarz.de/en/news/ki-flash-eu-produkthaftungsrichtlinie) ·
[Hogan Lovells](https://www.hoganlovells.com/en/publications/eu-introduces-comprehensive-digitalera-product-liability-directive) ·
[Reed Smith](https://www.reedsmith.com/articles/eu-product-liability-directive-software-digital-products-cybersecurity/) — Abruf 20.09.2026.

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **5.1** | **Produkteigenschaft geprüft** — eigenständige Software und KI-Systeme fallen darunter | RL 2024/2853 | Einordnung, dokumentiert |
| **5.2** | **Fehlerbegriff berücksichtigt**, einschließlich Cybersicherheitsmängeln und unterbliebener Updates | RL 2024/2853 | Update- und Supportzusage, schriftlich |
| **5.3** | **Offenlegungspflichten im Prozess** eingeplant — Dokumentation muss herausgabefähig sein | RL 2024/2853 | Beweismittelkonzept |
| **5.4** | **Umsetzung im nationalen Recht verfolgt**, Frist 09.12.2026 | RL 2024/2853 | Wiedervorlage |

---

## 6 · Urheberrecht und Geschäftsgeheimnisse

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **6.1** | **Rechtsgrundlage für Trainingsdaten** geklärt; Nutzungsvorbehalte maschinenlesbar beachtet | § 44b UrhG (Text und Data Mining) · Art. 53 KI-VO | Herkunftsnachweis je Datenquelle |
| **6.2** | **Keine Geschäftsgeheimnisse in fremde Modelle** ohne vertragliche Absicherung | GeschGehG | Nutzungsregel plus AVV |
| **6.3** | **Urheberrechts-Policy des Modellanbieters** eingefordert | Art. 53 KI-VO | Anbietererklärung |

> **Abschnitt 6 ist der am schwächsten belegte dieses Plans.** Die Fundstellen sind zutreffend
> benannt, aber **nicht mit derselben Quellenlage geprüft** wie die Abschnitte 2 bis 5. Siehe
> *Lücken* unten.

---

## 7 · Arbeitsrecht

| | Prüfpunkt | Folgt aus | Nachweis |
|---:|---|---|---|
| **7.1** | **Mitbestimmung** bei Systemen, die zur Verhaltens- oder Leistungskontrolle **geeignet** sind | § 87 Abs. 1 Nr. 6 BetrVG | Betriebsvereinbarung. **Die Eignung genügt, die Absicht ist unerheblich** |
| **7.2** | **Diskriminierungsfreiheit** bei Auswahl- und Bewertungssystemen | AGG | Verzerrungsprüfung, dokumentiert |
| **7.3** | **Beschäftigtendatenschutz** | § 26 BDSG | Zweckbindung, dokumentiert |

> **7.1 wird regelmäßig zu spät geprüft.** Die Mitbestimmung knüpft an die **Eignung** zur
> Kontrolle an — ein Protokoll, das man auswerten *könnte*, löst sie aus.

---

## Teil B · Fristen, die beschlossen sind

| Datum | Was | Rechtsakt |
|---|---|---|
| 25.05.2018 | DSGVO anwendbar | VO (EU) 2016/679 |
| 02.02.2025 | **KI-Kompetenz** (Art. 4) und verbotene Praktiken (Art. 5) | VO (EU) 2024/1689 |
| 12.09.2025 | **Data Act anwendbar** | VO (EU) 2023/2854 |
| 06.12.2025 | **NIS2-Umsetzungsgesetz in Kraft**, ohne Übergangsfrist | NIS2-RLUG |
| 02.08.2026 | **Transparenzpflichten** (Art. 50) — von der Verschiebung **unberührt** | VO (EU) 2024/1689 |
| **11.09.2026** | **CRA-Meldepflichten**, 24 h / 72 h, auch für Bestandsprodukte | VO (EU) 2024/2847 |
| 12.09.2026 | **Access by Design** für neu in Verkehr gebrachte vernetzte Produkte | VO (EU) 2023/2854 |
| 09.12.2026 | Umsetzungsfrist **Produkthaftung** in nationales Recht | RL (EU) 2024/2853 |
| 02.12.2026 | Zwei **neue Verbote** in der KI-Verordnung | VO (EU) 2026/1744 |
| **02.12.2027** | **Anhang-III-Hochrisikopflichten** — verschoben von 02.08.2026 | VO (EU) 2026/1744 |
| 11.12.2027 | **CRA vollständig anwendbar**, CE-Kennzeichnung | VO (EU) 2024/2847 |
| 02.08.2028 | **Anhang-I-Hochrisikopflichten** | VO (EU) 2026/1744 |

> **Die Verschiebung ist keine Entlastung, sondern eine Umsortierung.** Zwischen dem 11.09.2026 und
> dem 11.12.2027 greifen fünf Fristen aus vier verschiedenen Rechtsakten. Wer nur die KI-Verordnung
> verfolgt, sieht davon eine.

---

## Teil C · Exkurs — was debattiert wird, aber **nicht** beschlossen ist

> **Alles in diesem Teil ist Erwartung, keine Pflicht.** Es gehört in die Planung, nicht in eine
> Compliance-Aussage. Wer diese Punkte wie geltendes Recht behandelt, macht denselben Fehler wie
> jemand, der beschlossene Fristen ignoriert — nur in die andere Richtung.

**① Haftung für KI, eigenständig geregelt.** Eine gesonderte **KI-Haftungsrichtlinie** mit
widerlegbaren Kausalitätsvermutungen war geplant und ist nach der Quellenlage im Repository
**zurückgezogen** worden; die Neufassung der Produkthaftung (Abschnitt 5) trägt den Gegenstand
seither allein. **Ob das reicht, ist offen** — die Debatte um eine Beweislastumkehr bei
undurchsichtigen Systemen läuft weiter. *Nicht unabhängig verifiziert; siehe Lücken.*

**② Weitere Vereinfachungsvorhaben.** Der *Digital Omnibus* war der erste seiner Art. Weitere
Bündel zur Vereinfachung des digitalen Rechtsrahmens sind angekündigt und teils im Verfahren.
**Was darin steht, ist bis zur Veröffentlichung im Amtsblatt kein Recht** — und der erste Omnibus
hat gezeigt, dass sich Fristen dabei um **sechzehn Monate** verschieben können.

**③ Beschäftigtendatenschutz, eigenes Gesetz.** Ein eigenständiges Beschäftigtendatenschutzgesetz
wird seit Jahren diskutiert; § 26 BDSG gilt bis dahin. Für KI-gestützte Personalentscheidungen wäre
es der Punkt mit der größten praktischen Wirkung.

**④ Verhältnis von KI-Verordnung und DSGVO.** Ob und wie sich Art. 22 DSGVO
(automatisierte Einzelentscheidung) und Art. 14 KI-VO (menschliche Aufsicht) überlagern, ist
nicht abschließend geklärt. **Praktisch heißt das: beide erfüllen, nicht eines auswählen.**

---

## Lücken — was dieser Plan **nicht** belegt

| | Was fehlt | Warum es zählt |
|---:|---|---|
| **L1** | **Kein Unionsrechtsakt im Volltext am Amtsblatt geprüft.** Daten und Nummern stammen aus Sekundärquellen — **außer** § 15 AGG und § 61b ArbGG, die am amtlichen Volltext gelesen sind | Eine falsche Verordnungsnummer macht jeden Verweis wertlos |
| **L2** | **Abschnitt 6** (Urheberrecht, Geschäftsgeheimnisse) ist nicht auf demselben Stand belegt wie 2 bis 5 | Trainingsdaten sind der Punkt, an dem Modellprojekte rechtlich am häufigsten kippen |
| **L3** | **Data Governance Act** (VO (EU) 2022/868) ist **nicht aufgenommen** | Er regelt Datenmittler und Datenaltruismus — relevant, sobald Daten Dritter einbezogen werden |
| **L4** | **Der Rückzug der KI-Haftungsrichtlinie** ist nur über die Repository-eigene Quellenlage belegt | Teil C ① steht und fällt damit |
| **L5** | **Fünfzehn der sechzehn Fundstellen wurden am 20.09.2026 maschinell auf Erreichbarkeit geprüft** (HTTP 200), die sechzehnte blockt Automaten | Eine tote Fundstelle ist keine Fundstelle — der Test gehört wiederholt, nicht einmal gemacht |

## Änderungsvermerk

| Datum | Was | Warum |
|---|---|---|
| 2026-09-20 | Erstfassung. Sieben Rechtsakte belegt, vier Lücken benannt | Der Kurs behandelt Recht, setzt es aber nicht — ein Prüfraster muss aus den Rechtsakten kommen |
| 2026-09-20 | **Prüfpunkt 1.6 (Aufbewahrungsmatrix) neu**, alt 1.6–1.8 zu 1.7–1.9 umnummeriert. Abschnitt 1 hat neun statt acht Punkte, der Plan 39 statt 38 | Der Plan verlangte in 1.5 nachweisbare Löschung, ohne zu verlangen zu wissen, **was nicht gelöscht werden darf**. Das war die einzige Stelle, an der korrektes Abarbeiten Schaden anrichtet — Beweismittel weg, Anspruch trotzdem da. Gefunden bei der Anwendung auf einen Fall, nicht bei der Erstfassung |
| 2026-09-20 | Frontmatter zählt jetzt **Prüfpunkte und Rechtsgebiete**, nicht mehr *„sieben Rechtsakte“* | Die alte Angabe war nicht nachzählbar: der Plan nennt in sieben Abschnitten mehr als sieben Rechtsakte (allein Abschnitt 1 vier). Eine Zahl, die man nicht nachzählen kann, gehört nicht ins Frontmatter |

## Empfehlung

**Typ: To-do.**

1. **L1 zuerst schließen, und zwar für die vier Fristen, die 2026 und 2027 greifen.** Verordnungsnummer
   und Datum am Amtsblatt nachschlagen kostet je zehn Minuten. Solange das nicht geschehen ist, trägt
   dieser Plan die Orientierung, aber keine Aussage in einer Vorlage.
2. **Prüfpunkt 4.6 sofort behandeln, unabhängig vom übrigen Plan.** Die CRA-Meldepflicht gilt seit
   dem 11.09.2026, erfasst Bestandsprodukte und lässt 24 Stunden. Sie ist der einzige Punkt hier, bei
   dem Verzug unmittelbar sanktionsbewehrt ist.
3. **Teil C bei jeder Wiedervorlage gegen Teil B prüfen.** Ein Punkt, der aus der Debatte ins
   Amtsblatt wandert, muss die Tabelle wechseln — und die Erfahrung mit dem Digital Omnibus zeigt,
   dass das schnell gehen kann.
