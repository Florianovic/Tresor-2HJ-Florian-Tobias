# Tresor-2HJ-Florian-Tobias

## Über das Projekt:
Wir haben uns für dieses Halbjahr dazu entschieden einen Tresor zum sicheren Aufbewahren von Gegenständen zu bauen, welcher mit einem Code, der über ein Tastenfeld eingegeben wird, geöffnet weren kann. Als Schließmechanismus soll ein Servomotor dienen, welcher verhindert, dass die Tür geöffnet wird wenn ein falscher Code eingegeben wurde. </br>
Es folgt eine Komponentenliste und eine Anleitung zum Code für unser Projekt.

### Inhaltsverzeihnis
<ul>
  <li><a href="#komponenten">Komponentenliste</a></li>
  <li><a href="#keypad">Funktionsweise Keypad</a></li>
  <li><a href="#code">Der Code</a></li>
  <li><a href="#endprodukt">Das Endprodukt</a></li>
  <li><a href="#probleme">Probleme während dem Projekt</a></li>
  <li><a href="#fazit">Fazit</a></li>
  <li><a href="#quellen">Quellen</a></li>
 </ul>
  
  
<h2 id="komponenten">Komponentenliste</h2>
<ul>
  <li>Arduino Uno</li>
  <li>Servo</li>
  <li>Gehäuse</li>
  <li>Einige Jumper-Kabel</li>
  <li>Keypad</li>
  <li>Stromversorgung</li>
 </ul>
  
  
<h2 id="keypad">Das Keypad</h2>
Das Keypad ist eine Komponente mit der man einen Zahlen- bzw. Buchstaben-Code eingeben kann, welcher beispielsweise ein Signal zur Aktivierung eines Servos verursacht. 
Es ist aufgeteilt in vier waagerechte Zeilen und vier senkrechte Spalten. Jede Zeile bzw. Spalte ist mit je einem Pin des Arduinos belegt, so dass für die 16 Tasten nur acht Pins benutzt werden müssen. Dabei werden vier Pins als Eingänge und vier Pins als Ausgänge des Arduinos festgelegt. Durch das Drücken einer beliebigen Taste werden nun Zeile und Spalte dieser Taste verbunden und somit auch Eingang und Ausgang des Arduinos. Eine Spannung wird gemessen und durch die Zuordnung der Pins auf die Spalten und Zeilen lässt sich jede gedrückte Taste genau bestimmen.


<h2 id="code">Der Code<h2>
  
  ![Code Teil1](https://raw.githubusercontent.com/Florianovic/Tresor-2HJ-Florian-Tobias/master/Keypad%20Teil%201.JPG)
  ![Code Teil2](https://raw.githubusercontent.com/Florianovic/Tresor-2HJ-Florian-Tobias/master/Keypad%20Teil%202.JPG)


<h2 id="endprodukt">Das Endprodukt</h2>
<p align="center"><a href="https://youtu.be/mYkLfzecf9w"><img src="https://github.com/Florianovic/Tresor-2HJ-Florian-Tobias/blob/master/S1190001.JPG" width="400px"><br>Link zum Video</a></p>


<h2 id="probleme">Probleme wärend dem Projekt</h2>
Bis zum Ende hatten wir gehofft zusätzlich ein LCD Monitor einzubauen, welcher die auf dem Keypad eingegebenen Zahlen anzeigt und angiebt, ob der eingegebene Code korrekt oder falsch ist. Leider ist uns dies bis zum Schluss trotz stundenlangem Probieren nicht gelungen. Zu erst haben wir den Fehler in den Komponenten gesucht, haben Kabel ausgetauscht und verschiedene Typen von Arduino verwendet (Uno und Mega) und haben uns als sich dies als erfolglos erwies mehrfach mit Mitschülern in Verbindung gesetzt und diese, neben eigenen Recherchen, nach Tipps wie wir den Monitor zum Laufen bringen könnten befragt. Selbst nachdem wir einen Code vollständig übernommen und alle Bibliotheken genau so installiert hatten wie angegeben, funktionierte der Monitor immer noch nicht. Desshalb haben wir uns schweren Herzens dazu entscheiden müssen den LCD-Monitor aus dem Projekt zu streichen. Wir wissen leider immer noch nicht was der Fehler war und wieso der Monitor nicht funktioniert hat. <br>
Es folgt der Code, bei welchem der Monitor das erste mal bei <a href="https://github.com/dennis602/Stundenprotokoll-II#30">Dennis und Peter</a> funktioniert hatte, bei uns jedoch nicht:


![LCD-Test](https://github.com/Florianovic/Tresor-2HJ-Florian-Tobias/blob/master/LCD-Test.PNG)

Bei uns wurde, andes als bei Dennis und Peter, nur ein beleuchteter Hintergrund angezeigt.</br>
Des weiteren funktionierte der Arduino nur während er an einen Computer angeschlossen war und nicht mit einer Batterie, weshalb wir darauf verzichten mussten den Arduino in der Box einzubauen sondern ihn neben der Kiste zu platzieren mussten um eine Verbindung herstellen zu können.

<h2 id="fazit">Unser Fazit</h2>
Leider haben wir all unsere Energie bis zum Ende darein gesteckt den Monitor, welcher nunmal das komplexeste Bauteil des Projektes war, zum Laufen zu bringen, sodass im Endeffekt nur ein Projekt von geringem Umfang entstehen konnte. Außerdem erschwerte uns das Probllem der Batterie die Arbeit, sodass nicht einmal eine seperate Kiste entstehen konnte. Des Weiteren kam noch der Problemfaktor 'Corona' hinzu, welcher sowohl die Kommunikation, als auch das gemeinsame Arbeiten am Projekt deutlich erschwerte. Im Endeffekt konnten wir deutlich weniger erreichen als wir uns vorgenommen hatten.

<h2 id="quellen">Quellen</h2>

https://www.makerblog.at/2018/11/4x4-keypad-am-arduino-servoschloss-mit-pincode-selbst-basteln-tutorial/
