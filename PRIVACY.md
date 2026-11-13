# Datenschutzerklärung

Für die Browser-Erweiterung Autodarts plugin by RA · Beta2.7.9. Stand: 13. November 2026.

## 1. Verantwortlicher

Andreas Rosenthal

Stallhofen 259/4

8152 Stallhofen

Österreich

E-Mail: [andi0486@gmail.com](mailto:andi0486@gmail.com)

## 2. Zweck der Erweiterung

Die unabhängige Erweiterung dient der Anzeige von Bildern der gegnerischen Dartboard-Kameras während Online-Matches auf Autodarts Play. Sie erkennt die Zuordnung von lokalem und gegnerischem Board und zeigt ab Version 2.7.5 den aktuellen bestätigten gegnerischen Dreier-Visit mit bis zu neun Kamerabildern. Die nach Spielername sortierbare lokale History enthält im aktuellen Match je eindeutig zugeordnetem Onlinegegner die letzten neun Darts mit bis zu 27 Bildern. Offlinegegner und Gäste am selben lokalen Dartboard werden nicht aufgezeichnet. Sie nutzt bestehende Kamerastreams; sie startet keine eigene Kamera- oder Mikrofonaufnahme. Die Matchüberwachung wird erst nach Aktivierung durch den Nutzer gestartet.

## 3. Verarbeitete Daten

- Autodarts-Matchinformationen, Match-/Wurfzeiten, Spielstatus, Spielernamen, Benutzer- und Boardkennungen zur Erkennung des Gegners und des lokalen Dartboards.

- Bereits vorhandene Dartboard-Kamerabilder für den aktuellen gegnerischen Dreier-Visit mit maximal neun Bildern und die aktuelle Matchhistory je bestätigtem Onlinegegner mit maximal neun Darts/27 Bildern sowie gegebenenfalls für ein gewähltes Diagnosearchiv.

- Zur Zuordnung notwendige Konten- oder Sitzungsinformationen auf der Autodarts-Seite. Anmeldetokens werden nicht bewusst in Galerie- oder Diagnosearchive übernommen.

- Technische Fehler- und Statusereignisse für die Minimaldiagnose. Ausführliche Ereignis-, Kamera- und bereinigte Kommunikationsmetadaten werden nur bei Aktivierung dieser Optionen aufgezeichnet; vollständige Nachrichtentexte sind nicht vorgesehen.

- Bei aktiviertem Cloud-Upload oder manuellem Diagnoseexport: Installationskennung, Zeitstempel, Archivdateien und lokale Zugangsdaten zur Anmeldung beim Server. Ab Version 2.7.4 wird der eigene technische Zugang nach ausdrücklicher Cloudwahl automatisch eingerichtet. Dabei verarbeitet der Server zufällige Registrierungskennungen, kryptografische Prüfwerte, eine eigene Zuordnung, Erstellungszeit, Gültigkeits- und Sperrzustände sowie begrenzte Anfrage-, Upload- und Archivmetadaten (Dateiname, Größe, gegebenenfalls OneDrive-Dateikennung). Der individuelle geheime Zugangswert wird auf dem Server nicht im Klartext gespeichert. Die IP-Adresse kann technisch zur Missbrauchsvermeidung und Anfragebegrenzung verarbeitet werden.

## 4. Lokale Speicherung und Löschung

Die Erweiterung speichert Einstellungen, Einwilligungsstatus, Galerie, Diagnose und gegebenenfalls ausstehende Uploadaufträge lokal im Browser, insbesondere über IndexedDB und Chrome-Speicher. Zusätzliche Diagnoseoptionen sind standardmäßig deaktiviert. Bilddaten werden nicht künstlich in der Qualität reduziert. Ein Wechsel der getrennten Datenrevision kann Galerie-, Diagnose- und Warteschlangendaten zurücksetzen. Ein reiner Versionswechsel löst diesen Reset nicht aus. Der Nutzer kann die Galerie leeren oder die Erweiterung deinstallieren; bereits in OneDrive gespeicherte Archive werden dadurch nicht automatisch gelöscht.

Ab Version 2.7.3 speichert die Erweiterung Galeriebilder, gespeicherte Match- und Diagnoseinhalte, wartende Uploadaufträge und den Uploadschlüssel nach erfolgreich abgeschlossener Umstellung automatisch mit AES-GCM verschlüsselt im jeweiligen Browserprofil. Ein zusätzliches Passwort oder eine weitere App ist dafür nicht erforderlich. Der browserinterne Schlüssel bleibt dauerhaft im betreffenden Profil und wird der Erweiterung nicht als exportierbarer Rohschlüssel bereitgestellt. Einwilligungsstatus und technische Steuerangaben sind von dieser Inhaltsverschlüsselung ausgenommen.

