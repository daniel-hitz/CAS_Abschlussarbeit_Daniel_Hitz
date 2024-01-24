# Wer dominiert in den Stadtparlamenten von Wädenswil und Adliswil?
Analyse von über 700 Vorstössen aus den Stadtparlamenten zwischen dem 1. Januar 2006 und dem 31. Dezember 2023.

## 1. Ausgangsthesen
Die lokalen Parlamente bestimmen zu weiten Teilen, was vor den Haustüren der Leserinnen und Leser vor sich geht. Im Einzugsgebiet der Zürichsee-Zeitung liegen die Stadtparlamente Wädenswil und Adliswil. über diese beiden kommunalen Legislativen weiss man eigentlich nur sehr wenig. Die Berichterstattung beschränkt sich auf aktuelle Debatten und Entscheide. Eine längerfriste Analyse über mehrere Legislaturen eines Stadtparlaments hinweg sowie einen Vergleich der beiden Parlamente gibt es noch nicht. Es ist an der Zeit, diese Lücke zu schliessen und die beiden Parlamente und vor allem deren Mitglieder genauer anzuschauen. Es stellen sich mir folgende 5 Fragen und die entsprechenden Thesen.

**1. Welche Parteien und Fraktionen reichen die häufigsten Vorstösse ein?** 
These: In Wädenswil sind es die rechten, in Adliswil die linken Parteien. Folgefrage: Entspricht die Anzahl Vorstösse auch der Fraktionsgrösse und den Wähleranteilen?

**2. Welches sind die erfolgerichsten Fraktionen und wessen Vorstösse werden am meisten abgelehnt?** 
These: Habe ich nicht - Ich lasse mich vom Ergebnis der Daten überraschen.

**3. Welches waren die fleissigsten Parlamentarier/innen?**
These: Es gibt einzelne Politiker*innen, die besonders viele Vorstösse eingereicht haben, andere gar keine. Folgefrage: Haben die "fleissigen" auch Erfolg mit ihren Vorstössen oder beschäftigen sie nur die Behörden?

**4. Wie viele Vorstösse stammen von Männern und wie viele von Frauen?** 
These: Die Männer dominieren. Folgefragen: Bei welchen Fraktionen drängen sich die Männer in den Vordergrund?

**5. Wie sieht ein Vergleich der Stadtparlamente von Wädenswil und Adliswil aus?** 
These: In Wädenswil werden viel mehr Vorstösse eingereicht als in Adliswil. Bei beiden Parlamenten hat die Anzahl der Vorstösse in den letzten Jahren zugenommen.


