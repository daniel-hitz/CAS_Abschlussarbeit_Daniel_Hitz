# Wer dominiert in den Stadtparlamenten von Wädenswil und Adliswil?
Analyse von über 700 Vorstössen aus den beiden Stadtparlamenten zwischen dem 1. Januar 2006 und dem 9. Februar 2024.

## 1. Ausgangsthesen
Die lokalen Parlamente bestimmen zu weiten Teilen, was vor den Haustüren der Leserinnen und Leser vor sich geht. Im Einzugsgebiet der Zürichsee-Zeitung liegen die Stadtparlamente Wädenswil und Adliswil. über diese beiden kommunalen Legislativen weiss man eigentlich nur sehr wenig. Die Berichterstattung beschränkt sich auf aktuelle Debatten und Entscheide. Eine längerfriste Analyse über mehrere Legislaturen eines Stadtparlaments hinweg gibt es noch nicht. Es ist an der Zeit, diese Lücke zu schliessen und die beiden Parlamente und vor allem deren Mitglieder genauer anzuschauen. Ich habe dafür mehrere Thesen. Es wäre gut möglich, diese in Form eines Listicles oder mehreren Geschichten zu beantworten. So sollte letztlich mindestens eine Geschichte herausschauen, wenn sich eine der Thesen als falsch herausstellen würde. Ich möchte daher folgende 4 Fragen und die entsprechenden Thesen überprüfen:

**1. Welche Parteien reichen am häufigsten Vorstösse ein?**
These: In Adliswil sind es die linken Parteien, in Wädenswil die rechten. Folgefrage: Entspricht die Anzahl Vorstösse auch den Anzahl Sitzen?

**2. Welches sind die erfolgreichsten Parteien und wessen Vorstösse werden am meisten abgelehnt?**
These: In Adliswil scheitert die SP und in Wädenswil die SVP am meisten. Folgefrage: Wie sind die politischen Mehrheiten im Parlament verteilt?

**3. Welches waren die fleissigsten Parlamentarier/innen?**
These: Es gibt einzelne Politiker/innen, die besonders viele Vorstösse eingereicht haben. Folgefrage: Haben die "fleissigen" auch Erfolg mit ihren Vorstössen oder beschäftigen sie nur die Behörden?

**4. Wie viele Vorstösse stammen von Männern und wie viele von Frauen?**
These: Die Männer dominieren. Folgefragen: Bei welchen Parteien drängen sich die Männer in den Vordergrund?


