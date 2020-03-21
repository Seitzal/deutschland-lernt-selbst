 # Diagramme

[Mermaid](https://mermaid-js.github.io/mermaid/#/classDiagram) is used for rendering. It is supported natively by some markdown editors such as [Typora](https://typora.io/), otherwise it is easiest to copypaste the code from and to the [Mermaid web editor](https://mermaid-js.github.io/mermaid-live-editor).

## Entity-Relationship Diagramm

```mermaid
graph LR
	lernt{lernt}
	hat{hat Materialien}
	
	Bundesland ---|n| lernt
	Fach ---|n| lernt
	Klassenstufe ---|n| lernt
	lernt ---|n| Modul
	Modul ---|n| hat
	hat ---|n| Selbstlern-Ressource
	Selbstlern-Ressource --- Link
	Selbstlern-Ressource --- Beschreibung
	Selbstlern-Ressource --- Upvotes
	Selbstlern-Ressource --- Downvotes
```



## Klassen-Diagramm



```mermaid
classDiagram

class Kurs {
	+Bundesland
	+Fach
	+Klassenstufe
	+Liste von Modulnamen
}

class SelbstlernRessourceGithub {
	+Modulname
	+Link
	+Beschreibung
}

class SelbstlernRessourceDatenbank {
	+Modulname
	+Upvotes
	+Downvotes
}

Kurs --> SelbstlernRessourceGithub
Kurs --> SelbstlernRessourceDatenbank
```

## Beispiel-Daten

## Ablauf-Diagramm

