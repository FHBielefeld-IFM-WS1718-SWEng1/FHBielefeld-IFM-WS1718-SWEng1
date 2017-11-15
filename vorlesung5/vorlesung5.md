# OOA/OOD mit UML-Diagrammen

## Lernziele
- Objektorientierte Modellierung kennenlernen
- Objektorientierte Analyse (OOA) & Objektorientiertes Design (OOD) kennenlernen
- �berblick �ber relevante UML-Diagrammtypen und deren Zusammenspiel
- Wissen, welche UML-Diagramme in welchen Phasen der Softwareentwicklung eingesetzt werden

## Modellbildung
![Modellbildung](vorlesung5/bilder/Bild1.png "Modellbildung")

## OOA / OOD mit UML

### Analysemethoden
- Richtlinien zur Vorgehensweise in der Analysephase
- Beispiele:
        - Strukturierte Analyse (SA)     
        - Objektorientierte Analyse (OOA)

### OOA / OOD
OOA und OOD zerlegen das Softwaresystem mit objektorientierten Verfahren in handhabbare Teile, dadurch ergeben sich Vorteile wie:

- Durchg�ngige und konsistente Beschreibung �ber alle Phasen der Softwareentwicklung hinweg 
(Bei Nutzung von Objektorientierten Sprachen -> Gleiche Konzepte f�r Analyse, Design und Implementierung)
- Erh�hte Verst�ndlichkeit durch Objekte als Konzept aus der realen Welt
- Erh�hte Wiederverwendbarkeit durch relativ abgeschlossene Objektdefinitionen und -implementierungen

### Objektorientierte Analyse (OOA)
Die OOA ist die fachliche Beschreibung der Systemanforderungen und die Pr�zisierung des Problems.
Es beschreibt was das System tun soll und nicht wie es implementiert werden soll.
Au�erdem soll f�r die Verringerung der Komplexit�t herausgefiltert werden, welche die wichtigsten Aspekte f�r die Aufgabe sind.

- Untersuchung und Beschreibung des Systembereichs unabh�ngig von der Programmiersprache
- Testen von Einheiten bereits vor ihrer Fertigstellung
- Ableitung eines Prototypen

### Objektorientiertes Design (OOD)
Das OOD ist eine Erweiterung des OOA-Modells zur Abbildung des Realit�tsmodells auf den L�sungsbereich. Es soll als Vorstufe der Umsetzung direkt in einer Programmiersprache implementierbar sein.

- Erweiterung um systemnahe Klassen
        - Schnittstellen
        - Benutzungsoberfl�che
        - Datenhaltung
        - Verteilung
- Hinzuf�gen von Klassen, Attributen und Methoden, die f�r die Realisierung gebraucht werden (z.B. Datenhaltung in Form einer verketteten Liste)
- Einbeziehung bestehender Entw�rfe und Klassenbibliotheken (z.B.UI-Library) in das Design

## UML
UML ist eine einheitliche Sprache zur Beschreibung von Softwaresystemen und ist insbesondere f�r die Analyse und den Entwurf in der fr�hen Phase der Softwareentwicklung geeignet.
Es enth�lt verschiedene Diagrammtypen, die sich gegenseitig erg�nzen und verschiedene Systemaspekte hervorheben. 

- Erm�glicht die Kommunikation zwischen Entwickler-Entwickler und Entwickler-Benutzer
- Bildet den Problembereich m�glichst genau auf ein (Programmier-) Modell ab
- Analogie zu einem Bauplan f�r ein Haus (Grundriss, Au�enansichten, Werkpl�ne etc.)
- Besitzt einige Freiheitsgrade bei der Modellierung

### UML Diagrammtypen
![UML Diagrammtypen �bersicht](vorlesung5/bilder/Bild2.png "Diagrammtypen �bersicht")

![UML Diagrammtypen 1](vorlesung5/bilder/Bild3.png "UML Diagrammtypen 1")
![UML Diagrammtypen 2](vorlesung5/bilder/Bild4.png "UML Diagrammtypen 2")
![UML Diagrammtypen 3](vorlesung5/bilder/Bild5.png "UML Diagrammtypen 3")