Die neue lokale Verschlüsselung gilt nicht rückwirkend für ältere Versionen, einschließlich 2.7.0. Bei einer noch nicht abgeschlossenen oder fehlgeschlagenen Umstellung können unverschlüsselte Altbestände vorhanden sein. Ein Fehler der lokalen Speicherung wird angezeigt; die Möglichkeit, die Einwilligung zu widerrufen, bleibt erhalten.

Die sichtbare History ist auf das aktuelle Match und je erfasstem Onlinegegner neun Darts begrenzt. Wiederanbinden desselben laufenden Matches erhält dessen Zuordnung; die bisherige Endansicht kann erhalten bleiben. Ein Matchende löscht nicht pauschal Diagnosen, Uploadaufträge oder Cloudarchive. Der Historyzugang aktiviert keine Übertragung und verspricht nicht, sämtliche Historybilder hochzuladen.

Die Spielernamenansage ist standardmäßig aus. Nach ausdrücklicher Aktivierung verarbeitet sie ausschließlich den Namen des bestätigten aktuellen Spielers einschließlich des eigenen Namens vorübergehend lokal im Browser. Zur Wahl stehen bewusst nachinstallierte Offline-Stimmen – Thorsten-rdh, Kerstin, MLS-Sprecher0 sowie Pocket Vera und Azelma – und die hier tatsächlich vorhandenen, ausdrücklich als lokal ausgewiesenen Browserstimmen. Alle ausführbaren Sprachkomponenten sind in der Erweiterung enthalten. Modell-, Tokenizer- und feste Stimmzustandsdaten werden erst auf deinen Klick von Hugging Face beziehungsweise GitHub und deren Download-CDNs geladen; dafür wird die optionale Websiteberechtigung abgefragt. Die Anbieter erhalten die für den Abruf nötigen Verbindungsdaten wie IP-Adresse und Browserangaben, keine Spielernamen, Matchdaten oder Kamerabilder von der Erweiterung.

Die Pocket-Stimmen teilen sich einen gemeinsamen Modelldatensatz, der nicht pro Stimme erneut gespeichert wird. Ihre festen Stimmzustände stammen aus öffentlich lizenzierten Referenzaufnahmen; die Erweiterung bietet keinen Mikrofon-, Stimmenimport- oder Stimmenklonvorgang an. Vor jeder Modellinstallation kannst du eine kleine mitgelieferte Hörprobe mit dem festen Namen „Andreas“ bewusst abspielen. Dafür wird kein Modell heruntergeladen und kein Sprachdienst angesprochen. Die Erzeugung aktueller Spielernamen erfolgt nach der Installation ausschließlich lokal. Sie kann je nach Rechner mehrere Sekunden dauern; eine zu späte oder nicht mehr aktuelle Ansage wird ausgelassen und nicht nachgeholt. Es gibt keine automatische Ersatzstimme.

Vor der Modellinstallation kannst du eine kleine mitgelieferte Hörprobe mit dem festen Namen „Andreas“ bewusst abspielen. Dafür wird kein Modell heruntergeladen und kein Sprachdienst angesprochen. Installierte Modelle und das freiwillig offline gespeicherte große Phonemizer-Quellpaket sind öffentliche Daten in einem getrennten lokalen Browsercache. Sie gehören nicht zu den verschlüsselten privaten Galerie-, Upload- oder Schlüsseldaten. Normale Updates erhalten diese Pakete und deine bisherige Stimmwahl; eine hier fehlende alte Stimme wird angezeigt und nicht still ersetzt. Du kannst Pakete in den Einstellungen entfernen.

Die Offline-Stimmen benötigen nach der Installation keinen externen Sprachdienst und keine zusätzliche Betriebssystemstimme. Stimmwahl und Lautstärke bleiben im Browserprofil. Die Erweiterung speichert oder versendet kein aus Spielernamen erzeugtes Audio und weicht nicht still auf eine Online- oder Standardstimme aus. Sie verändert keine anderen Autodarts-Caller-Einstellungen. Eine bewusste Probe gibt den Ton auf der jeweiligen Spielseite frei. Im Bereich „Lizenzen und Quellcode“ stehen die Lizenz- und Herkunftshinweise. Die eigene Quellenbeilage ist enthalten; das große passende Phonemizer-Quellpaket ist unabhängig von Modell, Einwilligung, PIN und Konto öffentlich bei GitHub herunterladbar. Beim bewussten Quellenabruf erhält GitHub beziehungsweise dessen Download-CDN die technisch nötigen Verbindungsdaten; Spielernamen, Matchdaten und Bilder werden dabei nicht übertragen.

