# Javadoc

[Javadoc](https://www.oracle.com/java/technologies/javase/javadoc.html) ist ein Werkzeug, das Teil des [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/downloads/) ist. Es erzeugt aus Javadoc-Kommentaren HTML-Seiten, die im Browser aufgerufen werden können. Die Javadoc-Kommentare aller Klassen aus den Java-Standardpaketen finden Sie z.B. [hier (Java Version 11)](https://docs.oracle.com/en/java/javase/11/docs/api/).

Ein Javadoc-Kommentar beginnt mit `/**` und endet mit `*/`. Ein solcher Kommentar kann sich über mehrer Zeilen erstrecken. Hier nochmal die drei Möglichkeiten der Kommentierung in Java:

```java 

// einzeiliger Kommentar - Kommentar endet am Zeilenende

/*

	Blockkommentar
	kann sich über mehrer Zeilen erstrecken

*/

/**
	Javadoc-Kommentar
	wie Blockkommentar über mehrere Zeilen
	aus Javadoc-Kommentaren erzeugt javadoc 
	HTML-Seiten

*/

```

Eine Anleitung dazu, wie Javadoc-Kommentare geschrieben werden sollten, findet sich [hier](https://www.oracle.com/java/technologies/javase/writing-doc-comments.html).