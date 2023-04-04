# LA1500
# Projekt-Dokumentation



 Orchid: Gilardoni, Goedertier, Raviraj und Koch

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   21.02    | 0.0.1   | Projekt definieren, User Stories machen und zwei Diagramme zu unserem Projekt erstellen |
|     28.02  | 0.0.2  |          Wir haben unsere Arbeit für die nächsten Wochen geplant und haben die Testfälle ausgearbeitet                                                   |
|   07.03    | 1.0.0   |          Wir haben angefangen die User Stories abzuarbeiten.                                   |
|   14.03    | 1.1.0   |          Wir haben weiter an unseren User Stories gearbeitet.                                   |
|   21.03    | 1.1.0   |          Wir haben weiter an unseren User Stories gearbeitet, bei denen wir stehen geblieben sind und haben eine Präsentation erstellt.                                |

# 1 Informieren

### 1.1 Ihr Projekt

Wie programmieren mit C#  (Unity) ein Tower-Defense spiel.

Wir programmieren ein Tower-Defense spiel. Dessen Prinzip ist das die Gegner eine festgelegte Strecke ab laufen, dabei können Türme neben der Strecke gebaut werden, um zu verhindern, dass die Gegner Das Ziel (unsere Basis) erreichen. Doch für den Spieler wird es immer komplizierter, da immer mehr Gegner kommen aber er die Strecke nicht verändern kann und somit die Länge immer gleich bleibt, die verwendet werden kann, um die Gegner zu stoppen.

