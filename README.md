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
  <li><a href="#lcd">Das Problem mit dem LCD</a></li>
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



<h2 id="lcd">Das Problem mit dem LCD</h2>
Bis zum Ende hatten wir gehofft zusätzlich ein LCD Monitor einzubauen, welcher die auf dem Keypad eingegebenen Zahlen anzeigt und anzeigt, ob der eingegebene Code korrekt oder falsch ist. Leider ist uns dies bis zum Schluss trotz stundenlangem Probieren nicht gelungen. Zu erst haben wir den Fehler in den Komponenten gesucht, haben Kabel ausgetauscht und verschiedene Typen von Arduino verwendet (Uno und Mega) und haben uns al sich dies als erfolglos erwies mehrfach mit Mitschülern in Verbindung gesetzt und diese, neben eigenen Recherchen, nach Tipps wie wir den Monitor zum Laufen bringen könnten befragt. Selbst nachdem wir einen Code vollständig übernommen und alle Bibliotheken genau so installiert hatten wie angegeben, funktionierte der Monitor immer noch nicht. Desshalb haben wir uns schweren Herzens nach mehreren Stunden dazu entscheiden müssen den LCD-Monitor aus dem Projekt zu streichen. Wir wissen leider immer noch nicht was der Fehler war und wieso der Monitor nicht funktioniert hat, aber um unseren Zeitplan einhalten zu können gab es für uns keine andere Option. </br>
Es folgt der Code, bei welchem der Monitor das erste mal bei <a href="https://github.com/dennis602/Stundenprotokoll-II#30">Dennis und Peter</a> funktioniert hatte:


![LCD-Test](https://github.com/Florianovic/Tresor-2HJ-Florian-Tobias/blob/master/LCD-Test.PNG)


<h2 id="quellen">Quellen</h2>
