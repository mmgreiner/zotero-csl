# zotero-csl

A dedicated Zotero citation style for Swiss Legal Documents, adopted for Kanton Luzern

## Zweck

[Zotero][zotero] ist ein open source Werkzeug, um eine Bibliographie anzulegen und zu verwalten. 

So können z.B. alle Luzerner Gesetze, die sogenannte [Systematische Rechtssammlung Luzern](https://srl.lu.ch/app/de/systematic/texts_of_law), einzeln in Zotero erfasst werden, und anschliessend einfach zitiert werden.

Für diese Zitierfunktion braucht es den Microsoft Word Plugin von Zotero. Dieser er kommt normalerweise zusammen mit der Installation von Zotero (siehe [Installation word-plugin](https://www.zotero.org/support/word_processor_plugin_installation)).

[zotero]: https://www.zotero.org/

Jetzt muss man aber dem Plugin noch mitteilen, in welcher Form genau zitiert werden soll, und wie die Bibliothek aussehen soll. Hierzu gibt es Duzende von Anweisungen, so z.B. die [Zitierreglen des Schweizer Bundesgerichts][zitierregeln-bger]. 


[zitierregeln-bger]: https://www.bger.ch/files/live/sites/tfl/files/pdf/Reglemente/01_Zitierregeln_d.pdf

Aber wie kommen diese Zitierregeln in das Word-Dokument? Hierfür braucht es entsprechende Zotero Styles, welche in einem standardisierten XML Format, dem [Citation Style Language (CSL)](http://citationstyles.org/) geschrieben sind.
Es gibt Hunderte dieser [Zitero Styles](https://www.zotero.org/styles) aus allen Bereichen der Wissenschaft.

## Citation Style für Kanton Luzern

Für den Kanton Luzern wurde ein Citation Style entwickelt, der sich eng an den bestehenden [ZitierGuide: Leitfaden zum fachgerechten Zitieren in rechtswissenschaftlichen Arbeiten (Roger Müller) (Deutsch - Schweiz)][zitierguide] hält.

Es wurden zwei Fälle angepasst: SRL und Berichte.

### Systematische Rechtssammlung Luzern

Gesetze können im Zotero mit folgenden Werten erfasst werden:

| Schlüssel | Wert |
|-----------|------|
| Eintragsart / *Item type* | Gesetz / *Statute* |
| Titel / *Title* | Berufungsreglement der Universität Luzern |
| Code | Systematische Rechtssammlung Kanton Luzern (SRL) |
| Codenummer | SRL |
| Öffentliche Gesetzesnummer | 539d |
| Datum des Inkrafttretens | 2002 |
| URL | <https://srl.lu.ch/app/de/texts_of_law/539d> |

Als Referenz ergibt dies:

    (SRL Nr. 539d)

und als Bibliographieeintrag:

    SRL Nr. 539d, Berufungsreglement der Universität Luzern, vom 2002, https://srl.lu.ch/app/de/texts_of_law/539d

### Berichte

Für alle internen Berichte wie Aktennotizen, Regierungsratsbeschlüsse usw kann ein Dokument in Zotero folgendermassen erfasst werden:

| Schlüssel | Wert |
|-----------|------|
| Eintragsart / *Item type* | Bericht / *Report* |
| Titel / *Title* | Lagebericht zum Stand der KI |
| Nummer des Berichts / *Report Number* | 2026-123 |
| Art von Bericht / *Report Type* | RRB |
| Autor / *Author* | Greiner, Markus |
| Extra | Jurisdiction: LU |

Dies erstellt eine Referenz wie folgt:

    (GREINER, Nr. 2026-1234)

Und erscheint in der Bibliographie als:

    GREINER MARKUS, Lagebericht zum Stand der KI, RRB, Nr. 2026–123

[zitierguide]: https://www.zotero.org/styles/zitierguide-leitfaden-zum-fachgerechten-zitieren-in-rechtswissenschaftlichen-arbeiten

## Installation

* Lade die Datei `luzern-law-intext_1.csl` herunter.
* Anschliessend in Zotero, gehe zu `Bearbeiten --> Einstellungen`.
* Mit dem Knopf `Aus Datei hinzufügen`, wähle die die Datei `luzern-law-intext_1.csl` aus.

Viel Erfolg 👍