## Modelle und UML-Diagramme
UML wird zur Darstellung und Modellierung eines Software-Systems benutzt. Ein (Software-)System l�sst sich durch eine Menge von Funktionen, Anwendungsf�llen und Diensten modellieren. Auch eine prozessorientierte Darstellung durch eine Menge von Prozessen, Abl�ufen, Vorg�ngen und Workflows ist m�glich. Ein System kann aber auch nur aus Daten und Objekten bestehen. Die Bezieheungen untereinander und die Straktur stehen dann im Fokus.
- Ein System kann und soll in Subsysteme zerlegt werden. Dies besteht aus unabh�ngigen Komponenten.
- Es wird zwischen statischen und dynamischen Modellen unterschieden.
- Die "UML-Pyramide" veranschaulicht die Zugeh�rigkeiten grafisch und ist nicht direkt umzusetzen, sondern soll grob den gesamten Prozess aufzeigen.
![UML-Pyramide](vorlesung5/bilder/Bild6.png "UML-Pyramide")

Die Diagramme verfeinern sich von oben nach unten auf der Pyramide. Das statische Modell zeigt eine Gesamtsicht auf das Problemfeld und l�sst unwesentliche Details weg, w�hrend das dynamische Modell das Sysremverhalten darstellt und zeitlicher Ablauf, Zust�nde und �berg�nge im Vordergrund stehen.

Ein Use-Case (Anwendungsfall) beschreibt Anforderungen und bestimmt den Funktionsumfang.
- Au�ensicht auf das Produkt
- Kommunikationsgrundlage mit Kunden
- Testgrundlage/ Erstellung fr�her Prototypen

Ein Dynamisches Aktivit�tsdiagramm beschreibt genau einen Workflow, wodurch sich bereits erste Klassen, Objekte und Beziehungen untereinander gewinnen lassen.
Ein statisches Paketdiagramm besteht aus zusammenh�ngenden Klassen und ist ohne weitere Kenntnis der einzelnen Klassen verstehbar.
Paket- und Klassendiagramme geben einen �berblick �ber die Ergebnisse des statischen Softwareentwurfs.
Sequenz- und Kommunikationsdiagramme werden benutzt wenn das Verhalten im Vordergrund steht. Sie beschreiben den Nachrichtenaustausch in einem System.
In Zustands�bergangsdiagrammen geht es um den Zustand eines einzigen Objekts im Verlauf. Es dient zum Aufsp�ren neuer Attribute und Methoden.

## Zuordnung der UML-Diagrammtypen zu Phasen der Softwareentwicklung
- Anforderungen -> Use-Case Diagramm
- Gesch�ftsprotesse -> Aktivit�tsdiagramm
- Statische Softwarestruktur -> Klassendiagramm
- Dynamisches Verhalten der Software -> Sequenzdiagramm, Zustandsdiagramm
- Struktur von Softwarekomponenten/ Bibliotheken -> Komponentendiagramm
- Zuordnung von Software auf Rechnersysteme -> Verteilungsdiagramm

### Zusammenspiel von UML Diagrammtypen
![Zusammenspiel von UML Diagrammtypen](vorlesung5/bilder/Bild7.png "Zusammenspiel von UML Diagrammtypen")
- Der Ablauf (Workflow) eines Use-Cases wird durch ein Aktivit�tsdiagramm modelliert.
- Szenarien eines Use-Cases werden durch Interaktionsdiagramme (z.B. Sequenzdiagramme) modelliert.
- Ein Use-Case wird durch Klassendiagramme strukturiert und die Klassen werden in Interaktionsdiagrammen verwendet.
- Das Verhalten einer Klasse wird in einem Zustandsdiagramm modelliert.
- Ein Paketdiagramm strukturiert Klassen zu gr��eren Einheiten.

## Pragmatisches "Schritt f�r Schritt" Vorgehensmodell
![Vorgehensmodell 1](vorlesung5/bilder/Bild8.png "Schritt f�r Schritt Vorgehensmodell 1")
![Vorgehensmodell 2](vorlesung5/bilder/Bild9.png "Schritt f�r Schritt Vorgehensmodell 2")
![Vorgehensmodell 3](vorlesung5/bilder/Bild10.png "Schritt f�r Schritt Vorgehensmodell 3")
![Vorgehensmodell 4](vorlesung5/bilder/Bild11.png "Schritt f�r Schritt Vorgehensmodell 4")
![Vorgehensmodell 5](vorlesung5/bilder/Bild12.png "Schritt f�r Schritt Vorgehensmodell 5")