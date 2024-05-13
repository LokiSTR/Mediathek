Dieses Projekt stammt aus der Laborphase von SE2 der Universität Hamburg (2024)

Notizen zur Projektplanung:

VomerkWerkzeug
Pro Medium muss gecheckt werden ob es ausgeliehen wurde
	Nein-> Ausleihen und entsprechende Rückmeldung
	Ja-> Checken ob vorgemerkt wurde und entsprechende Rückmeldung
		Nein-> Neue Queue anlegen und entsprechende Rückmeldung
		Ja-> Queue aufrufen, checken ob Queue voll und entsprechende Rückmeldung
			Ja-> Aufnahme in die Queue verweigern und entsprechende Rückmeldung
			Nein-> Aufnahme In die Queue und entsprechende Rückmeldung

VormerkWerkzeugTest
Alle Eigenschaften müssen in einem JUnit-Test bestehen

Vormerkkarte
Muss enthalten:
Eigenschaften:  - _medium:Medium
                - _vormerker:Queue<Kunde>
Methoden:       + istVormerkenMoeglich(Kunde):boolean
                + merkeVor(Kunde kunde, Medium medium)
                + entferneVormerkung(Kunde)
                + gibErstenVormerker():Kunde
                + getMedium():Medium
                + getAll():List<Kunden>