Ein bewusst vorgemerktes fertiges Chrome-Web-Store-Update wird nach tatsächlicher Beendigung aktiver Matches, Aufnahmen und Uploads übernommen. Dadurch wird keine Capture-/Sprach-/Cloudfunktion aktiviert; Storeprüfung oder Auslieferung werden nicht umgangen.

### Lokale OneDrive-Bediensperre

Die OneDrive-Bedienung ist standardmäßig gesperrt. Die lokale PIN-Freischaltung wird nur in diesem Browserprofil gespeichert und bleibt über Neustarts und normale Updates erhalten. Sie wird weder synchronisiert noch an einen Server gesendet; die eingegebene PIN wird nicht gespeichert. Mit „Entwicklerbereich sperren“ wird die lokale Freischaltung aufgehoben. Bestehende Cloudzugänge, Einstellungen, Wartedaten und Archive werden dadurch nicht gelöscht.

Die Sperre ist eine lokale Bediensperre. Ihr Prüfwert ist Teil des veröffentlichten Erweiterungscodes; gezielte Codeanalyse oder Codeänderungen können sie umgehen. Sie ersetzt keine serverseitige Berechtigungsprüfung. Die vorhandene Serverauthentifizierung und Datenverarbeitung bleiben unverändert. Galerie, History und lokale Namensansage benötigen keine Entwicklerfreischaltung. Widerruf, Status und notwendige Abbruch-/Nachbereinigung bleiben zugänglich.

## 5. Optionale Cloud-Übertragung und Empfänger

Ab Version 2.7.4 wird nach gesonderter Galerieeinwilligung und ausdrücklich gewählter Cloudverbindung, dem Speichern eines automatischen Uploadmodus oder vor einem manuell gestarteten Upload ein eigener Zugang über HTTPS eingerichtet. Es ist kein zusätzlicher Benutzeraccount, keine weitere App und keine einzelne Betreiberfreigabe erforderlich. Installation oder bloßes Laden der Einstellungen registriert noch keinen Zugang. Bestehende gültige Uploadanmeldungen werden weiterverwendet. Ein gesperrter Zugang wird nicht automatisch durch einen neuen ersetzt. Eine bestätigte Registrierung ist noch kein bestandener OneDrive-Schreib-/Lesetest.

Automatische Cloud-Uploads sind standardmäßig ausgeschaltet. Nach gesonderter Aktivierung oder beim ausdrücklich gestarteten manuellen Diagnose-Upload übermittelt die Erweiterung die ausgewählten Daten per HTTPS an den privaten Upload-Dienst bei Railway. Von dort speichert der Dienst die ZIP-Archive in einem vom Betreiber verwalteten Microsoft OneDrive. Menschliche Einsicht in konkrete Diagnoseinhalte zum technischen Support erfolgt nur nach ausdrücklicher Zustimmung für die betreffenden Daten und diesen Zweck oder aufgrund einer konkret anwendbaren Ausnahme, etwa für Sicherheit oder gesetzliche Pflichten. Ein allgemeiner Cloud- oder Diagnoseupload ist keine pauschale Zustimmung zu beliebiger menschlicher Dateneinsicht. Vor einem Supportzugriff werden Empfänger, Daten und Zweck erläutert. Für einen optionalen Wochenbericht kann der Maildienst Resend Dateinamen und OneDrive-Verweise an den Betreiber übertragen. Die Archive werden nicht als öffentliche Galerie bereitgestellt.

Manuelle Diagnosearchive sind auf weniger als 45 MiB beschränkt. Neue Zugänge verwenden getrennte Bereiche im zentralen OneDrive-Ziel. Ein manueller Vorgang ist erst vollständig abgeschlossen, wenn höchstens zehn eigene manuelle Archive im jeweiligen Bereich verbleiben. Ist das Archiv bereits gespeichert und die Bereinigung noch offen, wird dies getrennt gemeldet. Normale Matcharchive werden bei erfüllten Alters- und Anzahlbedingungen bereinigt, frühestens nach 14 Tagen und unter Erhalt von mindestens zehn Archiven. Die Bereinigung ist an entsprechende Servervorgänge gebunden; Dateien können länger gespeichert bleiben. Für bestehende Uploadanmeldungen bleibt die bisherige Ablage bestehen. Zusätzliche Anfrage-, Upload- und Speichergrenzen können die weitere Nutzung anhalten. Eine dauerhafte Sicherung oder unbegrenzte Cloudnutzung wird nicht zugesagt.