## 2. Datensatz 
Berücksichtigt wurden die Daten auf den Webseiten der beiden Städte. Es sind über 700 Vorstösse, deren relevante Daten auf über 700 Subseiten enthalten sind. Beücksichtigt werden alle Geschäfte zwischen dem 1.1.2006 und dem 31.12.2023. (https://www.waedenswil.ch/politbusiness / https://www.adliswil.ch/politbusiness). 


## 3. Einschätzung von Aufwand und Ertrag
**Zum Aufwand:** Eine einfache und übersichtliche Zusammenstellung aller Vorstösse der letzten Jahre haben die beiden Städte nicht. Die Daten von den Webseiten zu holen, könnte aufwändig werden. Die beiden Städte haben keinen fertigen Datensatz und die Webseiten der Stadtparlamente sind mit jenem des Zürcher Stadtparlaments oder des Kantonsrates nicht zu vergleichen. Um an die Daten zu kommen, sind Selenium und Beautifulsoup notwendig. Sind die Daten mal da und strukturiert, sollte eine Auswertung aber relativ rasch möglich sein. Um den Aufwand verhältnismässig zu halten, beschränke ich mich auf die Online zugänglichen Geschäfte. Es bestünde natürlich auch die Möglichkeit, im Stadtarchiv sämtliche Vorstösse der letzten 50 Jahre physisch durchzuschauen und die Analyse zeitlich noch weiter auszuweiten. Hier wäre das Verhältnis von Aufwand und Ertrag aber wohl nicht mehr gegeben.

**Zum Ertrag:** Als Regionalzeitung ist es unsere Aufgabe, das politische Geschehen aufzuzeigen. Noch nie gab es jedoch eine vertiefte und längerfristige Analyse, wer sich wie sehr für die Bevölkerung einsetzt (oder die Stadtverwaltungen unnötig beschäftigt). Das Thema wird die Leserinnen und Leser mit Sicherheit interessieren. Zudem können die gewonnenen Daten vor den nächsten Parlamentswahlen einfach aktualisiert und wieder recycelt werden. So dient der Aufwand auch für mehrere Geschichten.

**Das Fazit:** Die Gewinnung der Daten dürfte aufwändig werden, der Ertrag sollte sich aber auch im Hinblick auf künftige Geschichten lohnen.


## 4. Der Knackpunkt
Das Gute und zugeleich das Schlechte ist, dass die Webseiten der beiden Städte exakt gleich aufgebaut sind. Das hilft zwar, weil ich praktisch den identischen Code für beide Webseiten brauchen kann, es ist aber auch unpraktisch, weil die Seiten ziemlich umständlich gestaltet sind. So wird die Seitenzahl beispielsweise nicht über die URL ausgewiesen und beim Aktualisieren der Seiten wird die Reihenfolge der Elemente geändert. Es braucht also ein paar Kniffs mit Selenium, um an die Daten zu kommen.

Die Partei der Parlamentarierinnen und Parlamentarier wird nicht ausgewiesen. Ich muss also entweder anderweitig eine Liste einholen oder diese manuell hinzufügen. Das könnte je nachdem aber schwierig werden, weil viele der Politiker*innen schon lange nicht mehr aktiv sind.

Zudem geht der Datensatz auf den Webseiten nur bis 2005 resp. 2006 zurück und scheint auch nicht vollständig zu sein. Aussagekräftig und vollständig sind die Daten der beiden Parlamente erst ab 2010.

Ein weiterer Knackpunkt ist die unterschiedliche Handhabung beim Einreichen von Vorstössen. Während in Adliswil oftmals einzelne Politiker/innen den Vorstoss einreichen, sind es in Wädenswil ganze Fraktionen. Das ist bei der Auswertung der "fleissigsten Parlamentsmitglieder" sicher zu berücksichtigen.


## 5. Zusammenfassung eines Briefinggesprächs
Im Gespräch mit der Leiterin Parlamentsdienste von Adliswil (Vanessa Ziegler) war zu erfahren, dass die Geschäfte auf der Webseite der Stadt mindestens in den letzten 8 Jahren zuverlässig eingetragen wurden. Auch davor (also bis ca. 2009) sind ihr keine Fehler bekannt, damals hat die Geschäfte aber jemand anderes nachgeführt. Es sei durchaus möglich eine solche Analyse auf den Geschäften der Stadtwebseite abzustützen. Eine übersichtlichere und einfachere Zusammenstellung habe die Stadt Adliswil nicht. Zu beachten ist, dass  in Adliswil nicht immer alle Parlamentarierinnen, die einen Vorstoss unterschrieben haben, auch als Mitunterzeichnende aufgeführt werden. So habe man zum Teil gerade bei älteren Vorstössen auch nicht alle Unterschriften lesen können. Immer ausgewiesen werden aber jene Politiker/innen, die den Vorstoss verfasst und eingereicht haben. Laut Ziegler seien das auch jene, die die Arbeit am Vorstoss hatten. Eine Liste mit allen Parlamentarier/innen und deren Partei der letzten fünf Legislaturen wird mir zugestellt.

Im Gespräch mit Roger Kempf, Leiter Parlamentsdienste in Wädenswil, wurde klar, dass es gewisse politische Instrumente noch nicht so lange gibt, wie ich zurückschauen möchte. Eine dringliche Interpellation gebe es beispielsweise erst seit ein paar Jahren. Das sollte die Analyse aber nicht beeinträchtigen. 
Eine übersichtlichere Darstellung als auf der Webseite mit allen Vorstössen der vergangenen Jahren habe die Stadt Wädenswil nicht. Es gebe höchstens die Geschäftsberichte des Stadtrats, in denen die einzelnen Vorstösse aus dem Paralment erwähnt würden. Diese reichen aber nur bis 2016 zurück. In Wädenswil ist die Situation zudem ein wenig anders als in Adliswil. Hier werden Vorstösse eher selten von 1 bis 2 Personen eingereicht, sondern meistens von ganzen Fraktionen oder Kommissionen. Die einzelnen Fraktionen haben über die letzten Jahre auch geändert. Auch hier werde ich eine Liste mit allen Parlamentsmitgliedern der letzten 5 Legislaturen samt Partei erhalten.

## 6. Aufwandslogbuch
- Sept.23  bis Dez.23: CAS-Kurse
- Nov.23 bis Dez.23: Über Themen gebrainstormt
- 11./12. Dezember: Datenarbeit über Verwaltungs- und Bildungskosten geschrieben - und wegen fehlender Vergleichbarkeit verworfen
- 12.-30.Dezember: Weiter gebrainstormt
- 1. Januar: Webseiten der Stadtparlamente von Wädenswil und Adliswil studiert.
- 2. Januar: File erstellt
- 2. Januar: Fragen und Thesen ausgearbeitet
- 1.-2. Januar: Code zur Beschaffung der Daten geschrieben
- 2. Januar: Code laufen gelassen und Daten von den beiden Webseiten in rund 700 Files gesammelt
- 3. Januar: Mit Beautifulsoup Daten aus den gesammelten Files gezogen
- 3. Januar: Mit Kollegen über Sinn des Projekts gesprochen
- 4. Januar: Letzter Tag am MAZ - Daten geordnet
- ...

## 7. Endprodukt
Die Geschichte wurde bereits publiziert. Sie ist über folgenden Link zu finden: www.zsz.ch
