# gitStarted Zusammenfassung
In diesem Repo soll zusammengefasst werden, was man für die Arbeit mit git und gitHub kennen sollte.
- In [diesem cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) finden Sie Hinweise, wie man .md-Dateien formatiert.
- Mit diesen [Generator](https://www.tablesgenerator.com/markdown_tables) können Sie Tabellen für Markdown erzeugen

:dart: Ziele:
1. Die Arbeit soll nicht im Browser stattfinden. Clonen Sie das Repo und arbeiten Sie lokal.
1. Hier gehts um Teamwork: Ich erwarte häufige Commits (+ häufiges pushen/pullen )

## TODO
### **- Begriffe definieren und erklären (z.B. repository, branch etc.)**

Git: 				ein open source, verteiltes Versionskontrollsystem  

GitHub: 			eine Plattform für das Hosting und die Zusammenarbeit an Git-Repositories  

Repository: 		Ein Repository enthält alle Dateien Ihres Projekts und den Revisionsverlauf jeder Datei.  

Branch: 			ein leichtgewichtiger, beweglicher Zeiger auf einen Commit  

Fork: 				eine Kopie eines Repositorys auf GitHub, das einem anderen Benutzer gehört  

Remote: 			ein gemeinsames Repository auf z.B. GitHub, das alle Teammitglieder zum Austausch ihrer Änderungen nutzen  

### **- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)**

`git init`: 			Wandeln Sie ein vorhandenes Verzeichnis in ein Git-Repository um  

`git add`: 			erstellt einen Schnappschuss der Datei als Vorbereitung für die Versionierung  

`git commit -m "message"`:	ein Git-Objekt, ein Schnappschuss des gesamten Repositorys, komprimiert in einer SHA / speichert Datei-Versionen dauerhaft im Versionsverlauf auf  

`git checkout`:		Wechselt zum angegebenen Branch und aktualisiert das Arbeitsverzeichnis (Working directory)  

`git log`: 			listet den Versionsverlauf für den aktuellen Branch auf  

`git status`: 		zeigt den Zustand des working directory und der Staging-area an  

`git HEAD`: 				Der HEAD-Zeiger steht für Ihr aktuelles Arbeitsverzeichnis und kann bei Verwendung von Git Checkout in verschiedene Branches, Tags oder Commits verschoben werden.  

`git reset`: 			Macht alle Commits nach commit rückgängig und behält Änderungen lokal bei  

### **- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)**

`git fetch`: 			Lädt den gesamten Verlauf von den Remote-Tracking-Branches herunter  

`git merge`:			Kombiniert den Remote-Tracking-Branch mit dem aktuellen lokalen Branch  

`git push`: 			Lädt alle lokalen Branch-Commits auf GitHub hoch  

`git clone [url]`: 	Klonen (herunterladen) eines Repositorys, das bereits auf GitHub vorhanden ist, einschließlich aller Dateien, Branches und Commits  

`git pull`:			Aktualisiert Ihren aktuellen lokalen Arbeitsbranch mit allen neuen Commits aus dem entsprechenden Remote-Branch auf GitHub. git pull ist eine Kombination aus git fetch und git merge  


*Wenn man einen lokalen Branch hat, welcher nicht auf dem Remote-Repository existiert, kann man einen Branch mit dem selben Namen auf dem Remote-Repository erstellen*

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
	- Mit Override überschreibt man virtual und abstract methoden einer base klasse 
	- Beispiel: public abstract int Rechner(){}
					public override int Rechner(){}  
					
  - Polymorphie
	- Polymorphismus ist eine Liste die Objekte von Mutter und Kind klassen hinzugefügt
      werden können und bearbeitet werden können.
	- Beispiel: Class Mutter, Class Kind, List<Mutter> mutter = new List<Mutter>();
	  Diese Liste kann jetzt Objekte von die Klassen Mutter und Kind anehmen und bearbeiten.
- Wie überschreibt man die Methode `virtual string ToString()`?
	- Override string TOString(){}