## 2. Datensatz und Repository
Berücksichtigt wurden die Daten auf den Webseiten der beiden Städte. Es sind über 700 Vorstösse, deren relevante Informationen auf über 700 Subseiten enthalten sind.(https://www.waedenswil.ch/politbusiness / https://www.adliswil.ch/politbusiness) 
In Wädenswil habe ich folgende Geschäftsarten ausgewählt: Anfrage, Dringliche Interpellation, Einzelinitiative, Interpellation, Kleine Anfrage, Motion, Petition, Postulat, Volksinitiatve.
In Adliswil habe ich folgende Geschäftsarten ausgewählt: Anfrage, Dringliches Postulat, Interpellation, Motion, Parlamentarische Initiative, Postulat, Volksinitiative.
Weitere Daten wie die Liste aller Parlamentsmitgliedern seit 2006 und deren Partei sowie die Sitzverteilungen der einzelnen Legislaturen habe ich von den Stadtverwaltungen Wädenswil und Adliswil als Excel erhalten. Daraus habe ich die csv-Dateien erstellt.

Der Code für die Datensammlung sind in den Files '1. Datensammlung und Bereinigung Adliswil.ipynb' und '1. Datensammlung und Bereinigung Wädenswil.ipynb'. Die relevanten Subseiten von den Stadtwebseiten sind in den Ordnern Subpages_Adliswil und Subpages_Wädenswil gespeichert. Die bereinigten CSV-Daten sowie weitere Datensätze sind im Ordner All_Datas gespeichert. In den Files "2. Auswertung Adliswil" und "2. Auswertung Wädenswil" sind die Codes und Grafiken für die Auswertungen. Im PDF Titel, Storylines und weiteres Vorgehen sind die finalen Ergebnisse (Achtung es sind mehr Seiten als nach dem ersten Laden angezeigt werden).


## 3. Einschätzung von Aufwand und Ertrag
**Zum Aufwand:** Eine einfache und übersichtliche Zusammenstellung aller Vorstösse der letzten Jahre haben die beiden Städte nicht. Die Daten von den Webseiten zu holen, könnte aufwändig werden. Die beiden Städte haben keinen fertigen Datensatz und die Webseiten der Stadtparlamente sind mit jenem des Zürcher Stadtparlaments oder des Kantonsrates nicht zu vergleichen. So wird die Seitenzahl beispielsweise nicht über die URL ausgewiesen und beim Aktualisieren der Seiten wird die Reihenfolge der Elemente geändert. Es braucht also ein paar Kniffs mit Selenium, um an die Daten zu kommen. Sind die Daten mal da und strukturiert, sollte eine Auswertung aber relativ rasch möglich sein. Ein Vorteil ist, dass die Seiten von Wädenswil und Adliswil identisch aufgebaut sind. Wenn ich den Code für eine Stadt geschrieben habe, sollte er auch für die andere funktionieren.

Um den Aufwand verhältnismässig zu halten, beschränke ich mich auf die online zugänglichen Geschäfte. Es bestünde natürlich auch die Möglichkeit, im Stadtarchiv sämtliche Vorstösse der letzten 50 Jahre physisch durchzuschauen und die Analyse zeitlich noch weiter auszuweiten. Hier wäre das Verhältnis von Aufwand und Ertrag aber wohl nicht mehr gegeben. In der gewählten Form rechne ich mit einem Aufwand von rund 40 Stunden für die Geschichte und 10 Stunden für die Dokumentation.

**Zum Ertrag:** Als Regionalzeitung ist es unsere Aufgabe, das politische Geschehen aufzuzeigen. Noch nie gab es jedoch eine vertiefte und längerfristige Analyse, wer sich wie stark im Parlament einsetzt. Zudem können die gewonnenen Daten vor den nächsten Parlamentswahlen mit sehr wenig Aufwand aktualisiert und recycelt werden.

**Das Fazit:** Die Gewinnung der Daten dürfte aufwändig werden, der Ertrag sollte sich aber auch im Hinblick auf künftige Geschichten lohnen.


## 4. Die Knackpunkte

Die Partei der Parlamentarierinnen und Parlamentarier wird bei den Vorstoss-Informationen auf den Webseiten nicht ausgewiesen. Ich bin also darauf angewiesen, dass ich diese Informationen von den Städten Adliswil und Wädenswil erhalte. Ansonsten müsste ich aufwändig via Googlesuche oder archive.org die Parteien von längst nicht mehr aktiven Politiker/innen ausfindig machen. Das würde Tage dauern und den Aufwand wohl nicht mehr rechtfertigen.

Wenn die Informationen auf den Webseiten der beiden Städte grobe Lücken aufweisen oder falsch sind, könnte die Geschichte in sich zusammenbrechen. Ich muss möglichst früh mit Stichproben und Briefinggesprächen herausfinden, ob diese Daten eine Analyse erlauben.

Wenn es kaum unterschiede zwischen den Parteien beim Einreichen von Vorstössen gibt, könnte die Geschichte langweilig werden. Das finde ich aber erst nach einer tieferen Analyse heraus. Eine der 4 verschiedenen Fragestellungen sollte aber auch dann eine (andere) Geschichte möglich machen.

## 5. Zusammenfassung der Briefinggespräche
Im Gespräch mit der Leiterin Parlamentsdienste von Adliswil (Vanessa Ziegler) war zu erfahren, dass die Geschäfte auf der Webseite der Stadt mindestens in den letzten 8 Jahren zuverlässig eingetragen wurden. Auch davor (also bis ca. 2009) sind ihr keine Fehler bekannt, damals hat die Geschäfte aber jemand anderes nachgeführt. Es sei durchaus möglich eine solche Analyse auf den Geschäften der Stadtwebseite abzustützen. Eine übersichtlichere und einfachere Zusammenstellung habe die Stadt Adliswil nicht. Man könnte höchstens alle Vorstösse im Archiv physisch einsehen. Zu beachten ist, dass in Adliswil nicht immer alle Parlamentarierinnen, die einen Vorstoss unterschrieben haben, auch als Mitunterzeichnende aufgeführt werden. So habe man zum Teil gerade bei älteren Vorstössen auch nicht alle Unterschriften lesen können. Immer ausgewiesen werden aber jene Politiker/innen, die den Vorstoss verfasst und eingereicht haben. Laut Ziegler seien das auch jene, die die Arbeit am Vorstoss hatten. Eine Liste mit allen Parlamentarier/innen und deren Partei der letzten fünf Legislaturen wird mir zugestellt.

Im Gespräch mit Roger Kempf, Leiter Parlamentsdienste in Wädenswil, wurde klar, dass es gewisse politische Instrumente noch nicht so lange gibt, wie ich zurückschauen möchte. Eine dringliche Interpellation gebe es beispielsweise erst seit ein paar Jahren. Das sollte die Analyse aber nicht beeinträchtigen, ich will ja keine Auswertung zu den einzelnen Vorstossarten machen. 
Eine übersichtlichere Darstellung als auf der Webseite habe auch die Stadt Wädenswil nicht. Es gebe höchstens die Geschäftsberichte des Stadtrats, in denen die einzelnen Vorstösse aus dem Paralment erwähnt würden. Diese reichen aber nur bis 2016 zurück. Alles davor müsste im Stadtarchiv angesehen werden. In Wädenswil ist die Situation zudem ein wenig anders als in Adliswil. Hier werden Vorstösse eher selten von einzelnen Personen eingereicht, sondern meistens von ganzen Fraktionen oder Kommissionen. Auch hier werde ich eine Liste mit allen Parlamentsmitgliedern der letzten 5 Legislaturen samt Partei erhalten.

## 6. Aufwandslogbuch
- 23.09  bis 23.12: CAS-Kurse
- 23.11 bis 23.12: Über Themen gebrainstormt
- 11./12..12: Erste Arbeit über Verwaltungs- und Bildungskosten angefangen - und wegen fehlender Vergleichbarkeit verworfen
- 12.-26.12.: Weiter nach Themen gesucht
- 27.12.: Webseiten der Stadtparlamente von Wädenswil und Adliswil studiert. (2h)
- 28.12.: Fragen und Thesen ausgearbeitet und mir überlegt, wie ich damit eine relevante Geschichte erzählen könnte (2h)
- 29.12.: Mit Stichproben die Vollständigkeit und Genauigkeit der Daten auf den Webseiten geprüft. (2h)
- 29.12 bis 31.12.: Code zur Beschaffung der Daten geschrieben (6h)
- 1.1.: Code finalisiert und Programm laufen gelassen. Daten von den beiden Webseiten in rund 700 Files gesammelt (1h)
- 3.1.: Mit Beautifulsoup Daten aus den gesammelten Files gezogen und erste kurze Auswertungen vorgenommen (3h)
- 3.1.: Briefinggespräche mit Parlamentsleitern von Wädenswil und Adliswil geführt(wegen Weihnachtsferien etwas spät) (1h)
- 3.1.: Mit Kollegen über Sinn des Projekts gesprochen (1h)
- 4.1.: Letzter Tag am MAZ - Daten geordnet und Tipps für weitere Schritte eingeholt (8h)
- 8.1.: Fragen und Thesen angepasst (1h)
- 15.1.: Daten kritisch hinterfragt - Grundsätzlich sind sie korrekt. Es gibt ein paar NaN Dateien zum bereinigen. (1h)
- 16.1.: Daten bereinigt (5h)
- 24.1.: Repository erstellt und alles ins Github transferiert (2h)
- 25.1.: Readme geschrieben (2h)
- 28.1.: csv-File mit Parlamentariern bereinigt und eingelesen. Dataframes für Auswertung vorbereitet und ausgewertet, welche Partei wie viele Vorstösse eingereicht hat. (6h)
- 29.1.: Weitere Auswertungen zu Parteien gemacht, Parteistärke berechnet, Geschlechterquote ausgewertet und diverse Grafiken erstellt. (5h)
- 30.1.: Weitere Auswertungen zu Erfolg und Misserfolg der Parteien (4h)
- 3.2.: Auswertungen Adliswil abgeschlossen und Auswertungen Wädenswil sowie Datensätze für Wädenswiler Parlamentarier und Parteistärken erstellt. (3h)
- 4.2.: Auswertungen für Wädenswil adaptiert (2h) / Fazite aus den einzelnen Analysen gezogen und Besonderheiten für die Geschichte(n) gesucht. (1h)
- 8.2.: Titel, Lead und Storyline für Geschichte Adliswil geschrieben (3h)
- 9.2.: Titel, Lead und Storyline für Geschichte Wädenswil geschrieben (1h)
- 10.2.: Letzte Kontrolle vor der Abgabe und Abgabe (1h)


**Aufwand in Stunden:**
Thesen formulieren und brainstormen: 5h
Datenbeschaffung: 14h 
Daten auswerten: 17h
Grafiken erstellen: 5h
Geschichte schreiben: 4h
Dokumentation: 5h
Total: ca. 50h


## 7. Endprodukt
Titel, Lead, Storyline, Grafiken und Skizze des weiteren Vorgehens sind als PDF 'Titel, Storylines und weiteres Vorgehen.pdf' im Repository.