Für unser Spiel benutzen wir die Programmiersprache c# und verwenden Unity mit der Kollaboration Funktion.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |    muss        |   funktional   | Als Entwickler möchte ich, dass wenn man das Spiel startet ein Hauptmenü erscheint, damit der Spieler nicht direkt in die Runde gezwungen wird. |
| 2    |           muss      |   funktional   | Als Spieler möchte ich, dass es ein Startknopf im Hauptmenü gibt, damit ich eine Runde starten kann. |
| 3    |  muss               |   rand         | Als Spieler möchte ich, dass das Spiel Musik hat, damit ich mehr Spass habe und es meine Erfahrung besser macht. |
| 4    |  muss             |   rand         | Als Spieler möchte ich, dass es ein Einstellungen-Knopf im Hauptmenü gibt, damit ich die Musiklautstärke anpassen kann. |
| 5    |         muss        |    funktional  | Als Spieler möchte ich, dass es verschiedene Türme gibt, mit denen ich mich von Gegnern schützen kann. |
| 6    |         muss        |  funktional    | Als Spieler möchte ich, dass es mehrere Runden gibt, damit man eine höhere Herausforderung beim Spielen hat. |
| 7    |    muss             |  funktional    | Als Spieler möchte ich Geld von besiegten Gegner erhalten, damit ich reich werden kann. |
| 8    |       muss          |    funktional  | Als Entwickler möchte ich, dass jede Runde mehr Gegner erscheinen, damit der Spieler es schwerer hat zu gewinnen. |
| 9    |  muss          |   funktional   | Als Entwickler möchte ich, dass wenn man verliert, man ein Todes-Menü hat, damit man die Runde neu starten kann oder ins Hauptmenü zurückgehen kann. |
| 10   |         muss        |  funktional    | Als Spieler möchte ich, dass es ein Beenden-Knopf im Hauptmenü gibt, damit ich das Spiel schliessen kann. |
| 11   |           kann      |   rand         | Als Spieler möchte ich verschiedene Gegnertypen haben, damit meine Spielerfahrung besser ist.  |
| 12   |    kann             |   rand         | Als Entwickler möchte ich, dass verschiedene Gegnertypen unterschiedlich viel Leben abziehen, wenn sie das Ziel erreichen, damit der Spieler mehr aufpassen muss. |
| 13   |  kann               |   rand         | Als Spieler möchte ich meine Türme verbessern können, mit erlangtem Geld durch das besiegen von Gegnern, damit ich eine höhere Chance habe das Spiel zu gewinnen.  |
| 14   |  muss               |   funktional   | Als Spieler möchte ich mich frei auf der Map bewegen können, damit ich alles beobachten kann. |
| 15   |  kann               |   rand         | Als Spieler möchte ich, dass es am Anfang vom Spieler einen Timer von 30 Sekunden hat, damit ich eine gewisse Zeit habe mich für die erste Welle an Gegnern vorzubereiten. |
| 16   |  muss               |   funktional   | Als Entwickler möchte ich, dass das Spiel eine 'Hauptmap' hat, damit der Spieler sieht wo er was machen kann in einer Runde. |
| 17   |  kann               |   rand         | Als Spieler möchte ich, dass das Spiel verschiedene Maps hat, damit ich abwechslungsweise diese Maps spielen kann. |


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Das Spiel wird gestartet | Nichts | Das Hauptmenü erscheint. |
| 2.1  | Das Spiel wird gestartet | Man drückt die Taste 'Start' | Runde wird gestartet. |
| 3.1  | Das Spiel wird gestartet | Nichts | Man hört Musik im Hintergrund. |
| 4.1  | Das Spiel wird gestartet | Man drückt die Taste 'Optionen' | Das Fenster 'Optionen' wird geöffnet. |
| 5.1  | Die Runde wird gestartet | Man drückt auf einen Turm in der Auswahl | Man kann den Turm frei auf der Map setzen, solange er nicht zu nahe an einem anderen Objekt/Turm ist.|
| 6.1  | Die Runde wird gewonnen | Nichts | Es spawnen neue Gegner und der Rundenzähler geht eine Stelle nach oben. |
| 7.1  | Ein Gegner wird besiegt | Nichts | Die Münzen/Geld Anzahl des Spielers geht hoch.|
| 8.1  | Nächste Runde wird gestartet | Nichts | Die Gegner-Welle ist grösser als in der vorherigen Runde. |
| 9.1  | Man verliert/stirbt im Spiel | Neustart Taste wird gedrückt | Die Runde wird neu gestartet und man fängt von vorne an, also Runde 1. |
| 9.2  | Man verliert/stirbt im Spiel | Hauptmenü Taste wird gedrückt | Das Hauptmenü erscheint, wie wenn man das Spiel neu aufgestartet hat. |
| 10.1 | Man ist im Hauptmenü | Beenden Taste wird gedrückt. | Das Spiel schliesst sich. |
| 11.1 | Man erreicht eine gewisse Runde | Nichts | Neue Gegner erscheinen, die eine gewisse spezielle Fähigkeit haben (Schnelligkeit, Resistenz, Stärke, usw.). |
| 12.1 | Ein Gegner des Typen 'Normal' kommt ins Ziel | Nichts | Es wird 1 Leben abgezogen. |
| 12.2 | Ein Gegner des Typen 'Stark' kommt ins Ziel | Nichts | Es werden 5 Leben abgezogen. |
| 12.3 | Ein Gegner des Typen 'Boss' kommt ins Ziel | Nichts | Es werden alle Leben abgezogen. |
| 13.1 | Man hat einen gewissen Turm mit genug Geld um ihn zu verbessern. | Man drückt beim Turm auf 'Verbessern' | Dem Spieler wird die gebrauchte Menge an Geld abgezogen und der Turm wird verbessert. |
| 13.2 | Man hat einen gewissen Turm mit ungenügend viel Geld, um ihn zu verbessern | Man drückt beim Turm auf 'Verbessern' | Es wird gesagt, dass der Spieler nicht genug Geld hat und der Turm wird nicht verbessert. |
| 14.1 | Man hat eine Figur als Spieler in der Runde | Man drückt WASD | Die Figur bewegt sich auf der Map herum. |
| 15.1 | Man ist im Hauptmenü | Man drückt auf den Startknopf | Die Runde wird gestartet und man sieht auf dem Bildschirm einen Timer von 30 Sekunden herunterzählen. |
| 16.1 | Die Runde wird gestartet | Nichts | Die Figur des Spielers ist auf einer schon vorbereiteten Map. |
| 17.1 | Man ist im Hauptmenü | Man drückt den Startknopf | Bevor die Runde anfängt, kann der Spieler aus einem Sortiment von mehreren Maps eine davon auswählen. |



