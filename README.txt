Ziel: Fahrgäste über die Güte der Anschlusspünktlichkeit informieren und Alternativen anbieten

Szenario 1: Fahrgast möchte pünktlich am Endbhf ankommen und wahrscheinliche Anschlussprobleme eliminieren.
Szenario 2: Fahrgast informiert sie über wahrscheinliche Anschlussprobleme um sich auf einen raschen Umstieg vorzubereiten.

Idee: Wir bringen die Pünktlichkeit der einzelnen Züge der gesuchten Verbindung in Bezug auf die jeweilige Umsteigezeit.
Daraus ergibt es sich eine "Anschlusswahrscheinlichkeit".

Zusatzchallenge: Wetterdaten in die Pünktlichkeit und Vorhersage inkludieren

Dazu benötigen wir:
Die Pünktlichkeit eines Zugs im Ankunfts-/Umsteigebahnhof: im aktuellen Scope betrachten wir lediglich die historischen Soll-/Istzeiten 
für eine Zugnummer für einen Bahnhof, z.B. Railjet160 in Zürich Hb.

Arbeitsschritte:
1. Auswertung der Soll-Ist-Zeiten der SBB aus https://opentransportdata.swiss/de/dataset/istdaten
2. Auswertung der Soll-Ist-Zeiten der ÖBB aus einem internen System (Ansprechperson markus.massak@oebb.at)
3. Schweizer Wetterdaten (https://meteo.sbb.ch/) mit SBB-Soll-Ist-Zeiten korellieren

Step-by-Step:

Wir nehmen die Verbindung Wien Praterstern - Bern Wankdorf
R2311		06:48	06:58
Umstieg Wien Hbf 8min
RJX160		07:30	15:20
Umstieg Zürich Hbf 7min
IC724		15:32	16:28
Umstieg Bern 6min
S2(15263)	16:42	16:45

Wir berechnen anhand der historischen Verspätungen den Anteil jener Züge, die innerhalb/außerhalb der geplanten Umstiegszeit liegen.
Beispiel Zürich:
Geplante Ankunft 15:20 + 7min. Umstiegszeit = 15:27 ergibt eine Reserve von 5min. auf Zug IC724
Hat ein historischer Zug RJX160 in Zürich mehr Verspätung als unsere 5min. Reserve beträgt, so gilt er für unsere Verbindung als verspätet. 
Aus dem Anteil der pünktlichen (<=5min.) und unpünktlichen (>5min.) historischen Züge ergibt sich unsere Anschlusswahrscheinlichkeit.


Ausblick siehe Präsentation
