# Wer dominiert in den Stadtparlamenten von Wädenswil und Adliswil?
Analyse von über 700 Vorstössen aus den beiden Stadtparlamenten zwischen dem 1. Januar 2006 und dem 31. Dezember 2023.

## 1. Ausgangsthesen
Die lokalen Parlamente bestimmen zu weiten Teilen, was vor den Haustüren der Leserinnen und Leser vor sich geht. Im Einzugsgebiet der Zürichsee-Zeitung liegen die Stadtparlamente Wädenswil und Adliswil. über diese beiden kommunalen Legislativen weiss man eigentlich nur sehr wenig. Die Berichterstattung beschränkt sich auf aktuelle Debatten und Entscheide. Eine längerfriste Analyse über mehrere Legislaturen eines Stadtparlaments hinweg gibt es noch nicht. Es ist an der Zeit, diese Lücke zu schliessen und die beiden Parlamente und vor allem deren Mitglieder genauer anzuschauen. Ich habe dafür mehrere Thesen. Es wäre gut möglich, diese in Form eines Listicles oder mehreren Geschichten zu beantworten. So sollte letztlich mindestens eine Geschichte herausschauen, wenn sich eine der Thesen als falsch herausstellen würde. Ich möchte daher folgende 4 Fragen und die entsprechenden Thesen überprüfen:

**1. Welche Parteien reichen am häufigsten Vorstösse ein?**
These: In Adliswil sind es die linken Parteien, in Wädenswil die rechten. Folgefrage: Entspricht die Anzahl Vorstösse auch den Wähleranteilen?

**2. Welches sind die erfolgerichsten Parteien und wessen Vorstösse werden am meisten abgelehnt?**
These: In Adliswil scheitert die SP und in Wädenswil die SVP am meisten. Folgefrage: Wie sind die politischen Mehrheiten im Parlament verteilt?

**3. Welches waren die fleissigsten Parlamentarier/innen?**
These: Es gibt einzelne Politiker/innen, die besonders viele Vorstösse eingereicht haben. Folgefrage: Haben die "fleissigen" auch Erfolg mit ihren Vorstössen oder beschäftigen sie nur die Behörden?

**4. Wie viele Vorstösse stammen von Männern und wie viele von Frauen?**
These: Die Männer dominieren. Folgefragen: Bei welchen Parteien drängen sich die Männer in den Vordergrund?