### 1.4 Diagramme
<img![image](https://user-images.githubusercontent.com/110893121/220322745-6f710a14-7274-4404-822a-a6fa3db3cd10.png)


<img src="https://user-images.githubusercontent.com/110891995/220317206-28ad02f3-9c1a-4012-bf51-e1c00ce3ca2f.png" width="300">

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |  7.3     |    Koch       |       Eine Hauptmenu erstellen.       |        45 min.       |
| 2.A  |    7.3   |   Koch        |     Einen Startknopf im Hauptmenu einfügen         |       45 min.        |
| 3.A  |    7.3   |   Gilardoni        |     Musik auswählen       |       45 min.        |
| 3.B  |   14.3   |   Gilardoni        |     Musik einfügen      |       45 min.        |
| 4.A  |    7.3   |    Raviraj     |     Knopf für Einstellungen und ein Fester für die Einstellungen      |       45 min.        |
| 4.B  |    7.3   |    Raviraj     |     In der Einstellung die Musik leiser oder lauter stellen können.     |       45 min.        |
| 16.A  |    7.3   |   Goedertier    |    Eine Hauptmap erstellen.    |       45 min.        |
| 5.A  |    14.3   |   Goedertier    |    Türme in die Hauptmap einfügen.   |       45 min.        |
| 6.A  |    7.3   |  Koch    |    Eine Startrunde programmieren.    |       45 min.        |
| 6.B  |    14.3   |   Koch   |    Weitere Runden erstellen.    |       45 min.        |
| 7.A  |    14.3   |    Gilardoni     |   Man bekommt Geld wenn Gegner sterben.  |       45 min.        |
| 8.A  |    7.3   |    Gilardoni     | Es gibt Gegener.  |       45 min.        |
| 8.B  |    14.3   |    Gilardoni     | Die Gegner kommen wenn die Runde beginnt.  |       45 min.        |
| 9.A  |    7.3   |    Goedertier    | Todes Menu erstellen.  |       45 min.        |
| 9.B  |    14.3   |    Goedertier    | Todes Menu kommt wenn man stirbt.  |       45 min.        |
| 10.A  |    7.3   |    Raviraj   | Ein Knopf einfügen mit dem man das Programm schliessen kann.  |       45 min.        | 
| 14.A  |   14.3   |   Raviraj  |  Man kann sich auf der Map frei bewegen. |       45 min.        |
| 11.A  |   14.3   |   Goedertier  |  Verschiedene Gegner Typen erstellen. |       45 min.        |
| 11.B  |   14.3   |   Goedertier  |  Verschiedene Gegner Typen in das Spiel einfügen. |       45 min.        |
| 12.A  |   14.3   |   Gilardoni  | Die Gegner ziehn unterschiedlich viel Leben abziehen . |       45 min.        |
| 13.A  |   14.3   |   Koch  |  Einen Knopf einfügen um die Türme zu verbessern. |       45 min.        |
| 13.B  |   14.3   |   Koch  |  Wenn man den Knopf drückt verbessern, verbessert sich die Türmen, so dass sie mehr Gegner töten können. |       45 min.        |
| 13.C  |   21.3   |   Koch  |  Wenn man auf den Knopf drückt verbessern, zieht es einen bestimmten Betrag an Gold ab. |       45 min.        |
| 15.A  |   14.3   |   Raviraj   |  Einen Timer erstellen, der sagt wann die Runde beginnt |       45 min.        |
| 17.A  |   21.3   |   Goedertier   | Neue Maps erstellen. |       45 min.        |
| 17.B  |   21.3   |   Gilardoni   | Neue Maps erstellen. |       45 min.        |
| 17.C  |   21.3   |   Raviraj   | Maps ins Spiel implementieren. |       45 min.        |
 17.D |   21.3   |   Raviraj   | Bei jeder neuen Runde gibt es eine neue Runde |       45 min.        |
|Total: ||||1260 min|



## 3 Entscheiden

Keine

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |  07.03     |     Koch      |         45     |      45             |
| 2.A  |   07.03    |    Koch       |         45      |     45              |
| 4.A  |   07.03    |    Koch       |         45      |     90             |
| 3.A  |   07.03    |    Gilardoni      |         45      |     45              |
| 3.B |   07.03    |    Gilardoni      |         45      |     45              |
| 11.A |   07.03    |    Gilardoni      |         45      |     90            |
| 16.A |   07.03    |     Goedertier     |         45      |     90       |
| 9.A |   07.03    |     Goedertier   |         45      |     90       |
| 11.A |   07.03    |     Goedertier   |         45      |     90       |
| 17.A |   07.03    |     Goedertier   |         45      |     90       |
| 4.B |   07.03    |     Gilardoni   |         45      |     180       |
| 4.A |   07.03    |     Koch  |         45      |     90     |
| 9.A |   07.03    |     Koch  |         45      |    90      |
| 10.A |   07.03    |     Raviraj    |         45      |     45      |
| 16.A |   07.03    |     Raviraj    |         45      |     90     |
| 9.B |   07.03    |     Koch    |         45      |     120   |
| 16.A |   07.03    |     Raviraj    |         45      |     120  |
| 4.B |   07.03    |      Gilardoni    |         45      |     120    |
| 17.A |   07.03    |     Goedertier   |         45      |     120    | 


## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 04.04.23 | Das Hauptmenü erscheint, wenn man das Programm startet. | Koch |



Unser Programm, wurde nicht fertig geschrieben, das heisst, dass wir nicht alles testen konnten. Aber von den Sachen, die wir hatten, hat das alles funktioniert.

## 6 Auswerten

https://github.com/TigerL06/LA1500/blob/main/Lernbericht.md