Registrierungs- und Sperrdatensätze haben keine automatische Löschfrist. Das Abschalten der Uploadautomatik oder die Deinstallation entfernt weder diese technischen Datensätze noch Cloudarchive. Anfragen zur Löschung dieser Daten und Archive können an die Kontaktadresse gerichtet werden. Ein bewusst gestarteter manueller Upload bleibt auch bei ausgeschalteter Automatik eine gesonderte Entscheidung.

## 6. Rechtsgrundlagen

Die optionale Aktivierung, Diagnose und Cloud-Funktion erfolgt nach Information des Nutzers und gegebenenfalls auf Grundlage einer Einwilligung nach Art. 6 Abs. 1 lit. a DSGVO. Für technische Betriebssicherheit und auf den beschriebenen Zweck beschränkte Fehlerbehandlung kommen berechtigte Interessen nach Art. 6 Abs. 1 lit. f DSGVO in Betracht. Die Verarbeitung von Aufnahmen und Kennungen anderer Matchteilnehmer muss auf eine jeweils einschlägige Rechtsgrundlage gestützt sein; ihre Interessen sind zu berücksichtigen.

## 7. Zweckbindung, Sicherheit und internationale Übermittlung

Die Nutzung der erfassten Daten ist auf die Galerie, die freiwillig gewählte lokale Spielernamenansage, den bewussten Abruf öffentlicher Sprach- und Quelldaten, die gewählte technische Diagnose und Cloudarchivierung sowie deren erforderlichen Betrieb beschränkt. Wir halten die Limited-Use-Beschränkungen der Chrome-Web-Store-Nutzerdatenrichtlinie ein. Daten werden weder verkauft noch für Werbung, Werbeprofile oder andere nicht offengelegte Zwecke verwendet. Eine Übermittlung erfolgt nur für diese Funktionen oder aufgrund einer anwendbaren, offengelegten Ausnahme.

Die automatische lokale Verschlüsselung schützt die gespeicherten Inhalte gegen das bloße Lesen ihrer verschlüsselten Datensätze. Sie garantiert keinen vollständigen Schutz bei Zugriff auf das gesamte Browserprofil, den laufenden Browser oder einen kompromittierten PC. Chrome und Edge können auf verschiedenen PCs mit ihrem jeweiligen lokalen Profil verwendet werden; lokale Daten und Schlüssel werden dadurch nicht automatisch auf ein anderes Profil übertragen. Die Erweiterung benötigt entschlüsselte Inhalte während der Nutzung. Heruntergeladene Diagnose-ZIPs und an Railway oder OneDrive übertragene Archive erhalten durch diese lokale Speicherverschlüsselung keine zusätzliche Ende-zu-Ende-Verschlüsselung.

Die Übertragung zu Railway erfolgt verschlüsselt über HTTPS. Die Erweiterung verkauft keine Daten, enthält keine Werbung und erstellt keine Werbeprofile. Für die verwendeten Hosting-, Cloud- und Maildienste kann eine Verarbeitung auch außerhalb des Europäischen Wirtschaftsraums erfolgen; die dort jeweils anwendbaren Übermittlungsmechanismen richten sich nach Anbieter und Infrastruktur. Weitere Informationen können beim Verantwortlichen angefragt werden.

## 8. Rechte betroffener Personen

Nach Maßgabe der DSGVO bestehen insbesondere Rechte auf Auskunft, Berichtigung, Löschung, Einschränkung, Widerspruch und gegebenenfalls Datenübertragbarkeit. Einwilligungen können mit Wirkung für die Zukunft widerrufen werden. Anfragen an [andi0486@gmail.com](mailto:andi0486@gmail.com). Es besteht ein Beschwerderecht bei der [Österreichischen Datenschutzbehörde](https://www.dsb.gv.at/).

## 9. Unabhängiges Projekt

„Autodarts plugin by RA“ ist keine offizielle Erweiterung von Autodarts und wird weder von Autodarts betrieben noch unterstützt. Diese Erklärung wird bei Änderungen der Datenverarbeitung aktualisiert.

Autodarts plugin by RA · 13.11.2026
