## 2017-05-eng-heizungen

Dieses Dokument beschreibt die Vorprozessierung und explorative Analyse des Datensatzes, der Grundlage des auf srf.ch veröffentlichten Artikel [Klimafreundliche Heizungen: So gross sind die Unterschiede in den Kantonen](http://www.srf.ch/news/schweiz/abstimmungen/abstimmungen/energiestrategie/so-gross-sind-die-unterschiede-in-den-kantonen) ist.

SRF Data legt Wert darauf, dass die Datenvorprozessierung und -Analyse nachvollzogen und überprüft werden kann. SRF Data glaubt an das Prinzip offener Daten, aber auch offener und nachvollziehbarer Methoden. Zum anderen soll es Dritten ermöglicht werden, auf dieser Vorarbeit aufzubauen und damit weitere Auswertungen oder Applikationen zu generieren.  

Die Vorprozessierung und Analyse wurde im Statistikprogramm R vorgenommen. 

Originalquelle der Daten ist die auf Gemeindeebene aggregierte [Gebäude- und Wohnungsstatistik (GWS)](https://www.bfs.admin.ch/bfs/de/home/statistiken/bau-wohnungswesen/erhebungen/gws2009.html) für die Jahre 2009-2015 (siehe Abschnitt "Originalquelle"). Für die Aggregation auf Kantonsebene wurden die jeweiligen [statistischen Raumgliederungen](https://www.bfs.admin.ch/bfs/de/home/grundlagen/raumgliederungen.html) des entsprechenden Jahres zu Hilfe genommen. 

Die Endprodukte des vorliegenden Scripts, neben der vorliegenden explorativen Analyse, sind (Datenbeschreibung siehe unten):

* `energietraeger.csv`: Anteil Wohngebäude mit Heizungssystemen nach Energieträger, aggregiert auf Kantonsebene, Jahr 2015.
* `klimafreundlich.csv`: Anteil Wohngebäude mit klimafreundlichen Heizungssystemen und Unterschied zu 2009, aggregiert auf Kantonsebene, Jahr 2015.

### R-Script & Daten

Das zugrunde liegende Script sowie die prozessierten Daten können unter [diesem Link](https://srfdata.github.io/2017-05-eng-heizungen/rscript.zip) heruntergeladen werden. Durch Ausführen von `main.Rmd` kann der hier beschriebene Prozess nachvollzogen und der für den Artikel verwendete Datensatz generiert werden. Dabei werden Daten aus dem Ordner `input` eingelesen und Ergebnisse in den Ordner `output` geschrieben. 

### GitHub

Der Code für die vorliegende Datenprozessierung ist auf [https://github.com/srfdata/2017-05-eng-heizungen](https://github.com/srfdata/2017-05-eng-heizungen) zur freien Verwendung verfügbar. 

### Lizenz

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">2017-05-eng-heizungen</span> von <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/srfdata/2017-05-eng-heizungen" property="cc:attributionName" rel="cc:attributionURL">SRF Data</a> ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.