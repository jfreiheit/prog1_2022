# Aufgaben

Hier finden Sie die Aufgaben. Die Abgabefristen der einzelnen Aufgaben stehen [hier](../#planung-vorlaufig-kann-sich-noch-andern). Beachten Sie die nachfolgenden Hinweise zum Hochladen der Aufgaben. 

## Hinweise zur Abgabe der Aufgaben

Die Aufgaben laden Sie in [Moodle](https://moodle.htw-berlin.de/course/view.php?id=29156) unter dem Reiter "Aufgaben" hoch. Dort ist für jede Aufgabe eine Moodle-Aufgabe erstellt. Beachten Sie, dass ein Hochladen nach Ablauf der Abgabefrist nicht mehr möglich ist. 


### Eclipse

Sie sind in der Wahl Ihrer Entwicklungsumgebung frei. Ich verwende in der Veranstaltung Eclipse. Dafür gelten die folgenden Hinweise: 

- Achten Sie darauf, dass Sie die Quelldateien (also die `.java`-Dateien aus dem `src`-Verzeichnis) hochladen. 
- Ihre Klassen erstellen Sie immer in einem package `aufgaben.aufgabeX`. Das heißt, Aufgabe1 ist im package `aufgaben.aufgabe1`, Aufgabe2 im package `aufgaben.aufgabe2` usw. 
- In Ihrem `workspace`gibt es dann einen Ordner für Ihr Java-Projekt, z.B. `WS22` (je nachdem, wie Sie Ihr Java-Projekt genannt haben) und darin befindet sich ein `bin`- und ein `src`-Ordner. In dem `src`-Ordner befindet sich dann ein Ordner `aufgaben` und darin ein Ordner `aufgaben1` (für Aufgabe1). Darin befindet sich Ihre `.java`-Datei, die Sie hochladen sollen. Angenommen, Sie haben Ihre Klasse `Aufgabe1` genannt, dann heißt die Klasse also `Aufgabe1.java`. Sie folgen also dem Pfad `workspace`--> *Java-Projekt* (z.B. `WS22`) --> `src` --> `aufgaben` --> `aufgabe`*X*.
- Wenn Ihre Lösung aus mehreren Klassen (mehreren `.java`-Dateien) besteht, können Sie entweder die Dateien einzeln hochladen oder Sie zippen Ihre Dateien (am besten dann den `aufgabeX`-Ordner und laden das `.zip`-File hoch. 
- In Ihrer Lösung (Ihrer/n Klasse/n) fügen Sie direkt oberhalb Ihrer Klassendefinition einen JavaDoc-Kommentar ein (`/** ... */`). Dieser enthält ein `@author`-Tag. dahinter schreiben Sie Ihren Namen. Das sieht dann z.B. so aus:
	```java
	package aufgaben.aufgabe1;

	/**
	 * 
	 * @author Jörn Freiheit
	 * 
	 * Diese Klasse gibt auf die Konsole ein Rhombus (eine Raute) aus.
	 * Der Rhombus ist entweder gefuellt oder ungefuellt. 
	 *
	 */
	public class Aufgabe1
	{
		// hier Ihre Implementierung
	}
	```
- Sie können Ihre Aufgaben zu zweit lösen. Tragen Sie dann hinter das `@author`-Tag beide Namen ein und **laden Sie bitte beide** die Lösung in Moodle hoch!

## Code Review

Für jede abgegebene Aufgabe wird Ihnen die Lösung einer Kommilitonin zum Review zugewiesen. Analysieren Sie den Code Ihrer Kommilitonin und geben Sie ihr dazu eine Rückmeldung!  Es genügen 2 bis 3 Review-Kommentare.
Zur offiziellen Abgabe einer Aufgabe gehören also

- das Hochladen der eigenen Lösung,
- das Analysieren/Kommentieren einer fremden Lösung.

#### Hinweise zum Review:

- Es geht nicht darum, das Programm zu überarbeiten, sondern darum es nachzuvollziehen und Ihrer Kommilitonin eine Rückmeldung und eventuell Anregungen zu geben.
- Weisen Sie sowohl auf Stärken als auch auf Schwächen des Quelltexts hin.
- Worauf Sie u.a. achten können:
	- Ist der Quelltext gut strukturiert und verständlich?
	- Haben Variablen und Methoden passende Namen? Werden die Namen konsistent verwendet?
	- Werden Konventionen eingehalten? Beispiel: Klassennamen starten immer mit Großbuchstaben, Objektnamen immer mit Kleinbuchstaben
	- Ist das Programm übersichtlich formatiert? Beispiel: kein horizontales Scrolling nötig
- Machen Sie ggf. Vorschläge für (alternative) Lösungen.
- Gehen Sie respektvoll miteinander um, es gibt keinen Grund, unhöflich zu sein.
- Lesen Sie Ihre Kommentare noch einmal durch, bevor Sie sie an Ihre Kommilitonin weitergeben.

![review](./files/12_review.png)

## Aufgaben

#### Aufgabe 1 (Abgabe bis 22.11.2022 24:00 Uhr)

??? "Aufgabe1 - Rhombus"
	- Erstellen Sie eine Klasse `Aufgabe1` mit `main()`-Methode im package `aufgaben.aufgabe1` 
	- Implementieren Sie eine Methode `public static void printRhombus(int upperHalf, boolean filled){}`
	- Ist der Parameterwert von `filled` `true`, dann soll ein Rhombus (eine Raute) wie folgt auf die Konsole ausgegeben werden:
		```bash
		      *
		     ***
		    *****
		   *******
		  *********
		 ***********
		  *********
		   *******
		    *****
		     ***
		      *
		```
	- Ist der Parameterwert von `filled` `false`, dann soll der Rhombus ungefüllt sein, also so:
		```bash
		      *
		     * *
		    *   *
		   *     *
		  *       *
		 *         *
		  *       *
		   *     *
		    *   *
		     * *
		      *
		```
	- der Wert für `upperHalf` gibt die Höhe einer Hälfte des Rhombus an. Die Gesamthöhe des Rhombus berechnet sich aus `
		```java
		int height = 2 * upperHalf +1;
		```
	- In unserem oben gezeigten Beispiel ist der Wert von `upperHalf` `5` und die Gesamthöhe des Rhombus `11`. 
	- Die obere Ausgabe ist also durch die Anweisung `printRhombus(5, true);` und die untere durch die Anweisung `printRhombus(5, false);` entstanden.
	- Die Berechnung der Höhe aus dem Parameterwert `upperHalf` hat die Vorteile, 
		- dass die Höhe dadurch immer eine ungerade Zahl ist (was notwendig ist) und 
		- dass Sie den Wert `upperHalf` gut verwenden können (was ebenfalls notwendig ist, wie Sie merken werden)
	- **Tipp:**: Schreiben Sie sich zwei weitere Methoden `public static void printRhombusFilled(int upperHalf){}` und `public static void printRhombusUnfilled(int upperHalf){}`, die Sie entsprechend des Wertes von `filled` aufrufen. In der einen Methode erstellen Sie die ausgefüllte Raute und in der anderen die ungefüllte. Dann wird Ihr Programm nicht zu unübersichtlich. Fangen Sie am besten mit der ausgefüllten an, die ist etwas leichter. 
	- Bedenken Sie auch, dass in jeder Zeile nicht nur eine bestimmte Anzahl Sterne ausgegeben werden muss, sondern erst noch eine bestimmte Anzahl Leerzeichen. Wieviele Leerzeichen sind es in Zeile `x` bei einem gegebenen Wert für `upperHalf`? Wieviele Sterne sind es in Zeile `x` bei einem gegebenen Wert für `upperHalf`? Sie sollten diese Fragen zunächst mithilfe von Zettel und Stift beantworten ehe Sie mit dem Programmieren beginnen. Zettel und Stift sind die wichtigsten Hilfsmittel einer Programmiererin!
	- Das Programm soll für beliebige (nicht so große - max. Wert `100`) positive Zahlen (also `> 0`) von `upperHalf` funktionieren. Insbesondere sind die Tests für `upperhalf == 1` interssant. 
	- Laden Sie Ihre Lösung bis Dienstag, den **22.11.2022 um 24.00 Uhr** in Moodle hoch
	- Viel Spaß und viel Erfolg!


#### Aufgabe 2 (Abgabe bis 29.11.2022 24:00 Uhr)

??? "Aufgabe2 - Numbers"
	- Erstellen Sie eine Klasse `Aufgabe2` mit `main()`-Methode im package `aufgaben.aufgabe2`.
	- Bei der Lösung der Aufgabe soll nicht der Datentyp `String` verwendet werden! 
	- Implementieren Sie eine Methode `public static int lengthOfNumber(int number){}`. Diese Methode gibt die Länge von `number` zurück, d.h. die Anzahl der Ziffern in der Zahl. **Beachten Sie**: für `number == 0` soll jedoch `0` zurückgegeben werden. <br/>
		**Beispiele:** <br/>
			```
			number  --> Rückgabewert
			0 		--> 0
			1 		--> 1
			9 		--> 1
			10 	    --> 2
			1234    --> 4
			-1234   --> 4
			```

	- Implementieren Sie eine Methode `public static int firstDigit(int number){}`. Diese Methode gibt die erste Ziffer von `number` zurück.  <br/>
		**Beispiele:** <br/>
			```
			number  --> Rückgabewert
			0 		--> 0
			1 		--> 1
			9 		--> 9
			10 	    --> 1
			1234    --> 1
			-1234   --> 1
			5678    --> 5
			```

	- Implementieren Sie eine Methode `public static int powerOf10ToN(int n){}`. Diese Methode gibt den Wert für `10 ^ n` zurück. Sie können davon ausgehen, dass `n >= 0` gilt.  <br/>
		**Beispiele:** <br/>
			```
			n       --> Rückgabewert
			0 		--> 1
			1 		--> 10
			2 		--> 100
			3 	    --> 1000
			4       --> 10000
			```

	- Implementieren Sie eine Methode `public static int cutFirstDigit(int number){}`. Diese Methode entfernt von `number` die erste Ziffer.  Für `-10 < number < 10` wird `0` zurückgegeben. <br/>
		**Beispiele:** <br/>
			```
			number  --> Rückgabewert
			0 		--> 0
			1 		--> 0
			9 		--> 0
			-9 	    --> 0
			11      --> 1
			91      --> 1
			1234    --> 234
			-1234   --> -234
			9999    --> 999
			-9999   --> -999
			1023    --> 23  // Achtung! führende Nullen in der verbleibenden Zahl entfallen
			```

	- Implementieren Sie eine Methode `public static boolean secondDigitIsZero(int number){}`. Diese Methode gibt ein `true` zurück, wenn die zweite Ziffer in `number` eine `0` ist. Sonst `false`. <br/>
		**Beispiele:** <br/>
			```
			number  --> Rückgabewert
			0 		--> false
			1 		--> false
			9 		--> false
			11 	    --> false
			101     --> true
			111     --> false
			1001    --> true
			-10234  --> true
			1111    --> false
			10000   --> true
			```

	- Testen Sie alle Methoden ausführlich in der `main()`-Methode.
	
	- Laden Sie Ihre Lösung bis Dienstag, den **29.11.2022 um 24.00 Uhr** in Moodle hoch
	- Viel Spaß und viel Erfolg!

