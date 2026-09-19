# Whitepaper · LHIND „Responsible AI: Der EU AI Act als Grundlage für erfolgreiche KI-Anwendungen"

**Bibliothekseintrag – Steckbrief zu fremdem Material, Regelschicht**
Quelle: Lufthansa Industry Solutions, 8 Seiten, © LHIND 4–2025 · Datei: `whitepapers/responsible-ai-cmyk-wp-de-lhind.pdf` *(nicht oeffentlich: `responsible-ai-cmyk-wp-de-lhind.pdf`)*
Angelegt: 2026-09-19 · Status: **geprüft gegen [`eu-ai-act.md`](eu-ai-act.md).** Zwei sachliche Fehler gefunden
Anschluss: [`eu-ai-act.md`](eu-ai-act.md)
Geltung: **firmenunabhängig.** Kein Fallwert, kein Mandantenbezug

> **Belegstatus vorweg.** Dies ist **anbieterfinanziertes Material**. Lufthansa Industry Solutions
> verkauft Beratung zu genau diesem Thema; die Fußzeile des Papiers nennt
> `marketing.sales@lhind.dlh.de`. **Das macht es nicht falsch, aber es macht es zu einer Quelle,
> die man gegenliest statt zitiert.** Die PDF liegt im Repository und ist **von der öffentlichen
> Fläche gesperrt** — fremdes, urheberrechtlich geschütztes Material, dieselbe Regel wie beim
> ISO-Normtext.

## 1 · Wozu es taugt

Eine **achtseitige Einführung** in die Systematik der KI-Verordnung, in verständlichem Deutsch und
ohne Juristendeutsch. Für den ersten Überblick brauchbar: Es erklärt, dass die Verordnung nach
Risiko klassifiziert, nennt vier Klassen, und benennt die Pflichtenrichtung (Risikomanagement,
Datenqualität, Dokumentation, menschliche Aufsicht, Registrierung, Konformitätsbewertung).

**Für eine Einordnung des eigenen Vorhabens taugt es nicht.** Warum, steht unten.

## 2 · Zwei sachliche Fehler, beide für unseren Fall einschlägig

### 2.1 Emotionserkennung und biometrische Kategorisierung stehen unter *begrenztem Risiko*

Das Papier schreibt unter **Begrenztes Risiko**:

> *„In diese Kategorie fallen Systeme, die mit Menschen interagieren und bei denen die Gefahr der
> Manipulation oder Täuschung besteht. Dazu gehören Systeme zur Emotionserkennung und
> biometrischen Kategorisierung oder Chatbots."*

**Das flacht drei verschiedene Fälle auf einen ab.** Nach [`eu-ai-act.md`](eu-ai-act.md) § 2 und § 3:

| Fall | Tatsächliche Klasse |
|---|---|
| Emotionserkennung **am Arbeitsplatz und in Bildungseinrichtungen** | **Verboten**, Art. 5 |
| Biometrische Kategorisierung nach **sensiblen Merkmalen**, Emotionserkennung sonst | **Hochrisiko**, Anhang III Nr. 1 |
| Chatbots, Systeme mit direktem Menschkontakt | **Transparenzpflichtig**, Art. 50 |

**Warum die Verkürzung teuer ist:** Wer Emotionserkennung **am Arbeitsplatz** erwägt und diesem
Papier folgt, hält einen **verbotenen** Tatbestand für die zweitniedrigste Stufe.

### 2.2 Anhang III Nr. 4 — Beschäftigung — fehlt vollständig

Unter **Hohes Risiko** nennt das Papier genau zwei Gruppen: *„produktbezogene KI-Systeme
(Medizintechnik, Fahrzeuge) und Systeme für kritische Infrastrukturen"*. Das sind Anhang I und
Anhang III Nr. 2.

**Die übrigen sieben Bereiche aus Anhang III kommen nicht vor** — darunter **Nr. 4, Beschäftigung
und Personalmanagement**, ausdrücklich mit Filterung von Bewerbungen und Bewertung von Kandidaten.

**Wer in Personalauswahl, Bildung, Kreditvergabe, Strafverfolgung, Migration oder Justiz arbeitet,
kommt nach diesem Papier zu dem Schluss, nicht betroffen zu sein.** Das sind sechs der acht
Hochrisikobereiche.

## 3 · Und ein überholter Fristenstand

> *„Diese Systeme werden ab 2026 streng reguliert."*

Das Papier stammt aus **4-2025**. Die **Verordnung (EU) 2026/1744** — Amtsblatt 24.07.2026 —
verschiebt die Anhang-III-Pflichten auf **02.12.2027**. Der Digital Omnibus kommt im Papier
**null mal** vor, was bei einem Stand von 2025 zu erwarten ist.

**Bemerkenswert ist nicht der Fehler, sondern die Gesellschaft, in der er steht:**
`coursebook/woche-5/5.0` führt denselben überholten Stand als **erste von drei Korrekturen** an
seinem eigenen Material. Ein Anbieterpapier von 2025 und ein Kursfoliensatz von 2026 machen
denselben Fehler — **unser Bibliothekseintrag hatte ihn am 18.09. schon richtig.**

## 4 · Wie damit umgehen

- **Nicht in eine Entscheidungsvorlage zitieren.** Weder die Klassifizierung noch die Fristen.
- **Als Gegenlesung brauchbar:** Wer die eigene Einordnung gegen dieses Papier hält und die
  Abweichungen begründen kann, hat die Einordnung verstanden. Genau das ist hier passiert.
- **Als Beispiel im Kurs brauchbar:** ein belegter Fall dafür, dass ein professionell gestaltetes
  Anbieterpapier in zwei Punkten falsch liegt — und dass der Fehler nur auffällt, wenn man eine
  eigene, extern belegte Fassung danebenlegt.

## Änderungsvermerk

| Datum | Was | Warum |
|---|---|---|
| 2026-09-19 | Angelegt, gegen `eu-ai-act.md` geprüft | Drei Whitepaper sollten in den Viewer. Der Viewer rendert kein PDF — und ein PDF, das man nur ablegt, ist nicht eingeordnet |

## Empfehlung

**Typ: Anweisung.**

1. **Dieses Papier nicht zitieren, sondern als Gegenprobe benutzen.** Beide Fehler betreffen die
   Einordnung selbst — der zweite besonders, weil er ganze Hochrisikobereiche verschwinden lässt.
2. **Befund 2.2 als Lehrbeispiel verwenden.** Ein professionell gestaltetes Anbieterpapier, das
   sechs von acht Hochrisikobereichen auslässt, zeigt deutlicher als jede Folie, warum eine eigene
   Einordnung nötig ist.
3. **Bei jedem weiteren Anbieterpapier zuerst die Klassifizierung gegenlesen.** Sie ist die Stelle,
   an der ein Marketingtext am billigsten vereinfacht — und die einzige, die über die eigene
   Betroffenheit entscheidet.
