# LaTeX @ILEK
Diese Vorlage dient als grober Leitfaden zu Erstellung der Abschlussarbeit. Die Formatierung ist somit nicht zwingend umzusetzen.

Die Formatierung des Deckblattes sollte, soweit möglich, unverändert bleiben. 

Von der Gliederung der Arbeit kann abgewichen werden, solang dieses sinnig begründbar ist.

# LaTeX Grundlagen
Um mit LaTeX zu Arbeiten, wird einerseits ein Editor und andererseits eine LaTeX-Distribution benötigt. Der Editor dient hierbei zur Eingabe des LaTeX-Code, die LaTeX-Distribution übersetzt den Code in ein Dokument. 

Beispielsweise kann eine Kombination der folgende Programme verwendet werden:

1. MiKTeX https://miktex.org/download (LaTeX-Distribution)

1. TeXstudio https://www.texstudio.org/ (Editor)

Alternativ besteht auch die Möglichkeit Online-Dienste zu benutzen, welche mögliche Schwierigkeiten bei der Einrichtung der oben genannten Lösung umgehen. Diese vereinen Editor und LaTeX-Distribution.

1. Overleaf https://de.overleaf.com/

Für eine problemlose Kompilierung des \LaTeX-Dokumentes ist es notwendig, einige Einstellungen in den Editor zu übernehmen.

1. Als Standardcompiler wird LuaLaTeX oder PdfLaTeX empfohlen. Lediglich bei LuaLaTeX wird die offizielle Schrift der Universität Stuttgart unterstützt. Diese ist online nicht verfügbar und muss bei den Betreuuern angefragt werden.

1. Als Standard Bibliographieprogramm sollte Biber ausgewählt werden

# Hinweis zur Abgabe

## Gedrucktes Exemplar
In der Regel sollten insgesamt zwei Examplare an das ILEK ausgehändigt werden. Für den Druck gelten die folgenden Empfehlungen:

- Dickeres Papier (z.B. 100-120 g/m²)
- Softcover mit Kaltleimbindundung
- Für den Einband sollte der [Umschlag](#01_frontcover) verwendet werden 

Die Auswahl eines ein- oder doppelseitigen Druckes richtet sich nach der Seitenzahl. Bis ca. 50 Seiten wird ein einseitiger Druck empfohlen, darüber hinaus ein doppelseitiger.

Wichtig bei der Auswahl eines ein- oder doppelseitigen Druckes ist das LaTeX-Dokument entsprechend anzupassen. Dadurch werden die Seitenränder und Seitenzahl korrekt ausgerichtet.

- Doppelseitiger Druck: In der main.tex-Datei die Option `<twoside>` auswählen
- Einseitiger Druck: In der main.tex-Datei die Option `<twoside>` auskommentieren (Standarteinstellung)

Mit diesen Informationen einfach an das Kopiergeschäft herantreten, diese wissen meist was zu tun ist.

## Digitales Exemplar (PDF)
Hierfür in der main.tex-Datei die Option `<twoside>` auskommentieren (Standarteinstellung).

Bitte die Arbeit in digitaler Form auf einer CD speichern und einem der gedruckten Exemplare beilegen. Die CD sollte ebenso das LaTeX-Dokument, alle Abbildung und die während der Arbeit erstellten Berechnungen (bswp. in Form von Excel-Tabellen, Programmcode oder FE-Berechnungen ohne Ergebnisse) enthalten.

### literatur.bib

Enthält die Daten für das Literaturverzeichnis der Arbeit. Keine Anpassungen notwendig.

Empfohlen wird die Verwaltung und Anfertigung des Literaturverzeichnisses mit den folgenden Programmen. Es bietet sich an bereits zu beginn der Abschlussarbeit alle Quellen mit den genannten Programmen zu verwalten

1. Citavi https://www.citavi.com/de

1. Zotero https://www.zotero.org/

## 00_ressources
Enthält notwendige Einstellungen und Dateien für LaTex.

### preambel.tex
In der Präambel werden alle für das gesamte Dokument gültigen Formatierungseinstellungen getroffen sowie zusätzlich benötigte Pakete geladen. Keine Anpassungen notwendig.

### variables.tex
Enthält alle wichtigen Angaben (Titel, Betreuer, Jahr ..) zur Arbeit. Diese müssen entsprechend angepasst werden sodass Einband und Titelblatt mit den richtigen Informationen erstellt werden.

### fonts
Enthält die Schriftart der Universität Stuttgart. Aufgrund der Lizenzierung der Schrift dürfen wir die dafür notwendigen Dateien nicht über GitHub zu Verfügung stellen. 

Daher entweder den Betreuer der Arbeit nach den entsprechenden Dateien fragen oder alternativ Arial verwenden (automatisch eingestellt wenn die Schriftart Univers for UniS nicht gefunden wird).

Die Schriftarten der Universität Stuttgart müssen wie folgt benannt werden:

- UniversforUniS45LtObl-Rg
- UniversforUniS55Rm-Regular
- UniversforUniS65Bd-Regular

### tikz
Durch Tikz Kompilierte Grafiken. Keine Anpassungen notwendig.
