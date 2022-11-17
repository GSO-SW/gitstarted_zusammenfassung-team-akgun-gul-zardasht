# gitStarted Zusammenfassung
In diesem Repo soll zusammengefasst werden, was man für die Arbeit mit git und gitHub kennen sollte.
- In [diesem cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) finden Sie Hinweise, wie man .md-Dateien formatiert.
- Mit diesen [Generator](https://www.tablesgenerator.com/markdown_tables) können Sie Tabellen für Markdown erzeugen

:dart: Ziele:
1. Die Arbeit soll nicht im Browser stattfinden. Clonen Sie das Repo und arbeiten Sie lokal.
1. Hier gehts um Teamwork: Ich erwarte häufige Commits (+ häufiges pushen/pullen )

## TODO
- Begriffe definieren und erklären (z.B. repository, branch etc.)
- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)
- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)

## TODO2
- Fachbegriffe OOP erklären (mit Beispielen)

  - abstract (Klassen)
Man kann kein Objekt einer abstract Klasse erstellen. Man nutzt sie zum vererben.
Zum Beispiel die Klasse Säugetier: Alle Säugetiere haben folgendes gemeinsam:
Alle stillen mit Milch, Sie atmen alle Sauerstoff und gebähren ihre Kinder. 

abstract class Säugetier
{
  #Code
}

  - abstract (Methoden)
Êine abstract Methode ist nicht instanziierbar. Erbende Klassen müssen die abstract
Methode überschreiben. Die abstract Klasse darf in der Mutterklasse keinen Methodenrumpf
haben.
Kann mit Override überschrieben werden.

public abstract int getArea();

 - virtual
Eine virtual Methode kann in der Kinderklasse überschrieben werden.
Kann mit override überschrieben werden.

public virtual double Area()
{
    return x * y;
}

  - override
	(z)	- Mit Override überschreibt man virtual und abstract methoden einer base klasse 
		- Beispiel: public abstract int woRechner(){}
					public override int Rechner(){}
  - Polymorphie
	(z)	- Polymorphismus ist eine Liste die Objekte von Mutter und Kind klassen hinzugefügt
          werden können und bearbeitet werden können.
		- Beispiel: Class Mutter, Class Kind, List<Mutter> mutter = new List<Mutter>();
		  Diese Liste kann jetzt Objekte von die Klassen Mutter und Kind anehmen und bearbeiten.
	
- Wie überschreibt man die Methode `virtual string ToString()`?
	(z)	- Override string TOString(){}