## 2. Datensatz 
Berücksichtigt wurden die Daten auf den Webseiten der beiden Städte. Es sind über 700 Vorstösse, deren relevante Daten auf über 700 Subseiten enthalten sind. Beücksichtigt werden alle Geschäfte zwischen dem 1.1.2006 und dem 31.12.2023. (https://www.waedenswil.ch/politbusiness / https://www.adliswil.ch/politbusiness). 

Der Code für die Datensammlung sind in den Files '1. Datensammlung und Bereinigung Adliswil.ipynb' und '1. Datensammlung und Bereinigung Wädenswil.ipynb'. Die Informationen von den Stadtwebseiten sind in den Ordnern Subpages_Adliswil und Subpages_Wädenswil gespeichert. Die bereinigten CSV-Daten der Webseiten sowie weitere Datensätze im Ordner All_Datas. In den Files "2. Auswertung Adliswil" und "2. Auswertung Wädenswil" sind die Codes und Grafiken für die Auswertungen.


## 3. Einschätzung von Aufwand und Ertrag
**Zum Aufwand:** Eine einfache und übersichtliche Zusammenstellung aller Vorstösse der letzten Jahre haben die beiden Städte nicht. Die Daten von den Webseiten zu holen, könnte aufwändig werden. Die beiden Städte haben keinen fertigen Datensatz und die Webseiten der Stadtparlamente sind mit jenem des Zürcher Stadtparlaments oder des Kantonsrates nicht zu vergleichen. So wird die Seitenzahl beispielsweise nicht über die URL ausgewiesen und beim Aktualisieren der Seiten wird die Reihenfolge der Elemente geändert. Es braucht also ein paar Kniffs mit Selenium, um an die Daten zu kommen. Sind die Daten mal da und strukturiert, sollte eine Auswertung aber relativ rasch möglich sein. Um den Aufwand verhältnismässig zu halten, beschränke ich mich auf die online zugänglichen Geschäfte. Es bestünde natürlich auch die Möglichkeit, im Stadtarchiv sämtliche Vorstösse der letzten 50 Jahre physisch durchzuschauen und die Analyse zeitlich noch weiter auszuweiten. Hier wäre das Verhältnis von Aufwand und Ertrag aber wohl nicht mehr gegeben. In der gewählten Form rechne ich mit einem Aufwand von rund 40 Stunden für die Geschichte und 10 Stunden für die Dokumentation.

**Zum Ertrag:** Als Regionalzeitung ist es unsere Aufgabe, das politische Geschehen aufzuzeigen. Noch nie gab es jedoch eine vertiefte und längerfristige Analyse, wer sich wie stark im Parlament einsetzt. Zudem können die gewonnenen Daten vor den nächsten Parlamentswahlen mit sehr wenig Aufwand aktualisiert und recycelt werden.

**Das Fazit:** Die Gewinnung der Daten dürfte aufwändig werden, der Ertrag sollte sich aber auch im Hinblick auf künftige Geschichten lohnen.


## 4. Die Knackpunkte

Die Partei der Parlamentarierinnen und Parlamentarier wird bei den Vorstoss-Informationen auf den Webseiten nicht ausgewiesen. Ich bin also darauf angewiesen, dass ich diese Informationen von den Städten Adliswil und Wädenswil erhalte. Ansonsten müsste ich aufwändig via Googlesuche oder archive.org die Parteien von längst nicht mehr aktiven Politiker/innen ausfindig machen. Das würde Tage dauern und den Aufwand wohl nicht mehr rechtfertigen.

Wenn die Informationen auf den Webseiten der beiden Städte grobe Lücken aufweisen oder falsch sind, könnte die Geschichte in sich zusammenbrechen. Ich muss möglichst früh mit Stichproben und Briefinggesprächen herausfinden, ob diese Daten eine Analyse erlauben.

Wenn es kaum unterschiede zwischen den Parteien beim Einreichen von Vorstössen gibt, könnte die Geschichte langweilig werden. Das finde ich aber erst nach einer tieferen Analyse heraus. Eine der 4 verschiedenen Fragestellungen sollte aber auch dann eine (andere) Geschichte möglich machen.

## 5. Zusammenfassung der Briefinggespräche
Im Gespräch mit der Leiterin Parlamentsdienste von Adliswil (Vanessa Ziegler) war zu erfahren, dass die Geschäfte auf der Webseite der Stadt mindestens in den letzten 8 Jahren zuverlässig eingetragen wurden. Auch davor (also bis ca. 2009) sind ihr keine Fehler bekannt, damals hat die Geschäfte aber jemand anderes nachgeführt. Es sei durchaus möglich eine solche Analyse auf den Geschäften der Stadtwebseite abzustützen. Eine übersichtlichere und einfachere Zusammenstellung habe die Stadt Adliswil nicht. Man könnte höchstens alle Vorstösse im Archiv physisch einsehen. Zu beachten ist, dass in Adliswil nicht immer alle Parlamentarierinnen, die einen Vorstoss unterschrieben haben, auch als Mitunterzeichnende aufgeführt werden. So habe man zum Teil gerade bei älteren Vorstössen auch nicht alle Unterschriften lesen können. Immer ausgewiesen werden aber jene Politiker/innen, die den Vorstoss verfasst und eingereicht haben. Laut Ziegler seien das auch jene, die die Arbeit am Vorstoss hatten. Eine Liste mit allen Parlamentarier/innen und deren Partei der letzten fünf Legislaturen wird mir zugestellt.

Im Gespräch mit Roger Kempf, Leiter Parlamentsdienste in Wädenswil, wurde klar, dass es gewisse politische Instrumente noch nicht so lange gibt, wie ich zurückschauen möchte. Eine dringliche Interpellation gebe es beispielsweise erst seit ein paar Jahren. Das sollte die Analyse aber nicht beeinträchtigen. 
Eine übersichtlichere Darstellung als auf der Webseite mit allen Vorstössen der vergangenen Jahren habe auch die Stadt Wädenswil nicht. Es gebe höchstens die Geschäftsberichte des Stadtrats, in denen die einzelnen Vorstösse aus dem Paralment erwähnt würden. Diese reichen aber nur bis 2016 zurück. Alles davor müsste im Stadtarchiv angesehen werden. In Wädenswil ist die Situation zudem ein wenig anders als in Adliswil. Hier werden Vorstösse eher selten von einzelnen Personen eingereicht, sondern meistens von ganzen Fraktionen oder Kommissionen. (Anm.: Eine Auswertung nach einzelnen Parlamentsmitgliedern ist zwar möglich, das System im Wädenswiler Parlament muss aber transparent gemacht werden). Auch hier werde ich eine Liste mit allen Parlamentsmitgliedern der letzten 5 Legislaturen samt Partei erhalten.

## 6. Aufwandslogbuch
- Sept. 23  bis Dez. 23: CAS-Kurse
- Nov.23 bis Dez.23: Über Themen gebrainstormt
- 11./12. Dezember: Erste Arbeit über Verwaltungs- und Bildungskosten angefangen - und wegen fehlender Vergleichbarkeit verworfen
- 12.-26.Dezember: Weiter nach Themen gesucht
- 27. Dezember: Webseiten der Stadtparlamente von Wädenswil und Adliswil studiert. (2h)
- 28. Dezember: Fragen und Thesen ausgearbeitet und mir überlegt, wie ich damit eine relevante Geschichte erzählen könnte (2h)
- 29. Dezember: Mit Stichproben die Vollständigkeit und Genauigkeit der Daten auf den Webseiten geprüft. (2h)
- 29 bis 31. Dezember: Code zur Beschaffung der Daten geschrieben (6h)
- 1. Januar: Code finalisiert und Programm laufen gelassen. Daten von den beiden Webseiten in rund 700 Files gesammelt (1h)
- 3. Januar: Mit Beautifulsoup Daten aus den gesammelten Files gezogen und erste kurze Auswertungen vorgenommen (3h)
- 3. Januar: Briefinggespräche mit Parlamentsleitern von Wädenswil und Adliswil(wegen Weihnachtsferien etwas spät) (1h)
- 3. Januar: Mit Kollegen über Sinn des Projekts gesprochen (1h)
- 4. Januar: Letzter Tag am MAZ - Daten geordnet und Tipps für weitere Schritte eingeholt (8h)
- 8. Januar: Fragen und Thesen angepasst (1h)
- 15. Januar: Daten kritisch hinterfragt - Grundsätzlich sind die Daten korrekt. Es gibt ein paar NaN Dateien, die noch angepasst werden müssen. (1h)
- 16. Januar: Daten bereinigt (5h)
- 24. Januar: Repository erstellt und alles ins Github transferiert (2h)
- 25. Janaur: Readme geschrieben (2h)
- 28. Januar: csv-File mit Parlamentariern bereinigt und eingelesen. Dataframes für Auswertung vorbereitet und ausgewertet, welche Partei wie viele Vorstösse eingereicht hat. (6h)
- 29. Januar: Weitere Auswertungen zu Parteien gemacht, Parteistärke berechnet, Geschlechterquote ausgewertet und diverse Grafiken erstellt. (5h)
- 30. Januar: Weitere Auswertungen zu Erfolg und Misserfolg der Parteien (4h)
- 3. Februar: Auswertungen Adliswil abgeschlossen und Auswertungen Wädenswil sowie Datensätze für Wädenswiler Parlamentarier und Parteistärken erstellt. (3h)
- 4. Februar: Auswertungen für Wädenswil adaptiert (2h) / Fazite aus den einzelnen Analysen gezogen und Besonderheiten für die Geschichte(n) gesucht. (1h)
- 8. Februar: Titel, Lead und Storyline für Geschichte Adliswil geschrieben (3h)
- 9. Feburar: Titel, Lead und Storyline für Geschichte Wädenswil geschrieben (1h)
- 10. Februar: Letzte Kontrolle vor der Abgabe (1h)



**Aufwand in Stunden:**
Thesen formulieren und brainstormen: 5h
Datenbeschaffung: 14h 
Daten auswerten: 17h
Grafiken erstellen: 5h
Geschichte schreiben: 4h
Dokumentation: 5h
Total: ca. 50h


## 7. Endprodukt
Titel, Lead, Storyline, Grafiken und Skizze des weiteren Vorgehens sind in den Dateien "Story_Adliswil" und "Story_Wädenswil" im Repository.
