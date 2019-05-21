Ziel: Fahrg�ste �ber die G�te der Anschlussp�nktlichkeit informieren und Alternativen anbieten

Szenario 1: Fahrgast m�chte p�nktlich am Endbhf ankommen und wahrscheinliche Anschlussprobleme eliminieren.
Szenario 2: Fahrgast informiert sie �ber wahrscheinliche Anschlussprobleme um sich auf einen raschen Umstieg vorzubereiten.

Idee: Wir bringen die P�nktlichkeit der einzelnen Z�ge der gesuchten Verbindung in Bezug auf die jeweilige Umsteigezeit.
Daraus ergibt es sich eine "Anschlusswahrscheinlichkeit".

Zusatzchallenge: Wetterdaten in die P�nktlichkeit und Vorhersage inkludieren

Dazu ben�tigen wir:
Die P�nktlichkeit eines Zugs im Ankunfts-/Umsteigebahnhof: im aktuellen Scope betrachten wir lediglich die historischen Soll-/Istzeiten 
f�r eine Zugnummer f�r einen Bahnhof, z.B. Railjet160 in Z�rich Hb.

Arbeitsschritte:
1. Auswertung der Soll-Ist-Zeiten der SBB aus https://opentransportdata.swiss/de/dataset/istdaten
2. Auswertung der Soll-Ist-Zeiten der �BB aus einem internen System (Ansprechperson markus.massak@oebb.at)
3. Schweizer Wetterdaten (https://meteo.sbb.ch/) mit SBB-Soll-Ist-Zeiten korellieren

Step-by-Step:

Wir nehmen die Verbindung Wien Praterstern - Bern Wankdorf
R2311		06:48	06:58
Umstieg Wien Hbf 8min
RJX160		07:30	15:20
Umstieg Z�rich Hbf 7min
IC724		15:32	16:28
Umstieg Bern 6min
S2(15263)	16:42	16:45

Wir berechnen anhand der historischen Versp�tungen den Anteil jener Z�ge, die innerhalb/au�erhalb der geplanten Umstiegszeit liegen.
Beispiel Z�rich:
Geplante Ankunft 15:20 + 7min. Umstiegszeit = 15:27 ergibt eine Reserve von 5min. auf Zug IC724
Hat ein historischer Zug RJX160 in Z�rich mehr Versp�tung als unsere 5min. Reserve betr�gt, so gilt er f�r unsere Verbindung als versp�tet. 
Aus dem Anteil der p�nktlichen (<=5min.) und unp�nktlichen (>5min.) historischen Z�ge ergibt sich unsere Anschlusswahrscheinlichkeit.


Ausblick siehe Pr�sentation
