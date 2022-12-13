# Übungen

## Übungsblätter (wochenweise)


??? note "Übung 0"
	1. Installieren Sie sich - falls noch nicht geschehen - eine Java-Entwicklungsumgebung (siehe [**Java**](../tools/#java)).
	2. Installieren Sie sich die IDE Ihrer Wahl (siehe [**IDE**](../tools/#ide)). In den Vorlesungen und Übungen verwende ich [**Eclipse**](../tools/#eclipse) und beschreibe die Schritte auch für Eclipse.
	3. Starten Sie Eclipse durch Doppelklick auf das Programmsymbol.
	4. Erstellen Sie einen *Workspace* (Arbeitsbereich) in einem gewünschten Ordner (z. B.
	`Prog12`) im Dateisystem. Achten Sie darauf, dass Sie Schreibrechte in diesem Ordner besitzen.
	5. Anlegen eines Projektordners:
		* Auswahl im Menü `File-->New-->Java Project`.
		* Eingabe des `Project name:` Name des Projektes (z.B. `WiSe22`). Klicken auf den Button `Finish`.
		* Das Fenster `New module-info.java` können Sie einfach mit `Create` bestätigen.
	4. Erstellen eines neuen Packages (Paketes):
		* Öffnen der Projektmappe im `Package Explorer`.
		* Auswahl des Ordners `src` mit der rechten Maustaste.
		* Auswahl des Menüpunktes `New --> Package`.
		* Geben Sie folgenden Paketnamen ein (Paketnamen werden kleingeschrieben) `uebungen.uebung0` (Achten Sie auf den Punkt und dass Sie alles zusammen schreiben).
	5. Erstellen einer neuen Klasse:
		* Öffnen der Projektmappe im Package Explorer.
		* Auswahl des Paketes (`uebungen.uebung0`) mit der rechten Maustaste.
		* Auswahl des Menüpunktes `New --> Class`.
		* Eingabe des Namens, der gleichzeitig der Klassen- und Dateiname ist: `Uebung0`. Klassennamen werden immer groß geschrieben.
		* Setzen des Häkchens bei `public static void main()`. (Sollten Sie vergessen haben, das Häkchen zu setzen, dann ist die Klasse, nachdem Sie `Finish` gedrückt haben, leer. Setzen Sie dann den Cursor zwischen die beiden geschweiften Klammern `{ }`, geben dann `main` ein und drücken die <kbd class="key-ctrl">Ctrl</kbd><span>+</span><kbd class="key-space">Leer</kbd>-Tasten und anschließend <kbd class="key-enter">Enter</kbd>. Dann erscheint die `main()`-Methode)
		* Klicken auf den Button `Finish`.
	6. In die `main()`-Methode (zwischen die geschweiften Klammern `{` und `}` geben 	Sie ein: `System.out.println("Uebung 0"));`.
	7. Drücken Sie dann entweder auf den ![run](./files/16_run.png)-Button oder 		wählen Sie aus dem Menü `Run --> Run` oder drücken Sie <kbd class="key-shift">shift</kbd><span>+</span><kbd class="key-command">command</kbd>+</span><kbd class="key-f11">f11</kbd>. In der `Console` in Ihrer IDE (in Eclipse unten) erscheint `Uebung 0`. 

	=== "Uebung0.java"
		```java
		package uebungen.uebung0;

		public class Uebung0
		{
			public static void main(String[] args)
			{
				System.out.println("Uebung 0");
			}
		}
		```

	![uebung0](./files/17_uebung0.png)

	!!! success
		Fertig! Ihre Entwicklungsumgebung ist bereit! Wir können loslegen. :thumbsup:


??? note "Übung 1"
	1. Erstellen Sie ein package `uebungen.uebung1`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung1` mit `main()`-Methode.
	3. Deklarieren und initialisieren Sie in der `main()`-Methode jeweils eine Variable mit dem Datentyp `int`, `long`, `char`, `byte`, `short`, `float`, `double`, `boolean` und `String`. Geben Sie alle Werte einzeln durch Aufruf der `println()`-Methode aus. Erzeugen Sie dabei folgende Ausgabe (Werte nur Beispiele):
	```bash
	Wert vom Typ int 		: 	123
	Wert vom Typ long 		: 	456789
	Wert vom Typ char 		: 	a
	Wert vom Typ byte 		: 	127
	Wert vom Typ short 		: 	32767
	Wert vom Typ float 		: 	4.23
	Wert vom Typ double		: 	6.98
	Wert vom Typ boolean	: 	true
	Wert vom Typ String		: 	Hallo!
	```
	4. Setzen Sie den Wert Ihrer `int`-Variablen auf `2147483647`. Geben Sie den Wert auf der Konsole aus, z.B.:	
	```bash
	Wert von i 	: 	2147483647
	```
	Erhöhen Sie nun den Wert der Variablen um `1` und geben Sie den Wert erneut aus. Was passiert? Warum?
	5. Wiederholen Sie das gleiche mit einer `long`-Variablen.
	6. Weisen Sie Ihrer `char`-Variablen den Wert `65` zu. Geben Sie den Wert Ihrer `char`-Variablen aus. Was passiert? Warum?
	7. Gegeben ist die folgende Klasse:
			
		```java
		public class PrinterClass 
		{

			public static void main(String[] args) 
			{
				System.out.print("answer=");
				System.out.println(40 + 2);
			}
		}
		```

		Was wird auf der Konsole ausgegeben?<br/>
		<b>a)</b> 
		```
		answer=42
		```
		<b>b)</b> 
		```
		answer=
		42
		```
		<b>c)</b> 
		```
		answer
		=
		42
		```
	8. Betrachten Sie folgenden Pseudocode:
			
		```
		cake prices are 1.0 and 2.0
		for each item
			if cake price is even
				print "even"
			else
				print "uneven"
		```		

		Welche Bedeutungen haben die Einrückungen? Was wird ausgegeben? <br/>
		<b>a)</b> 
		```
		even
		```
		<b>b)</b> 
		```
		uneven
		```
		<b>c)</b> 
		```
		even, uneven
		```
		<b>d)</b> 
		```
		uneven, even
		```
	9. Betrachten Sie folgenden Pseudocode:
			
		```
		n = 3
		while n > 1
			print n
			n = n – 1
		```		

		Welche Bedeutungen haben die Einrückungen? Was wird ausgegeben? <br/>
		<b>a)</b> 
		```
		3
		```
		<b>b)</b> 
		```
		3,2
		```
		<b>c)</b> 
		```
		3,2,1
		```
	10. Führen Sie folgende Übungen mit 8 Stellen durch:

		1. Rechnen Sie `126` in eine Binärzahl um.
	2. Rechnen Sie `-126` in eine Binärzahl um.
	3. Addieren Sie `00001010` und `00001100`. 
	4. Subtrahieren Sie `00001010` und `00001100`. 


??? question "Eine mögliche Lösung für Übung1"
	```java
	package uebungen.uebung1;

	public class Uebung1
	{
		public static void main(String[] args)
		{
			int in = 123;
			long lo = 456789;
			char ch = 'a';
			byte by = 127;
			short sh = 32767;
			float fl = 4.23f;
			double d1 = 6.98;
			boolean b1 = true;
			String s1 = "Hallo!";
			
			System.out.println(" --- Aufgabe 3 -------");
			System.out.println();
			System.out.println("Wert vom Typ int     : " + in );
			System.out.println("Wert vom Typ long    : " + lo );
			System.out.println("Wert vom Typ char    : " + ch );
			System.out.println("Wert vom Typ byte    : " + by );
			System.out.println("Wert vom Typ short   : " + sh );
			System.out.println("Wert vom Typ float   : " + fl );
			System.out.println("Wert vom Typ double  : " + d1 );
			System.out.println("Wert vom Typ boolean : " + b1 );
			System.out.println("Wert vom Typ String  : " + s1 );
			
			System.out.println();
			System.out.println(" --- Aufgabe 4 -------");
			System.out.println();
			in = 2147483647;
			System.out.println("Wert vom Typ int     : " + in );
			in = in + 1;		// in++;
			System.out.println("Wert vom Typ int     : " + in );
			
			System.out.println();
			System.out.println(" --- Aufgabe 5 -------");
			System.out.println();
			lo = 2147483647L;	// L am Ende des Wertes beachten
			System.out.println("Wert vom Typ long    : " + lo );
			lo = lo +1 ;
			System.out.println("Wert vom Typ long    : " + lo );
			
			System.out.println();
			System.out.println(" --- Aufgabe 6 -------");
			System.out.println();
			ch = 65;
			System.out.println("Wert vom Typ char    : " + ch );
			
			// 7 a)
			// 8 d)
			// 9 b)
			//  126 --> 0111 1110
			// -126 --> 1000 0010
			// 0000 1010 + 0000 1100 = 0001 0110  ( 10 + 12 = 22 )
			// 0000 1010 - 0000 1100 = 0000 1010 + 1111 0100 = 1111 1110 ( 10 - 12 = -2 )			
		}

	}
	```



??? note "Übung 2"
	
	1. Erstellen Sie ein package `uebungen.uebung2`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung2` mit `main()`-Methode.
	3. Schreiben Sie eine Methode 
	```java
	public static void printIntDivision(int nr1, int nr2) 
	{
	}
	``` 
	Diese Methode soll folgende Ausgabe auf die Konsole erzeugen,
	z.B. für `printIntDivision(7, 4);` die Ausgabe 
	```bash
	7 geteilt durch 4 ergibt 1. Es bleibt ein Rest von 3
	```
	z.B. für `printIntDivision(17, 4);` die Ausgabe
	```bash 
	17 geteilt durch 4 ergibt 4. Es bleibt ein Rest von 1
	```
	
		Rufen Sie die Methode entsprechend in der `main()`-Methode auf!

	5. Schreiben Sie zwei Methoden 
	```java
	public static int getQuotient(int nr1, int nr2) {} // und 
	public static int getRemainder(int nr1, int nr2) {}
	``` 
	Deklarieren Sie in der main()-Methode zwei int-Variablen und weisen Sie diesen Werte zu (z.B. `17` und `4`). Wenden Sie die beiden Methoden so an, dass mit Hilfe der `println()`-Methode folgende Ausgaben erscheinen: 
	```bash 
	17/4 = 4
	17 mod 4 = 1
	```
	6. Besitzen die folgende Methodenaufrufe einem Wert? Wenn ja, welcher?

		- `printIntDivision(17, 4);`
	- `getQuotient(17,4);`
	- `getRemainder(17,4);`

	7. Können wir die Methoden `getQuotient(int nr1, int nr2)` und `getRemainder(int nr1, int nr2)` auch in der `printIntDivision(int nr1, int nr2)`-Methode verwenden/aufrufen? Wenn ja, wie?


??? question "Eine mögliche Lösung für Übung 2"
	```java 
	package uebungen.uebung2;

	public class Uebung2
	{

		public static void printIntDivision(int nr1, int nr2)
		{
			//int quotient = nr1 / nr2;				
			int quotient = getQuotient(nr1, nr2);
			//int remainder = nr1 % nr2;
			int remainder = getRemainder(nr1, nr2);
			System.out.println(nr1 + " geteilt "
					+ "durch " + nr2 
					+ " ergibt " + quotient + ". "
					+ "Es bleibt ein Rest "
					+ "von " + remainder);
		}
		
		public static int getQuotient(int nr1, int nr2) 
		{
			int quotient = nr1 / nr2;
			return quotient;		
		} 
		
		public static int getRemainder(int nr1, int nr2) 
		{
			int remainder = nr1 % nr2;
			return remainder;
		}
		
		public static void main(String[] args)
		{
			printIntDivision(7,4);
			printIntDivision(17,4);
			
			int number1 = 17;
			int number2 = 4;
			int result = getQuotient(number1, number2);
			int rest = getRemainder(number1, number2);
			
			System.out.println(number1 + "/" 
							+ number2 + " = " 
							+ result);
			
			System.out.println(number1 + " mod " 
					+ number2 + " = " 
					+ rest);
		}

	}

	```


??? note "Übung 3"
	
	1. Erstellen Sie ein package `uebungen.uebung3`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung3` mit `main()`-Methode.
	3. Schreiben Sie eine Methode `public static void printTimesTables(int nr1, int nr2)`. Bei Aufruf der Methode z.B. für `printTimesTables(10,10);` soll das kleine Ein-Mal-Eins in der folgenden Form ausgegeben werden:

		??? "Ausgabe für printTimesTables(10,10);"
			```bash 
			1 * 1 = 1
			1 * 2 = 2
			1 * 3 = 3
			1 * 4 = 4
			1 * 5 = 5
			1 * 6 = 6
			1 * 7 = 7
			1 * 8 = 8
			1 * 9 = 9
			1 * 10 = 10

			2 * 1 = 2
			2 * 2 = 4
			2 * 3 = 6
			2 * 4 = 8
			2 * 5 = 10
			2 * 6 = 12
			2 * 7 = 14
			2 * 8 = 16
			2 * 9 = 18
			2 * 10 = 20

			3 * 1 = 3
			3 * 2 = 6
			3 * 3 = 9
			3 * 4 = 12
			3 * 5 = 15
			3 * 6 = 18
			3 * 7 = 21
			3 * 8 = 24
			3 * 9 = 27
			3 * 10 = 30

			4 * 1 = 4
			4 * 2 = 8
			4 * 3 = 12
			4 * 4 = 16
			4 * 5 = 20
			4 * 6 = 24
			4 * 7 = 28
			4 * 8 = 32
			4 * 9 = 36
			4 * 10 = 40

			5 * 1 = 5
			5 * 2 = 10
			5 * 3 = 15
			5 * 4 = 20
			5 * 5 = 25
			5 * 6 = 30
			5 * 7 = 35
			5 * 8 = 40
			5 * 9 = 45
			5 * 10 = 50

			6 * 1 = 6
			6 * 2 = 12
			6 * 3 = 18
			6 * 4 = 24
			6 * 5 = 30
			6 * 6 = 36
			6 * 7 = 42
			6 * 8 = 48
			6 * 9 = 54
			6 * 10 = 60

			7 * 1 = 7
			7 * 2 = 14
			7 * 3 = 21
			7 * 4 = 28
			7 * 5 = 35
			7 * 6 = 42
			7 * 7 = 49
			7 * 8 = 56
			7 * 9 = 63
			7 * 10 = 70

			8 * 1 = 8
			8 * 2 = 16
			8 * 3 = 24
			8 * 4 = 32
			8 * 5 = 40
			8 * 6 = 48
			8 * 7 = 56
			8 * 8 = 64
			8 * 9 = 72
			8 * 10 = 80

			9 * 1 = 9
			9 * 2 = 18
			9 * 3 = 27
			9 * 4 = 36
			9 * 5 = 45
			9 * 6 = 54
			9 * 7 = 63
			9 * 8 = 72
			9 * 9 = 81
			9 * 10 = 90

			10 * 1 = 10
			10 * 2 = 20
			10 * 3 = 30
			10 * 4 = 40
			10 * 5 = 50
			10 * 6 = 60
			10 * 7 = 70
			10 * 8 = 80
			10 * 9 = 90
			10 * 10 = 100
			```

	4. Schreiben Sie eine Methode `public static void printTimesMatrix(int nr1, int nr2)`. Bei Aufruf der Methode z.B. für printTimesMatrix(10,10) soll das kleine Ein-Mal-Eins in der folgenden Form ausgegeben werden:

		??? "Ausgabe für printTimesMatrix(10,10);"
			```bash
			 1  2  3  4  5  6  7  8  9  10 
			 2  4  6  8  10  12  14  16  18  20 
			 3  6  9  12  15  18  21  24  27  30 
			 4  8  12  16  20  24  28  32  36  40 
			 5  10  15  20  25  30  35  40  45  50 
			 6  12  18  24  30  36  42  48  54  60 
			 7  14  21  28  35  42  49  56  63  70 
			 8  16  24  32  40  48  56  64  72  80 
			 9  18  27  36  45  54  63  72  81  90 
			 10  20  30  40  50  60  70  80  90  100 
			```

	5. Schreiben Sie eine Methode `public static void printTriangleUp(int height)`. Bei Aufruf der Methode z.B. für `printTriangleUp(7)` soll folgende Ausgabe erscheinen:
		```bash
		*******
		******
		*****
		****
		***
		**
		*
		```

	6. Geben Sie alle möglichen Kombinationen für 3 ganze Zahlen `x`, `y` und `z` aus, für die gilt:
		```java
		x <= y <= z und
		x * y * z = 36
		```

		---
		
		<b><i>Genügt bis hierher. Ab hier Zusatz nur für diejenigen, die bereits früher fertig sind.</i></b>

		---

	- <b>Zusatz</b> Schreiben Sie eine Umrechnung für eine gegebene Anzahl von Sekunden (`printSeconds(int seconds)`), z.B. `printSeconds(3456789)`:
		```bash
		3456789 Sekunden sind 40 Tage, 13 Minuten, 9 Sekunden.
		```
		Aber z.B. `printSeconds(2345678)`:
		```bash
		2345678 Sekunden sind 27 Tage, 3 Stunden, 34 Minuten, 38 Sekunden.
		```
		Aber z.B. `printSeconds(123456)`:
		```bash
		123456 Sekunden sind 1 Tag, 10 Stunden, 17 Minuten, 36 Sekunden.
		```
		Aber z.B. `printSeconds(12345)`:
		```bash
		12345 Sekunden sind 3 Stunden, 25 Minuten, 45 Sekunden.
		```
	- <b>Zusatz</b> Schreiben Sie eine Methode, die für eine natürliche Zahl deren Quersumme ausgibt, z.B.: `crossSum(12345678)`
		```bash
		Die Quersumme von 12345678 ist 36.
		```


??? question "Eine mögliche Lösung für Übung 3"
	```java 
	package uebungen.uebung3;

	public class Uebung3
	{

		public static void printTimesTables(int nr1, int nr2)
		{
			for (int i = 1; i <= nr1; i++)
			{
				for(int j = 1; j <= nr2; j++)
				{
					// System.out.println(" i = " + i + ", j = " + j);
					int product = i * j;
					System.out.println(i + " * " + j + " = " + product);
				}
				System.out.println();
			}
		}

		public static void printTimesMatrix(int nr1, int nr2)
		{
			for (int i = 1; i <= nr1; i++)
			{
				for(int j = 1; j <= nr2; j++)
				{
					System.out.print(" i = " + i + ", j = " + j + " ");
					int product = i * j;
					System.out.print(product + " ");
				}
				System.out.println();
			}
		}

		public static void printTriangleUp(int height)
		{
			for(int row = 0; row < height; row++)
			{
				// System.out.print("Zeile " + row + " : ");

				for(int nrOfStars = 0; nrOfStars < (height - row); nrOfStars++)
				{
					// System.out.print(nrOfStars + " ");
					System.out.print("* ");
				}

				// System.out.println("  <- Ende Zeile " + row);
				System.out.println();
			}
		}

		public static void printXYZ()
		{
			for(int x = -36; x <= 36; x++)
			{
				for(int y = x; y <= 36; y++)
				{
					for(int z = y; z <= 36; z++)
					{
						if(x * y * z == 36)
						{
							System.out.println("x=" + x + ", y=" + y + ", z= " + z);
						}
					}
				}
			}
		}

		public static void main(String[] args)
		{
			System.out.println();
			System.out.println("---------------- Aufgabe 3 --------------");
			System.out.println();
			printTimesTables(10,10);

			System.out.println();
			System.out.println("---------------- Aufgabe 4 --------------");
			System.out.println();
			printTimesMatrix(10,10);

			System.out.println();
			System.out.println("---------------- Aufgabe 5 --------------");
			System.out.println();
			printTriangleUp(7);


			System.out.println();
			System.out.println("---------------- Aufgabe 6 --------------");
			System.out.println();
			printXYZ();
		}

	}

	```

	
??? note "Übung 4"
	
	1. Erstellen Sie ein package `uebungen.uebung4`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung4` mit `main()`-Methode.
	3. Implementieren Sie folgende Methoden: 
		- `public static int inputInt()` – in dieser Methode wird über die Konsole eine `int`-Zahl eingelesen. Diese Zahl wird von der Methode zurückgegeben. Zur Eingabe von Zahlen über die Konsole siehe Klasse [Scanner](../hilfsklassen/#die-klasse-scanner).
		- `public static boolean isPrime(int number)` – diese Methode prüft, ob die als Parameter übergebene `number` eine Primzahl ist. Die Methode gibt ein `true` zurück, wenn `number` eine Primzahl ist und `false` sonst.
		- `public static void printPrimeNumbers(int maximum)` – diese Methode gibt alle Primzahlen von 1 bis einschließlich `maximum` wie folgt auf der Konsole aus (Bsp. für `maximum=61`):
			```bash
			Zahl : 61
			.2 3 .5 .7 ...11 .13 ...17 .19 ...23 .....29 .31 .....37 ...41 .43 ...47 .....53 .....59 .61
			```
			d.h. es werden die Zahlen, die Primzahlen sind, ausgegeben und für die anderen Zahlen erscheint nur ein Punkt. Verwenden Sie in der Methode `printPrimenumbers(int)` die Methode `isPrime(int)`.
		- `public static int getSmallestDivider(int number)` – diese Methode gibt den kleinsten Teiler zurück, der `number` ganzzahlig teilt. Ist `number` eine Primzahl, wird `number` zurückgegeben. Für den Fall, dass `number` kleiner als `2` ist, geben Sie ebenfalls `number` zurück.
		- `public static String createStringOfPrimeFactorization(int number)` – diese Methode gibt einen String in folgender Form zurück (Bsp. für `number=632060`):
			```bash
			" 2 * 2 * 5 * 11 * 13 * 13 * 17 = 632060 "
			```
			d.h. alle kleinsten Teiler werden mit dem Multiplikationszeichen verbunden und am Ende erscheint `= Wert von number`. 
		- Testen Sie alle Methoden. Rufen Sie insbesondere `inputInt()`, `printPrimenumbers(int)` und `createStringOfPrimeFactorization(int)` in der `main()`-Methode auf.
	4. **Tipp:** Bei der Überprüfung, ob `number` eine Primzahl ist, genügt es, Teiler bis zur Wurzel von `number` zu suchen. Werden bis dahin keine Teiler gefunden, ist `number` eine Primzahl. Sie können sich dazu z.B. eine Variable der Form 
	`int bound = (int) Math.sqrt(number);` erstellen und müssen dann den Teiler nur bis `bound` suchen (der Typkonvertierungsoperator `(int)` macht aus der `double`-Zahl einen `int` - schneidet die Nachkommastellen ab).


??? question "Eine mögliche Lösung für Übung 4"
	```java 
	package uebungen.uebung4;

	import java.util.Scanner;

	public class Uebung4
	{
		public static int inputInt()
		{
			Scanner sc = new Scanner(System.in);
			System.out.print("Geben Sie eine Zahl ein : ");
			int number = sc.nextInt();
			sc.close();
			return number;
		}
		
		/*
		 * in der Methode wird <code>isPrime</code> verwendet, um nur ein <code>return</code> am 
		 * Ende der Methode zu realisieren. Man könnte auch statt <code>isPrime = false;</code>
		 * jeweils <code>return false;</code> bzw. statt <code>isPrime = true;</code>
		 * <code>return true;</code> schreiben und bräuchte dann weder <code>isPrime</code> noch
		 * die jeweiligen <code>else</code>-Zweige.
		 */
		public static boolean isPrime(int number)
		{
			boolean isPrime = true;		// true ist wichtig!
			
			if(number<2)
			{
				isPrime = false;
			}
			else 
			{
				if(number==2)
				{
					isPrime=true;
				}
				else
				{
					for(int divider=2; divider<=Math.sqrt(number) && isPrime; divider++)
					{
						if(number % divider == 0)
						{
							isPrime = false;
						}
					}
				}
			}
			
			return isPrime;
		}
		
		public static void printPrimeNumbers(int maximum)
		{
			for(int number=1; number<=maximum; number++)
			{
				if(isPrime(number))
				{
					System.out.print(number+" ");
				}
				else
				{
					System.out.print(". ");
				}
				if(number%30 == 0)
				{
					System.out.println();
				}
			}
		}
		
		/*
		 * in der Methode wird <code>found</code> verwendet, um nur ein <code>return</code> am 
		 * Ende der Methode zu realisieren. Man könnte auch statt <code>smallestDivider = number;</code>
		 * jeweils <code>return number;</code> bzw. statt <code>smallestDivider = divider;</code>
		 * <code>return divider;</code> schreiben und bräuchte dann weder <code>found</code> noch
		 * die jeweiligen <code>else</code>-Zweige.
		 */
		public static int getSmallestDivider(int number)
		{
			int smallestDivider = 0;
			boolean found = false;
			
			if(number<2)
			{
				smallestDivider = number;
			}
			else
			{
				if(isPrime(number))
				{
					smallestDivider = number;
				}
				else
				{
					for(int divider=2; divider<number && !found; divider++)
					{
						if(number % divider == 0)
						{
							smallestDivider = divider;
							found = true;
						}
					}
				}
			}
			return smallestDivider;
		}
		
		public static String createStringOfPrimeFactorization(int number) 
		{
			String s = "";
			/*
			 * 	2 * 2 * 5 * 11 * 13 * 13 * 17 = 632060
			 *  632060 --> 2 
			 *  316030 --> 2
			 *  158015 --> 5
			 *   ...   --> divider
			 *  result/divider == 1
			 */
			int smallestDivider = getSmallestDivider(number);
			s = s + smallestDivider;
			int result = number/smallestDivider;
			
			while(result > 1)
			{
				smallestDivider = getSmallestDivider(result);
				s = s + " * " + smallestDivider;
				result = result/smallestDivider;
			}
			s = s + " = " + number;
			
			return s;
		}

		public static void main(String[] args)
		{
			System.out.printf("%n%n----------- Aufgabe 1 ------------ %n %n");
			int number = inputInt();
			System.out.println("Sie haben " + number + " eingegeben.");
			
			System.out.printf("%n%n----------- Aufgabe 2 ------------ %n %n");
			System.out.println(isPrime(number));
			
			System.out.printf("%n%n----------- Aufgabe 3 ------------ %n %n");
			printPrimeNumbers(number);
			
			System.out.printf("%n%n----------- Aufgabe 4 ------------ %n %n");
			System.out.println(getSmallestDivider(number));
			
			System.out.printf("%n%n----------- Aufgabe 5 ------------ %n %n");
			String output = createStringOfPrimeFactorization(632060);
			System.out.println(output);
			
		
		}

	}
	```
	
??? note "Übung 5"
	
	1. Erstellen Sie ein package `uebungen.uebung5`. 
	2. Erstellen Sie in diesem package eine Klasse `Konto` (ohne `main()`-Methode!)
	3. Erstellen Sie in diesem package eine Klasse `Testklasse` mit `main()`-Methode	
	4. Erstellen Sie in der Klasse `Konto` zwei Objektvariablen
		- `guthaben` vom Typ `double` --> nur in der Klasse sichtbar!
		- `pin` vom Typ `int`	--> ebenfalls nur in der Klasse sichtbar!
	5. Erstellen Sie in der Klasse `Konto` einen Konstruktor für `Konto`
		- diesem Konstruktor wird als Parameter `int pPin` übergeben
		- mit dem Wert des Parameters wird innerhalb des Konstruktors der Wert von `pin` initialisiert
		- Initialisieren Sie im Konstruktor auch die Objektvariable `guthaben`. Sie bekommt den Wert `0.0` (hierfür haben wir also keinen Parameter, wir setzen den initialen Wert einfach generell auf `0.0`)
	6. Erstellen Sie in der Klasse `Konto` eine Objektmethode `einzahlen(double betrag)`
		- diese Objektmethode ist `public` und gibt nichts zurück
		- in dieser Methode wird der Wert der Objektvariablen `guthaben` um den Wert von `betrag` erhöht
		- erzeugen Sie in dieser Methode außerdem eine Ausgabe in der Form:
			```bash
			Es wurden 100,00 Euro eingezahlt.
			```
			falls der `betrag` den Wert `100.0` hatte. Verwenden Sie am besten die `printf()`-Methode, um stets genau 2 Stellen nach dem Komma des Betrages auszugeben (siehe [hier](../hilfsklassen/#formatierung-von-gleikommazahlen)). 
	7. Geben Sie in der `main()`-Methode der `Testklasse` ein:
		```java
		Konto k1 = new Konto(1234);
		
		k1.einzahlen(100.0);
		k1.einzahlen(50.0);
		k1.einzahlen(150.0);
		```
		und führen Sie die `Testklasse` aus. Es sollten folgende Ausgaben erzeugt werden:
		```bash
		Es wurden 100,00 Euro eingezahlt.
		Es wurden 50,00 Euro eingezahlt.
		Es wurden 150,00 Euro eingezahlt.
		```
	8. Erstellen Sie in der Klasse `Konto` eine Objektmethode `kontoauszug(int pPin)`
		- diese Objektmethode ist `public` und gibt nichts zurück
		- einen `kontoauszug(int pPin)` können Sie nur "ziehen", wenn der Parameterwert von `pPin` mit dem Wert der Objektvariablen `pin` übereinstimmt
		- wird der richtige Wert für die `pin` übergeben, geben Sie das `guthaben` in der folgenden Form aus:
			```bash
			Ihr aktuelles Guthaben betraegt 300,00 Euro.
			```
			falls `guthaben` den Wert von `300.0` hat. 
		- wird ein falscher Wert für die `pin` übergeben, geben Sie folgende Ausgabe aus:
			```bash
			Falsche PIN!
			```
	9. Erweitern Sie die `main()`-Methode der Testklasse um folgende Anweisungen:
		```java
		k1.kontoauszug(1235); 		// Falsche PIN!
		k1.kontoauszug(1234); 	
		``` 
		und führen Sie die `Testklasse` aus. Es sollten folgende (weitere) Ausgaben erzeugt werden:
		```bash
		Falsche PIN!
		Ihr aktuelles Guthaben betraegt 300,00 Euro.
		```
	10. Erstellen Sie in der Klasse `Konto` eine Objektmethode `auszahlen(int pPin, double betrag)`
		- diese Objektmethode ist `public` und gibt nichts zurück
		- es kann nur etwas ausgezahlt werden, wenn der Parameterwert von `pPin` mit dem Wert der Objektvariablen `pin` übereinstimmt
		- stimmen die Werte nicht überein, geben Sie erneut 
			```bash
			Falsche PIN!
			```
			aus. 
		- stimmt der `pin`-Wert, dann müssen Sie prüfen, ob das `guthaben` reicht, um `betrag` auszuzahlen. Ist nicht genug `guthaben` vorhanden, dann geben Sie aus
			```bash
			Ihr Guthaben reicht nicht, um 400,00 Euro auszuzahlen.
			``` 
			falls `betrag` den Wert `400.0` hatte. 
		- wenn der `pin`-Wert stimmt und genug `guthaben` vorhanden ist, um den `betrag` auszuzahlen, dann reduzieren Sie `guthaben` um den entsprechenden `betrag` und geben aus
			```bash
			Es wurden 100,00 Euro ausgezahlt.
			```
			falls der `betrag` den Wert `100.0` hatte.
	11. Erweitern Sie die `main()`-Methode der Testklasse um folgende Anweisungen:
		```java
		k1.auszahlen(1235, 100.0); 	// Falsche PIN!
		k1.auszahlen(1234, 100.0); 	
		k1.kontoauszug(1234); 		
		k1.auszahlen(1234, 300.0);	// Guthaben reicht nicht
		k1.auszahlen(1234, 200.0); 	
		k1.kontoauszug(1234); 	
		``` 
		und führen Sie die `Testklasse` aus. Es sollten folgende (weitere) Ausgaben erzeugt werden:
		```bash
		Falsche PIN!
		Es wurden 100,00 Euro ausgezahlt.
		Ihr aktuelles Guthaben betraegt 200,00 Euro.
		Ihr Guthaben reicht nicht, um 300,00 Euro auszuzahlen.
		Es wurden 200,00 Euro ausgezahlt.
		Ihr aktuelles Guthaben betraegt 0,00 Euro.
		```
	12. **Zusatz:** 
		- Erweitern Sie die Klasse um eine weitere Objektvariable `private double dispogrenze`
		- Initialisieren Sie diese Variable innerhalb des Konstruktors (ohne weiteren Parmeter) auf den Wert `-1000.0`. Sie dürfen somit Ihr Konto um `1000.00 Euro` überziehen.
		- Passen Sie die `auszahlen()`-Methode entsprechend an, so dass es auch möglich ist, einen `betrag` auszuzahlen, so lange man nicht unter die `dispogrenze` fällt.
		- Erstellen Sie eine Methode `public void zinsenZahlen()`.
			- Erstellen Sie in dieser Methode zwei [Konstanten](../variablen/#konstanten)
				- `DISPOZINSEN` vom Typ `double` bekommt den Wert `12.0` (soll `12%` entsprechen) und
				- `GUTHABENZINSEN` vom Typ `double` bekommt den Wert `0.5` (soll `0.5%` entsprechen) 
			- Berechnen Sie innerhalb der Methode die Zinsen für das Konto
				- `DISPOZINSEN` werden fällig (werden von `guthaben` abgezogen), falls `guthaben` negativ ist
				- `GUTHABENZINSEN` werden gewährt (werden zu `guthaben` addiert), falls `guthaben` positiv ist
				- passen Sie den Wert von `guthaben` entsprechend an
				- erzeugen Sie entsprechende Ausgaben, z.B. 
					```bash
					Ihnen wurden 18,00 Euro Zinsen abgebucht.
					```
					bzw.
					```bash
					Ihnen wurden 4,16 Euro Zinsen gutgeschrieben.
					```
		- Angenommen, die gesamte `main()`-Methode sieht jetzt so aus:
			```java
			public static void main(String[] args)
			{
				Konto k1 = new Konto(1234);
				
				k1.einzahlen(100.0);
				k1.einzahlen(50.0);
				k1.einzahlen(150.0);
				
				k1.kontoauszug(1235); 		// Falsche PIN!
				k1.kontoauszug(1234); 		
				
				k1.auszahlen(1235, 100.0); 	// Falsche PIN!
				k1.auszahlen(1234, 100.0); 	
				k1.kontoauszug(1234); 		
				k1.auszahlen(1234, 300.0);	
				k1.auszahlen(1234, 200.0); 	
				k1.kontoauszug(1234); 
				
				k1.einzahlen(150.0);
				k1.kontoauszug(1234); 		
				k1.zinsenZahlen();
				k1.kontoauszug(1234); 		
				k1.einzahlen(1000.0);
				k1.kontoauszug(1234); 		
				k1.zinsenZahlen();
				k1.kontoauszug(1234); 
			}
			```
			dann sollten Sie folgende Ausgabe erzeugen (gilt nur für **Zusatz**!):
			```bash
			Es wurden 100,00 Euro eingezahlt.
			Es wurden 50,00 Euro eingezahlt.
			Es wurden 150,00 Euro eingezahlt.
			Falsche PIN!
			Ihr aktuelles Guthaben betraegt 300,00 Euro.
			Falsche PIN!
			Es wurden 100,00 Euro ausgezahlt.
			Ihr aktuelles Guthaben betraegt 200,00 Euro.
			Es wurden 300,00 Euro ausgezahlt.
			Es wurden 200,00 Euro ausgezahlt.
			Ihr aktuelles Guthaben betraegt -300,00 Euro.
			Es wurden 150,00 Euro eingezahlt.
			Ihr aktuelles Guthaben betraegt -150,00 Euro.
			Ihnen wurden 18,00 Euro Zinsen abgebucht.
			Ihr aktuelles Guthaben betraegt -168,00 Euro.
			Es wurden 1000,00 Euro eingezahlt.
			Ihr aktuelles Guthaben betraegt 832,00 Euro.
			Ihnen wurden 4,16 Euro Zinsen gutgeschrieben.
			Ihr aktuelles Guthaben betraegt 836,16 Euro.
			```

??? question "Eine mögliche Lösung für Übung 5"
	=== "Konto.java"
		```java 
		package uebungen.uebung5;

		public class Konto
		{
			private double guthaben;
			private int pin;
			private double dispogrenze;
			
			public Konto(int pPin)
			{
				guthaben = 0;
				pin = pPin;
				dispogrenze = -1000.0;
			}
			
			public void einzahlen(double betrag)
			{
				guthaben = guthaben + betrag;
				System.out.printf("Es wurden %.2f Euro eingezahlt.%n", betrag);
			}
			
			public void auszahlen(int pPin, double betrag)
			{
				if(pin==pPin)
				{
					if(guthaben - dispogrenze >= betrag)
					{
						guthaben = guthaben - betrag;
						System.out.printf("Es wurden %.2f Euro ausgezahlt.%n", betrag);
					}
					else
					{
						System.out.printf("Ihr Guthaben reicht nicht, um %.2f Euro auszuzahlen.%n", betrag);
					}
				}
				else
				{
					System.out.println("Falsche PIN!");
				}
			}
			
			public void kontoauszug(int pPin)
			{
				if(pin==pPin)
				{
					System.out.printf("Ihr aktuelles Guthaben betraegt %.2f Euro.%n", guthaben);
				}
				else
				{
					System.out.println("Falsche PIN!");
				}
			}
			
			public void zinsenZahlen()
			{
				final double DISPOZINSEN = 12.0;
				final double GUTHABENZINSEN = 0.5;
				if(guthaben >0)
				{
					double zinsen = guthaben * GUTHABENZINSEN / 100.0;
					guthaben = guthaben + zinsen;
					System.out.printf("Ihnen wurden %.2f Euro Zinsen gutgeschrieben.%n", zinsen);
				}
				else
				{
					double zinsen = guthaben * DISPOZINSEN / 100.0;		// ist negativ!
					guthaben = guthaben + zinsen;
					System.out.printf("Ihnen wurden %.2f Euro Zinsen abgebucht.%n", -zinsen);
				}
			}
		}
		```
	=== "Testklasse.java"
		```java 
		package uebungen.uebung5;

		public class Testklasse
		{

			public static void main(String[] args)
			{
				Konto k1 = new Konto(1234);
				
				k1.einzahlen(100.0);
				k1.einzahlen(50.0);
				k1.einzahlen(150.0);
				
				k1.kontoauszug(1235); 		// Falsche PIN!
				k1.kontoauszug(1234); 		
				
				k1.auszahlen(1235, 100.0); 	// Falsche PIN!
				k1.auszahlen(1234, 100.0); 	
				k1.kontoauszug(1234); 		
				k1.auszahlen(1234, 300.0);	
				k1.auszahlen(1234, 200.0); 	
				k1.kontoauszug(1234); 
				
				k1.einzahlen(150.0);
				k1.kontoauszug(1234); 		
				k1.zinsenZahlen();
				k1.kontoauszug(1234); 		
				k1.einzahlen(1000.0);
				k1.kontoauszug(1234); 		
				k1.zinsenZahlen();
				k1.kontoauszug(1234); 
			}
		}
		```


??? note "Übung 6"
	
	1. Erstellen Sie ein package `uebungen.uebung6`. 
	2. Erstellen Sie in diesem package eine Klasse `Rectangle` (ohne `main()`-Methode!)
	3. Erstellen Sie in diesem package eine Klasse `Testklasse` mit `main()`-Methode	
	4. Erstellen Sie in der Klasse `Rectangle` zwei Objektvariablen
		- `a` vom Typ `int` --> nur in der Klasse sichtbar!
		- `b` vom Typ `int`	--> ebenfalls nur in der Klasse sichtbar!
		`a` und `b` sollen die Seiten des Rechtecks sein. 
	5. Implementieren Sie einen parameterlosen Konstruktor `Rectangle()`, der für die Seite `a` den Wert `10` und für die Seite `b` den Wert `20` setzt. 
	6. Implementieren Sie einen parametrisierten Konstruktor `Rectangle(int a, int b)`, der die Parameterwerte zum Initialisieren der Seiten verwendet. 
	7. Implementieren Sie eine Objektmethode `public int area()`, die den Flächeninhalt des Rechtecks zurückgibt. 
	8. Implementieren Sie eine Objektmethode `public int perimeter()`, die den Umfang des Rechtecks zurückgibt. 
	9. Implementieren Sie eine Objektmethode `public String toString()`, die einen `String` mit allen Informationen des Rechtecks in der folgenden Form
		```bash
		Rectangle : ( a=10, b=20, area=200, perimeter=60 )
		```
		zurückgibt. 
	10. Implementieren Sie eine Objektmethode `public void print()`, die den durch `toString()` erzeugten `String` auf die Konsole ausgibt.
	11. Geben Sie in der `main()`-Methode der `Testklasse` ein:
		```java
		// Objekte erzeugen
		Rectangle r1 = new Rectangle();
		Rectangle r2 = new Rectangle(12, 18);
		Rectangle r3 = new Rectangle(40, 5);
		Rectangle r4 = new Rectangle(20, 10);
		Rectangle r5 = new Rectangle(11, 21);
		
		System.out.printf("%n%n--------------- print()-Methode -----------------%n%n");
		r1.print();
		r2.print();
		r3.print();
		r4.print();
		r5.print();
		```
		und führen Sie die `Testklasse` aus. Es sollten folgende Ausgaben erzeugt werden:
		```bash
		--------------- print()-Methode -----------------

		Rectangle : ( a=10, b=20, area=200, perimeter=60 )
		Rectangle : ( a=12, b=18, area=216, perimeter=60 )
		Rectangle : ( a=40, b= 5, area=200, perimeter=90 )
		Rectangle : ( a=20, b=10, area=200, perimeter=60 )
		Rectangle : ( a=11, b=21, area=231, perimeter=64 )
		```
	12. Implementieren Sie eine Objektmethode `public boolean sidesAreEqual(Rectangle r)`, die ein `true` zurückgibt, wenn die Seiten des aufrufenden Objektes gleich den Seiten des Rectangle `r` sind. Beachten Sie, dass das Rechteck auch gedreht noch gleiche Seiten haben soll, also `a=10, b=20` ist nicht nur mit `a=10, b=20` gleich, sondern auch mit `a=20, b=10`. Wenn die Seiten ungleich sind, gibt die Methode ein `false` zurück.
	13. Implementieren Sie eine Objektmethode `public boolean areasAreEqual(Rectangle r)`, die ein `true` zurückgibt, wenn die Flächeninhalte des aufrufenden Objektes und des Rectangle `r` gleich sind. Ansonsten `false`.
	14. Implementieren Sie eine Objektmethode `public boolean perimetersAreEqual(Rectangle r)`, die ein `true` zurückgibt, wenn die Umfänge des aufrufenden Objektes und des Rectangle `r` gleich sind. Ansonsten `false`.
	15. Implementieren Sie eine Objektmethode `public void printComparison(Rectangle r)`, die die Vergleiche mit `r` in der unten dargestellten Form ausgibt. Rufen Sie in der Methode die Methoden `print()` (oder `toString()`), `sidesAreEqual()`, `areasAreEqual()` und `perimetersAreEqual()` auf. 
	16. Fügen Sie in der `main()`-Methode der `Testklasse` folgende Anweisungen hinzu:
		```java	
		System.out.printf("%n%n---------- printComparison()-Methode ------------%n%n");
		r1.printComparison(r2);
		r1.printComparison(r3);
		r1.printComparison(r4);
		r1.printComparison(r5);
		```
		und führen Sie die `Testklasse` aus. Es sollten folgende zusätzliche Ausgaben erzeugt werden:
		```bash
		---------- printComparison()-Methode ------------

		this      Rectangle : ( a=10, b=20, area=200, perimeter=60 ) 
		the other Rectangle : ( a=12, b=18, area=216, perimeter=60 ) 
		sides are not equal 
		areas are not equal 
		perimeters are equal 

		this      Rectangle : ( a=10, b=20, area=200, perimeter=60 ) 
		the other Rectangle : ( a=40, b= 5, area=200, perimeter=90 ) 
		sides are not equal 
		areas are equal 
		perimeters are not equal 

		this      Rectangle : ( a=10, b=20, area=200, perimeter=60 ) 
		the other Rectangle : ( a=20, b=10, area=200, perimeter=60 ) 
		sides are equal 
		areas are equal 
		perimeters are equal 

		this      Rectangle : ( a=10, b=20, area=200, perimeter=60 ) 
		the other Rectangle : ( a=11, b=21, area=231, perimeter=64 ) 
		sides are not equal 
		areas are not equal 
		perimeters are not equal 
		```
	17. **Zusatz:** 
		- Implementieren Sie eine Objektmethode `public double diagonal()`, die die Länge einer Diagonalen des Rechtecks zurückgibt. 
		- Erweitern Sie die `toString()`-Methode um die Ausgabe dieser Länge wie folgt:
			```bash
			Rectangle : ( a=10, b=20, area=200, perimeter=60, diagonal=22,361 )
			Rectangle : ( a=12, b=18, area=216, perimeter=60, diagonal=21,633 )
			Rectangle : ( a=40, b= 5, area=200, perimeter=90, diagonal=40,311 )
			Rectangle : ( a=20, b=10, area=200, perimeter=60, diagonal=22,361 )
			Rectangle : ( a=11, b=21, area=231, perimeter=64, diagonal=23,707 )
			``` 
			
		- Implementieren Sie eine Objektmethode `public void scale(int factor)`. Diese Methode "skaliert" (vergrößert oder verkleinert) das Rechteck um den Faktor `factor`, genauer gesagt, wird der **Flächeninhalt** um diesen Faktor skaliert (vergrößert oder verkleinert). Die neuen Seiten sollen das gleiche Verhältnis zueinander haben, wie die alten Seiten. Geben Sie die neuen Seitenlängen in der folgenden Form auf die Konsole aus (siehe nächsten Punkt `main()`).
		- Fügen Sie in der `main()`-Methode der `Testklasse` folgende Anweisungen hinzu:
		```java	
		System.out.printf("%n%n--------------- scale()-Methode -----------------%n%n");
		r1.scale(2);
		r2.scale(2);
		r3.scale(2);
		r4.scale(2);
		r5.scale(2);
		r1.scale(10);
		r2.scale(10);
		r3.scale(10);
		r4.scale(10);
		r5.scale(10);
		```
		und führen Sie die `Testklasse` aus. Es sollten folgende zusätzliche Ausgaben erzeugt werden:
		```bash
		--------------- scale()-Methode -----------------

		newArea=  400,00 newA= 14,14 newB= 28,28 check (newA*newB)= 400,00
		newArea=  432,00 newA= 16,97 newB= 25,46 check (newA*newB)= 432,00
		newArea=  400,00 newA= 56,57 newB=  7,07 check (newA*newB)= 400,00
		newArea=  400,00 newA= 28,28 newB= 14,14 check (newA*newB)= 400,00
		newArea=  462,00 newA= 15,56 newB= 29,70 check (newA*newB)= 462,00
		newArea= 2000,00 newA= 31,62 newB= 63,25 check (newA*newB)=2000,00
		newArea= 2160,00 newA= 37,95 newB= 56,92 check (newA*newB)=2160,00
		newArea= 2000,00 newA=126,49 newB= 15,81 check (newA*newB)=2000,00
		newArea= 2000,00 newA= 63,25 newB= 31,62 check (newA*newB)=2000,00
		newArea= 2310,00 newA= 34,79 newB= 66,41 check (newA*newB)=2310,00
		```


??? question "Eine mögliche Lösung für Übung 6"
	=== "Rectangle.java"
		```java 
		package uebungen.uebung6;

		public class Rectangle
		{
			private int a;
			private int b;
			
			public Rectangle()
			{
				this.a = 10;
				this.b = 20;
			}
			
			public Rectangle(int a, int b)
			{
				this.a = a;
				this.b = b;
			}
			
			public int area()
			{
				return this.a * this.b;
			}
			
			public int perimeter()
			{
				return 2 * (this.a + this.b);
			}
			
			public double diagonal()
			{
				int a2 = this.a * this.a;
				int b2 = this.b * this.b;
				double diagonal = Math.sqrt(a2 + b2);
				return diagonal;
			}
			
			public String toString()
			{
				/*
				return "Rectangle : ( a=" + 
						this.a + ", b=" + 
						this.b + ", area=" + 
						this.area() + ", perimeter=" + 
						this.perimeter() + ", diagonal=" +
						this.diagonal() + " )";
						*/
				return String.format("Rectangle : ( a=%2d, b=%2d, area=%3d, "
						+ "perimeter=%2d, diagonal=%.3f )", 
						this.a, 
						this.b, 
						this.area(), 
						this.perimeter(),
						this.diagonal());
				
			}
			
			public void print()
			{
				System.out.println( this.toString() );
			}
			
			public boolean sidesAreEqual(Rectangle r)
			{
				return (this.a == r.a && this.b == r.b) ||
						(this.a == r.b && this.b == r.a);
			}
			
			public boolean areasAreEqual(Rectangle r)
			{
				return (this.area() == r.area());
			}
			
			public boolean perimetersAreEqual(Rectangle r)
			{
				return (this.perimeter() == r.perimeter());
			}
			
			public void printComparison(Rectangle r)
			{
				System.out.printf("%-9s %s %n", "this", this.toString());
				System.out.printf("%-9s %s %n", "the other", r.toString());
				if(this.sidesAreEqual(r))
				{
					System.out.println("sides are equal");
				}
				else
				{
					System.out.println("sides are not equal");
				}
				if(this.areasAreEqual(r))
				{
					System.out.println("areas are equal");
				}
				else
				{
					System.out.println("areas are not equal");
				}
				if(this.perimetersAreEqual(r))
				{
					System.out.println("perimeters are equal");
				}
				else
				{
					System.out.println("perimeters are not equal");
				}
				System.out.println();
			}
		}

		```
	=== "Testklasse.java"
		```java 
		package uebungen.uebung6;

		public class Testklasse
		{

			public static void main(String[] args)
			{
				// Objekte erzeugen
				Rectangle r1 = new Rectangle();
				Rectangle r2 = new Rectangle(12, 18);
				Rectangle r3 = new Rectangle(40, 5);
				Rectangle r4 = new Rectangle(20, 10);
				Rectangle r5 = new Rectangle(11, 21);

				System.out.printf("%n%n--------------- print()-Methode -----------------%n%n");
				r1.print();
				r2.print();
				r3.print();
				r4.print();
				r5.print();

				System.out.printf("%n%n---------- printComparison()-Methode ------------%n%n");
				r1.printComparison(r2);
				r1.printComparison(r3);
				r1.printComparison(r4);
				r1.printComparison(r5);

			}

		}
		```


??? "Übung 7"
	
	---

	**Info:** Wir erstellen uns zwei neue Datentypen `Counter` und `Clock`. Die Idee der Klasse `Counter` soll sein, einen `counter` bis zu einem bestimmten `limit` hochzuzählen. Bevor der `counter` das `limit` erreicht, wird er wieder auf `0` gesetzt. Angenommen also das `limit` ist `60` und der `counter` hat den aktuellen Wert `59` und soll erhöht werden, dann ist der nächste Wert von `counter` wieder `0`, da das `limit` erreicht wurde. Die Klasse `Clock` verwendet zwei `Counter`-Objekte, eins für `hours` und das andere für `minutes`.

	---
	
	1. Erstellen Sie ein package `uebungen.uebung7`. 
	2. Erstellen Sie in diesem package eine Klasse `Counter` (ohne `main()`-Methode!)
	3. Erstellen Sie in diesem package eine Klasse `Programmklasse` mit `main()`-Methode	
	4. Erstellen Sie in der Klasse `Counter` zwei Objektvariablen
		- `counter` vom Typ `int` --> nur in der Klasse sichtbar!
		- `limit` vom Typ `int`	--> ebenfalls nur in der Klasse sichtbar!

	5. Erstellen Sie einen parametrisierten Konstruktor `public Counter(int limit)`, der den `counter` auf `0` initialisiert und das `limit` auf den Parameterwert. 

	6. Implementieren Sie eine Methode `public boolean increase()`. Diese Methode soll den Wert von `counter` um `1` erhöhen. Es muss jedoch geprüft werden, ob eventuell das `limit` erreicht wurde. Sollte dies der Fall sein, wird der Wert von `counter` wieder auf `0` gesetzt. Wird der `counter` tatsächlich um `1` erhöht, gibt die Methode ein `true` zurück, wurde der Wert von `counter` jedoch auf `0` gesetzt, gibt die Methode `false` zurück. Beispiel:

		- Angenommen `counter` hat den Wert `58` und das `limit` ist `60`. Dann ist der neue Wert von `counter` `59` und die Methode gibt `true` zurück. 

		- Angenommen `counter` hat den Wert `59` und das `limit` ist `60`. Dann ist der neue Wert von `counter` `0` und die Methode gibt `false` zurück. 

	7. Implementieren Sie eine Methode `public String toString()`. Diese Methode gibt den Wert von `counter` als zweistelligen String zurück. Beachten Sie

		- Ist der Wert von `counter` einstellig, z.B. `5`, dann soll der String `"05"` zurückgegeben werden.

	8. Implementieren Sie eine Methode `public void print()`. Diese Methode gibt den aktuellen Wert von `counter` unter Verwendung der Methode `toString()` auf die Konsole aus. 

	9. Geben Sie in der `main()`-Methode der `Programmklasse` ein:
		```java
		System.out.printf("%n---------------- Test Counter -----------%n%n");
		
		Counter counter = new Counter(60);
		for(int i=0; i<120; i++)
		{
			counter.increase();
			System.out.printf("%3d : ", i);
			counter.print();
		}
		```
		und führen Sie die `Testklasse` aus. Es sollten folgende Ausgaben erzeugt werden:

		??? "Ausgabe auf der Konsole"

			```bash

			---------------- Test Counter -----------

			  0 : 01
			  1 : 02
			  2 : 03
			  3 : 04
			  4 : 05
			  5 : 06
			  6 : 07
			  7 : 08
			  8 : 09
			  9 : 10
			 10 : 11
			 11 : 12
			 12 : 13
			 13 : 14
			 14 : 15
			 15 : 16
			 16 : 17
			 17 : 18
			 18 : 19
			 19 : 20
			 20 : 21
			 21 : 22
			 22 : 23
			 23 : 24
			 24 : 25
			 25 : 26
			 26 : 27
			 27 : 28
			 28 : 29
			 29 : 30
			 30 : 31
			 31 : 32
			 32 : 33
			 33 : 34
			 34 : 35
			 35 : 36
			 36 : 37
			 37 : 38
			 38 : 39
			 39 : 40
			 40 : 41
			 41 : 42
			 42 : 43
			 43 : 44
			 44 : 45
			 45 : 46
			 46 : 47
			 47 : 48
			 48 : 49
			 49 : 50
			 50 : 51
			 51 : 52
			 52 : 53
			 53 : 54
			 54 : 55
			 55 : 56
			 56 : 57
			 57 : 58
			 58 : 59
			 59 : 00
			 60 : 01
			 61 : 02
			 62 : 03
			 63 : 04
			 64 : 05
			 65 : 06
			 66 : 07
			 67 : 08
			 68 : 09
			 69 : 10
			 70 : 11
			 71 : 12
			 72 : 13
			 73 : 14
			 74 : 15
			 75 : 16
			 76 : 17
			 77 : 18
			 78 : 19
			 79 : 20
			 80 : 21
			 81 : 22
			 82 : 23
			 83 : 24
			 84 : 25
			 85 : 26
			 86 : 27
			 87 : 28
			 88 : 29
			 89 : 30
			 90 : 31
			 91 : 32
			 92 : 33
			 93 : 34
			 94 : 35
			 95 : 36
			 96 : 37
			 97 : 38
			 98 : 39
			 99 : 40
			100 : 41
			101 : 42
			102 : 43
			103 : 44
			104 : 45
			105 : 46
			106 : 47
			107 : 48
			108 : 49
			109 : 50
			110 : 51
			111 : 52
			112 : 53
			113 : 54
			114 : 55
			115 : 56
			116 : 57
			117 : 58
			118 : 59
			119 : 00
			```

	10. Erstellen Sie im package eine weitere Klasse `Clock`. In der Klasse `Clock` verwenden Sie zwei `Counter`. Der eine `Counter` zählt die `minutes` und hat das `limit` `60` und der andere `Counter` zählt die `hours` und hat das `limit` `24`.  

	11. In der Klasse `Clock` erstellen Sie zwei Objektvariablen `minutes` und `hours`, jeweils vom Typ `Counter` (beide nur in der Klasse sichtbar). 

	12. Erstellen Sie einen parameterlosen Konstruktor `public Clock()`. Darin erzeugen Sie für `minutes` das `Counter`-Objekt mit dem `limit` `60` und für `hours` das `Counter`-Objekt mit dem `limit` `24`.  

	13. Implementieren Sie eine Methode `public void increase()`. Diese Methode soll den Wert von `minutes` um `1` erhöhen. Sollte jedoch das `limit` von `minutes` erreicht sein, wird auch `hours` um `1` erhöht. Nutzen Sie die `increase()`-Methode von `Counter`!

	14. Implementieren Sie eine Methode `public String toString()`. Diese Methode gibt die Werte von `minutes` und `hours` in der Form `hh:mm`als String zurück, also z.B. `"23:59"` oder `"01:09"`. Nutzen Sie die `toString()`-Methode von `Counter`!

	15. Implementieren Sie eine Methode `public void print()`. Diese Methode gibt den aktuellen Wert von `Clock` unter Verwendung der Methode `toString()` auf die Konsole aus. 

	16. Fügen Sie in der `main()`-Methode der `Programmklasse` folgende Anweisungen hinzu:
		```java	
		
		System.out.printf("%n----------------- Test Clock ------------%n%n");
		
	    Clock clock = new Clock();
	    for(int i=0; i<1600; i++)
	    {
	        clock.increase();
	        if(i%50==0)
	        {
	            System.out.printf("%4d : ", i);
	            clock.print();
	        }
	    }
	    ```
		und führen Sie die `Programmklasse` aus. Es sollten folgende zusätzliche Ausgaben erzeugt werden:

		??? "Ausgabe auf der Konsole"

			```bash
			----------------- Test Clock ------------

			   0 : 00:01
			  50 : 00:51
			 100 : 01:41
			 150 : 02:31
			 200 : 03:21
			 250 : 04:11
			 300 : 05:01
			 350 : 05:51
			 400 : 06:41
			 450 : 07:31
			 500 : 08:21
			 550 : 09:11
			 600 : 10:01
			 650 : 10:51
			 700 : 11:41
			 750 : 12:31
			 800 : 13:21
			 850 : 14:11
			 900 : 15:01
			 950 : 15:51
			1000 : 16:41
			1050 : 17:31
			1100 : 18:21
			1150 : 19:11
			1200 : 20:01
			1250 : 20:51
			1300 : 21:41
			1350 : 22:31
			1400 : 23:21
			1450 : 00:11
			1500 : 01:01
			1550 : 01:51
			```


??? question "Eine mögliche Lösung für Übung 7"
	=== "Counter.java"
		```java 
		package uebungen.uebung7;

		public class Counter
		{
			private int counter;
			private int limit;
			
			public Counter(int limit)
			{
				this.counter = 0;
				this.limit = limit;
			}
			
			public boolean increase()
			{
				boolean increased = true;
				if(this.counter < this.limit - 1)
				{
					this.counter++;
				}
				else
				{
					this.counter = 0;
					increased = false;
				}
				return increased;
			}
			
			@Override
			public String toString()
			{
		//		String s = "";
		//		if(this.counter < 10)
		//		{
		//			s += "0" + this.counter;	// s = s + "0" + this.counter
		//		}
		//		else
		//		{
		//			s += this.counter;			// s = s + this.counter
		//		}
		//		return s;
				return String.format("%02d", this.counter);
			}
			
			public void print()
			{
				System.out.println(this.toString());
			}
		}

		```
	=== "Clock.java"
		```java 
		package uebungen.uebung7;

		public class Clock
		{
			private Counter minutes;
			private Counter hours;
			
			public Clock()
			{
				this.minutes = new Counter(60);
				this.hours = new Counter(24);
			}
			
			public void increase()
			{
				boolean increased = this.minutes.increase();
				if(!increased)
				{
					this.hours.increase();
				}
			}
			
			@Override
			public String toString()
			{
				return this.hours.toString() + ":" + this.minutes.toString();
			}
			
			public void print()
			{
				System.out.println(this.toString());
			}
		}

		```
	=== "Programmklasse.java"
		```java 
		package uebungen.uebung7;

		public class Programmklasse
		{

			public static void main(String[] args)
			{
				System.out.printf("%n---------------- Test Counter -----------%n%n");

				Counter counter = new Counter(60);
				for(int i=0; i<120; i++)
				{
				    counter.increase();
				    System.out.printf("%3d : ", i);
				    counter.print();
				}
				
				System.out.printf("%n----------------- Test Clock ------------%n%n");

				Clock clock = new Clock();
				for(int i=0; i<1600; i++)
				{
				    clock.increase();
				    if(i%50==0)
				    {
				        System.out.printf("%4d : ", i);
				        clock.print();
				    }
				}


			}

		}

		```


??? note "Übung 8"
	
	1. Erstellen Sie ein package `uebungen.uebung8`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung8` mit `main()`-Methode.
	3. Implementieren Sie eine `public static void print(char[] ca)`-Methode, so dass das `char[] ca` auf die Konsole ausgegeben wird. Achten Sie darauf, dass hinter dem letzten Element kein Komma steht. Testen Sie Ihre Methode auch für ein leeres Array.<br/>
		Bsp:  `print(['a', 'b', 'c', 'a', 'c', 'a', 'b', 'c'])` <br/>
		Ausgabe auf Konsole: `[a, b, c, a, c, a, b, c]`

	4. Kopieren Sie die `print`-Methode vollständig und ändern Sie den Typ des Parameters von `char[]` in `int[]`. (Die Methode ist jetzt *überladen* und `print()` kann jetzt entweder ein `char[]` oder ein `int[]` übergeben werden, welches auf die Konsole ausgegeben wird.)

	5. Implementieren Sie eine Methode `public static char[] stringToCharArray(String s)`. Diese Methode wandelt einen `String` in ein `char[]` um, so dass jedes Zeichen des Strings im `char[]` enthalten ist. Das `char[]` wird zurückgegeben. 
		Tipps: die Länge eines Strings wird mit der Objektmethode `length()` ermittelt. Die einzelnen Zeichen eines Strings können mithilfe der `charAt(index)`-Objektmethode von Strings ermittelt werden. Siehe [String](../hilfsklassen/#die-klasse-string) <br/>
		Bsp.: `stringToCharArray("hallo!")` --> `['h','a','l','l','o','!']` 

	7. Implementieren Sie eine Methode `public static int[] minAndMax(int[] iarr)`, der ein `int`-Array als Parameter übergeben wird und die ein zweielementiges Array zurückgibt. Das erste Element des zurückgegeben Arrays ist das Minimum des als Parameter übergebenen Arrays und das zweite Element ist das Maximum. <br/>
		Bsp.: 	`minAndMax([4,2,8,1,6,2,4,1,8])` --> `[1,8]` <br/>
              	`minAndMax([4])` --> `[4,4]`

	8. Implementieren Sie eine Methode `public static int[] reverse(int[] iarr)`, der ein `int`-Array übergeben wird und die die Reihenfolge der Elemente des Arrays umdreht (das letzte zuerst usw.) Das neuerstellte Array wird zurückgegeben. <br/>
		Bsp.: `reverse([4,2,8,1,6,2,4,1,8])` --> `[8,1,4,2,6,1,8,2,4]`  <br/>
              `reverse([4])` --> `[4]`

    9. **Zusatz:** 
		- Implementieren Sie eine Methode `public static char[] filter(char[] carr, char filter)`, der als Parameter ein `char`-Array und ein `char` übergeben wird. Die Methode soll ein `char`-Array zurückgeben, das dem als Parameter übergeben Array entspricht, außer dass jedes Vorkommen des als Parameter übergeben `carr` entfernt wurde <br/>
		Bsp: `filter(['a', 'b', 'c', 'a', 'c', 'a', 'b', 'c'], 'c')` --> `['a', 'b', 'a', 'a', 'b']`
    	- Implementieren Sie eine Methode `public static boolean containsDoublets(char[] ca)` die ein `true` zurückgibt, wenn *mindestens* ein Wert in `ca` *mindestens* zwei Mal vorkommt (wenn Sie schon dabei sind, können Sie sich auch überlegen, wenn *genau* ein Wert *genau* zwei Mal vorkommt - oder *mindestens* ein Wert *genau* zwei Mal - oder *genau* ein Wert *mindestens* zwei Mal) und `false` sonst.


	
??? note "Übung 9"
	
	1. Übung 9 vertieft das Verständnis von Programmabläufen, Methodenaufrufen und Algorithmen. 
	2. Walk-throughs und Multiple-choice-Aufgaben.

	
??? note "Übung 10"
	
	1. Erstellen Sie ein package `uebungen.uebung10`. 
	2. Erstellen Sie in diesem package eine Klasse `Uebung10` mit `main()`-Methode.
	3. **Vorabinformation**: 
		- Wir implementieren Würfe eines Würfels. Alle Würfe werden in einem Array `statistics` gespeichert. Das Array hat die Länge 6 und beschreibt, wie oft eine 1, wie oft eine 2, ..., wie oft eine 6 gewürfelt wurde.	

			![statistics](./files/50_statistics.png)

	4. Erstellen Sie sich in der `main()`-Methode zunächst das `statistics`-Array. Alle Elemente des Arrays sind vom Typ `int` und es hat die Länge `6`. 

	5. Implementieren Sie folgende Methoden: 

		- Implementieren Sie eine `public static int throwDice()`-Methode, die eine Zufallszahl aus dem Wertebereich `[1, ... , 6]` erzeugt und zurückgibt.
		
		- Implementieren Sie eine Methode `public static void printThrow(int cast)`, die den Wert des übergebenen Wurfes (`cast`) wie folgt ausgibt (Beispiel `cast==5`):
			```bash
			Es wurde eine 5 gewuerfelt
			```
		
		- Testen Sie beide Methoden, indem Sie in der `main()`-Methode eingeben:
			```java
			System.out.printf("%n%n------------------- Test throwDice and printThrow -------------------%n%n");
			for(int index=0; index<10; index++)
			{
				int cast = throwDice();
				printThrow(cast);
			}
			```

			Sie sollten eine Ausgabe in folgender Form bekommen (Zufallszahlen):
			```bash		
			------------------- Test throwDice and printThrow -------------------

			Es wurde eine 5 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 6 gewuerfelt
			Es wurde eine 5 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 5 gewuerfelt
			Es wurde eine 6 gewuerfelt
			Es wurde eine 6 gewuerfelt
			```

		- Implementieren Sie eine Methode `public static int[] insertIntoStatistics(int[] statistics, int cast)`. Das `statistics`-Array wird als Parameter übergeben und das `statistics`-Array selbst wird auch wieder zurückgegeben! Im `statistics`-Array wird der Wert an der Stelle um `1` erhöht, der dem Wurf `cast` entspricht. D.h. wurde eine `1` gewürfelt, wird der Wert im Index `0` um `1` erhöht, wurde eine `2` gewürfelt, der Wert im Index `1` usw. (siehe auch oben die Abbildung zu `statistics`)

		- Implementieren Sie eine Methode `public static void printStatistics(int[] statistics)`, die das `statistics`-Array wie folgt auf die Konsole ausgibt. <br/>

			Angenommen, das `statistics`-Array ist so befüllt: `[ 3,8,4,5,8,2 ]`, dann ist die Ausgabe auf der Konsole:

			```bash
			[ (3 x 1), (8 x 2), (4 x 3), (5 x 4), (8 x 5), (2 x 6) ]
			```

		- Testen Sie beide Methoden, indem Sie in der `main()`-Methode eingeben:
			```java			
			System.out.printf("%n%n------------------ Test insert- and printStatistics -----------------%n%n");
			for(int index=0; index<100; index++)
			{
				int cast = throwDice();
				statistics = insertIntoStatistics(statistics, cast);
			}
			printStatistics(statistics);	
			```

			Es wird angenommen, dass Sie das `statistics`-Array bereits gleich am Anfang in der `main()` erzeugt haben - wenn nicht, können Sie das auch hier machen. Beachten Sie den Aufruf von `statistics = insertIntoStatistics(statistics, cast);`. Die `insertIntoStatistics()`-Methode bekommt das `statistics`-Array als Parameter übergeben, gibt es selbst wieder zurück und in der `main()`-Methode speichern wir die Rückgabe wieder in der `statistics`-Referenz. Das ist zwar so gar nicht nötig, aber das lernen wir erst, wenn es um Objekte geht. Jetzt ist es völlig in Ordnung, das so zu machen. 

			Sie sollten eine Ausgabe in folgender Form bekommen (Zufallszahlen):
			```bash		
			------------------ Test insert- and printStatistics -----------------

			[  (20 x 1), (13 x 2), (16 x 3), (15 x 4), (19 x 5), (17 x 6) ]
			```

		- Implementieren Sie eine Methode `public static int sumOfStatistics(int[] statistics)`, die eine Summe über alle Werte im `statistics`-Array wie folgt berechnet: <br/>

			**Beispiel**: Angenommen, das Array ist so befüllt: `[ 3,8,4,5,8,2 ]`, dann ist die Summe: `3x1 + 8x2 + 4x3 + 5x4 + 8x5 + 2x6 = 3 + 16 + 12 + 20 + 40 + 12 = 103`. Die Summe `103` wird zurückgegeben.  

		- Testen Sie die Methode, indem Sie in der `main()`-Methode eingeben:
			```java			
			System.out.printf("%n%n--------------------- Test sumOfStatistics --------------------------%n%n");
			printStatistics(statistics);
			int sumTest = sumOfStatistics(statistics);
			System.out.println("Summe = " + sumTest);
			```

			Das `statistics`-Array ist ja bereits oben befüllt worden, das müssen wir hier also nicht mehr machen. Sie sollten eine Ausgabe in folgender Form bekommen (Zufallszahlen):
			```bash		
			--------------------- Test sumOfStatistics --------------------------

			[  (14 x 1), (15 x 2), (11 x 3), (16 x 4), (27 x 5), (17 x 6) ]
			Summe = 378
			```

		- **Zusatz:** Implementieren Sie eine Methode `public static int throwDiceUntilTarget(int target, int[] statistics)`, die so lange einen Würfel würfelt, bis als Summe der Augen das `target` erreicht ist. Die Anzahl der Würfe wird zurückgegeben. In dieser Methode erfolgen folgende Aufrufe:
			- nach jedem Wurf (`throwDice()`) wird der Wurf ausgegeben (`printThrow()`) 
			- jeder Wurf wird in das `statistics`-Array eingetragen (`insertIntoStatistics()`)
			- nach jedem Wurf wird die Summme aller Augen aller bisherigen Würfe ermittelt (`sumOfStatistics()`). 
			- so lange die Summe kleiner ist als das `target`, wird weiter gewürfelt

		- Testen Sie die Methode, indem Sie in der `main()`-Methode eingeben:
			```java				
			System.out.printf("%n%n------------------- Test throwDiceUntilTarget -----------------------%n%n");
			statistics = new int[6];	// altes Array war schon befuellt 
			final int TARGET = 100;
			int tries = throwDiceUntilTarget(TARGET, statistics);
			printStatistics(statistics);
			int sum = sumOfStatistics(statistics);
			System.out.println("Es wurden " + tries + " Versuche benötigt, um " + sum + " Punkte zu erzielen.");
			```

			Da das `statistics`-Array zuvor bereits befüllt war, erstellen wir es für das Testen dieser Methode nochmal neu. Sie sollten eine Ausgabe in folgender Form bekommen (Zufallszahlen):
			```bash		
			------------------- Test throwDiceUntilTarget -----------------------

			Es wurde eine 5 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 5 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 5 gewuerfelt
			Es wurde eine 2 gewuerfelt
			Es wurde eine 5 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 2 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 6 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 2 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 2 gewuerfelt
			Es wurde eine 6 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 3 gewuerfelt
			Es wurde eine 4 gewuerfelt
			Es wurde eine 1 gewuerfelt
			Es wurde eine 6 gewuerfelt
			[  (5 x 1), (4 x 2), (11 x 3), (4 x 4), (4 x 5), (3 x 6) ]
			Es wurden 31 Versuche benötigt, um 100 Punkte zu erzielen.
			```

			Es muss das `target` nicht exakt getroffen werden, das ist Zufall. Es stoppt, sobald `100` oder mehr Punkte erreicht wurden. 



## Zusätzliche Übungen


??? "Binäre Bäume"
	
	---

	**Info:** Wir erstellen uns einen Datentyp `BinaryTreeNode`, der einen Knoten in einem Binärbaum repräsentiert. Hier wird die Verwendung von `null` und Rekursion geübt.

	---
	
	1. Erstellen Sie eine Klasse `BinaryTreeNode`.
	2. Objektvariablen (alle `private`) dieser Klasse sind

		- `value` vom Typ `int`,
		- `left` vom Typ `BinaryTreeNode` und
		- `right` vom Typ `BinaryTreeNode`.

	3. Erstellen Sie einen parametrisierten Konstruktor `public BinaryTreeNode(int value)`, in dem der linke und rechte Teilbaum jeweils auf `null` gesetzt und die Objektvariable `value` mit dem Parameterwert initialisiert werden. 

	4. Implementieren Sie die Methoden `public boolean hasLeft()` und `public boolean hasRight()`, die ein `true` zurückgeben, wenn der linke bzw. rechte Teilbaum ein Objekt ist und `false`, wenn `left` bzw. `right` den Wert `null` haben. 

	5. Implementieren Sie eine Methode `public void insert(int value)`, die die folgende private Methode `private void insert(BinaryTreeNode root, int value)` aufruft.

	6. Implementieren Sie eine Methode `private void insert(BinaryTreeNode root, int value)`, die ein `BinaryTreeNode`-Objekt in den Binärbaum einfügt. Beachten Sie:

		- wenn `value` kleiner ist, als der `value`, von dem Knoten, den Sie gerade betrachten, dann fügen Sie den Wert in den linken Teilbaum ein,
		- wenn `value` größer ist, als der `value`, von dem Knoten, den Sie gerade betrachten, dann fügen Sie den Wert in den rechten Teilbaum ein,
		- wenn im Baum bereits ein Knoten mit `value` existiert, dann wird kein Knoten hinzugefügt. 

		**Tipp:** Sie sollten die Methode am besten rekursiv implementieren.

	7. Implementieren Sie eine Methode `public void print()`, die die folgende private Methode `private void print(int indent)` aufruft.

	8. Implementieren Sie eine Methode `private void print(int indent)`. Diese Methode gibt den `value` des aufrufenden Knotens auf die Konsole aus und ruft dann sowohl die `print(indent)`-Methode des linken Teilbaums als auch die `print(indent)`-Methode des rechten Teilbaums auf, falls sie jeweils existieren. Der `indent`-Parameter ist dazu da, damit für jede Verzweigungstiefe der Wert weiter eingerückt auf der Konsole ausgegeben wird, also z.B. so:

		```bash
		10
		l--------5
		         l--------3
		                  r--------4
		         r--------8
		                  r--------9
		r--------15
		         l--------13
		                  l--------12
		                  r--------14
		         r--------18
		                  l--------17
		```

		**Tipp:** Sie sollten die Methode am besten rekursiv implementieren.

	9. Die `main()`-methode der `Programmklasse` könnte z.B. so aussehen:

		```java
		BinaryTreeNode btn = new BinaryTreeNode(10);
		btn.insert(5);
		btn.insert(15); 
		btn.insert(8); 
		btn.insert(3); 
		btn.insert(18); 
		btn.insert(13);
		btn.insert(14); 
		btn.insert(9); 
		btn.insert(4); 
		btn.insert(17); 
		btn.insert(12);
		btn.print();
		```


??? question "Eine mögliche Lösung für Binäre Bäume"
	=== "BinaryTreeNode.java"
		```java 
		public class BinaryTreeNode
		{
			private int value;
			private BinaryTreeNode left;
			private BinaryTreeNode right;
			
			BinaryTreeNode(int value)
			{
				this.value = value;
				this.left = null;
				this.right = null;	
			}
			
			public boolean hasLeft()
			{
				return this.left != null;
			}
			
			public boolean hasRight()
			{
				return this.right != null;
			}	
			
			public void insert(int value)
			{
				this.insert(this, value);
			}
			
			private void insert(BinaryTreeNode root, int value)
			{ 
				if(value < root.value)
				{
					if(!root.hasLeft())
					{
						root.left = new BinaryTreeNode(value);
					}
					else
					{
						insert(root.left, value);
					}
				}
				else if(value > root.value)
				{
					if(!root.hasRight())
					{
						root.right = new BinaryTreeNode(value);
					}
					else
					{
						insert(root.right, value);
					}
				}
			}
			
			public void print()
			{
				print(1);
			}
			
			private void print(int indent)
			{
				System.out.println(this.value);
				if(this.hasLeft())
				{
					for(int i = 0; i < indent; i++)
					{
						if(i == indent-1) System.out.print("l--------"); 
						else 			  System.out.print("         "); 
					}
					this.left.print(indent+1);
				}

				if(this.hasRight())
				{
					for(int i = 0; i < indent; i++)
					{
						if(i == indent-1) System.out.print("r--------"); 
						else 			  System.out.print("         ");  
					} 
					this.right.print(indent+1);
				}
			}

		}
		```
	=== "Programmklasse.java"
		```java 
		public class Programmklasse
		{

			public static void main(String[] args)
			{
				BinaryTreeNode btn = new BinaryTreeNode(10);
				btn.insert(5);
				btn.insert(15); 
				btn.insert(8); 
				btn.insert(3); 
				btn.insert(18); 
				btn.insert(13);
				btn.insert(14); 
				btn.insert(9); 
				btn.insert(4); 
				btn.insert(17); 
				btn.insert(12);
				btn.print();
			}

		}
		```




