# Tresor-2HJ-Florian-Tobias

## Über das Projekt:
Wir haben uns für dieses Halbjahr dazu entschieden einen Tresor zu aufbewahren von Gegenständen zu bauen, welcher mit einem Code, welcher über ein Tastenfeld eingegeben wird, geöffnet weren kann. Als Schließmechanismus soll ein Servomotor dienen, welcher verhindert, dass die Tür geöffnet wird wenn ein falscher Code eingegeben wurde. </br>
Es folgt eine Komponentenliste und eine Anleitung zum Code für unser Projekt.

### Inhaltsverzeihnis
<ul>
  <li>Komponentenliste</li>
  <li>Funktionsweise Keypad</li>
  <li>Der Code</li>
  <li>Das Endprodukt</li>
  <li>Das Problem mit dem LCD</li>
 </ul>
  
### Komponentenliste
<ul>
  <li>Arduino Uno</li>
  <li>Servo</li>
  <li>Gehäuse</li>
  <li>Einige Jumper-Kabel</li>
  <li>Keypad</li>
 </ul>
  
  
### Keypad:
Das Keypad ist eine Komponente mit der man einen Zahlen- bzw. Buchstaben-Code eingeben kann, welcher beispielsweise ein Signal zur Aktivierung eines Servos verursacht. 
Es ist aufgeteilt in vier waagerechte Zeilen und vier senkrechte Spalten. Jede Zeile bzw. Spalte ist mit je einem Pin des Arduinos belegt, so dass für die 16 Tasten nur acht Pins benutzt werden müssen. Dabei werden vier Pins als Eingänge und vier Pins als Ausgänge des Arduinos festgelegt. Durch das Drücken einer beliebigen Taste werden nun Zeile und Spalte dieser Taste verbunden und somit auch Eingang und Ausgang des Arduinos. Eine Spannung wird gemessen und durch die Zuordnung der Pins auf die Spalten und Zeilen lässt sich jede gedrückte Taste genau bestimmen.
