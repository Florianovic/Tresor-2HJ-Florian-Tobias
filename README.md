# Tresor-2HJ-Florian-Tobias



### Keypad:
Das Keypad ist eine Komponente mit der man einen Zahlen- bzw. Buchstaben-Code eingeben kann, welcher beispielsweise ein Signal zur Aktivierung eines Servos verursacht. 
Es ist aufgeteilt in vier waagerechte Zeilen und vier senkrechte Spalten. Jede Zeile bzw. Spalte ist mit je einem Pin des Arduinos belegt, so dass für die 16 Tasten nur acht Pins benutzt werden müssen. Dabei werden vier Pins als Eingänge und vier Pins als Ausgänge des Arduinos festgelegt. Durch das Drücken einer beliebigen Taste werden nun Zeile und Spalte dieser Taste verbunden und somit auch Eingang und Ausgang des Arduinos. Eine Spannung wird gemessen und durch die Zuordnung der Pins auf die Spalten und Zeilen lässt sich jede gedrückte Taste genau bestimmen.
