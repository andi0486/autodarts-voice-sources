# Datenschutzerklärung

Für die Browser-Erweiterung Autodarts plugin by RA · Beta2.7.22. Stand: 15. November 2026.

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

Die Einstellungen bieten die Bereiche Galerie, Namensansage, Diagnose und Erweitert. Du kannst die Galerieerfassung deaktivieren und die Galerie leeren, automatische Uploads ausschalten, Diagnosearten wählen oder die lokale Namensansage deaktivieren. In der Stimmenverwaltung lassen sich bekannte alte Pakete und der erhaltene frühere Namenscache bewusst getrennt entfernen; Schlüssel bleiben dabei erhalten. Eine Deinstallation kann abhängig vom Browser lokale Erweiterungsdaten und Schlüssel entfernen. Vorhandene Profilsicherungen und Cloudarchive werden dadurch nicht automatisch gelöscht.

### Lokale Stimmen und öffentliche Sprachpakete

Die Spielernamenansage ist standardmäßig aus. Nach ausdrücklicher Aktivierung spricht sie ausschließlich den Namen des bestätigten aktuellen Spielers einschließlich des eigenen Namens. Zur Auswahl stehen zehn freiwillig installierte Supertonic3-Profile und Microsoft-Stimmen, die der Browser tatsächlich als lokal installiert anbietet. Die Erweiterung verarbeitet die Namen für diese Ansagen lokal und überträgt sie nicht an einen Sprachdienst. Andere Browserstimmen, Piper, Pocket und der frühere Katja-Onlinedienst sind in dieser Version nicht auswählbar. Es gibt keine automatische Ersatzstimme.

Die ausführbaren lokalen Sprachkomponenten liegen im Erweiterungspaket. Erst dein ausdrücklicher Klick lädt die festen Supertonic-Modell- und Profildaten nach erteilter optionaler Websiteberechtigung von Hugging Face und dem bestätigten Download-CDN. Dabei erhalten die Anbieter technisch nötige Verbindungsdaten, etwa IP-Adresse und Browserangaben; die Erweiterung sendet ihnen keine Spielernamen, Matchdaten, Bilder oder privaten Schlüssel. Die kleinen mitgelieferten Andreas-Hörproben lassen sich bewusst ohne Modelldownload oder Sprachdienst abspielen.

Öffentliche Modell- und Profildaten liegen in einem getrennten lokalen Browsercache. Sie gehören nicht zu den verschlüsselten privaten Galerie-, Upload-, Namensaudio- oder Schlüsseldaten. Die bisherige Stimme, Lautstärke und Einwilligungsdaten bleiben bei normalen Updates erhalten. Eine alte, künftig nicht unterstützte Stimme wird sichtbar gesperrt und nicht still ersetzt oder erneut heruntergeladen.

Bereits gespeicherte alte Piper-, Pocket- und Phonemizerquellenpakete bleiben als Altbestände sichtbar und können einzeln nach ausdrücklicher Bestätigung lokal entfernt werden. Ein noch von anderen gespeicherten Profilen oder laufenden Vorgängen benötigter Kern bleibt geschützt. Die Altbestandsentfernung löscht ausschließlich das ausgewählte Paket; alte gemeinsame Kerne benötigen eine eigene bewusste Entfernung, sobald keine Abhängigkeit mehr besteht. Galerie, Schlüssel, Cloudarchive und Browserprofile werden dadurch nicht gelöscht.

Die Namen werden für aktuelle lokale Ansagen vorübergehend im Browser verarbeitet. Für diese Ansagen erzeugte Audiodaten werden nicht dauerhaft als Namensarchiv gespeichert oder an einen Sprachdienst versendet. Es gibt keine automatische Ersatzstimme; andere Autodarts-Caller-Einstellungen werden nicht geändert.

### Optionale Supertonic3-Profile

Supertonic3 ist eine getrennte optionale lokale Stimmenfamilie mit den zehn festen Profilen M1 Alex, M2 James, M3 Robert, M4 Sam, M5 Daniel, F1 Sarah, F2 Lily, F3 Jessica, F4 Olivia und F5 Emily. Kein Profil wird automatisch heruntergeladen oder ausgewählt. Die kleinen mitgelieferten Hörproben sprechen ausschließlich „Andreas“ und können vor der Installation bewusst abgespielt werden, ohne einen Sprachdienst oder Modelldownload auszulösen.

Der gemeinsame Supertonic3-Modellkern umfasst 398.361.202 Bytes und wird einmal gespeichert. Weitere Profile benötigen nur ihre jeweilige kleine JSON-Stildatei. Der Download fester Modell-, Konfigurations-, Zeichenzuordnungs- und Profildaten erfolgt erst nach dem ausdrücklichen Klick und der optionalen Websiteberechtigung von Hugging Face beziehungsweise dem bestätigten Download-CDN. Die Anbieter erhalten dabei technisch nötige Verbindungsdaten, etwa IP-Adresse und Browserangaben; Spielernamen, Kamerabilder, Matchdaten und private Schlüssel werden von der Erweiterung nicht an den Modellhost gesendet. Alle ausführbaren Sprachkomponenten sind im Erweiterungspaket enthalten.

Nach erfolgreicher Installation verarbeitet Supertonic3 den aktuellen Namen vollständig lokal. Dafür sind kein Azure-Konto, externer Sprachdienst oder zusätzlich installierter PC-Helfer erforderlich. Modellkern und Presetprofile sind öffentliche Daten im getrennten Modellcache, nicht private Namensaufnahmen. Sie werden nicht zwischen Browserprofilen synchronisiert. Das Entfernen eines Profils erhält andere installierte oder gerade benötigte Profile; gemeinsame Daten werden erst entfernt, wenn sie kein anderes Profil und kein laufender Vorgang mehr benötigt. Galerie, private Namenscache-Schlüssel, Cloudarchive und die ausdrücklich gewählte Stimme werden dadurch nicht still ersetzt oder gelöscht.

Die Modellgewichte und festen Supertonic3-Presetprofile unterliegen OpenRAIL-M einschließlich ihrer Nutzungsbeschränkungen. Der fremde Beispielcode steht unter MIT. Vollständige Lizenztexte, Herkunft, genaue Revisionen und Änderungen sind unter „Lizenzen und Quellcode“ vor einem Download verfügbar. Diese fremden Bedingungen bleiben von der GPL-Lizenz des eigenen Erweiterungscodes getrennt. Geschwindigkeit, Speicherbedarf sowie Klang und Aussprache hängen vom jeweiligen Gerät und Namen ab; eine positive einzelne Robert-Demo ist keine allgemeine Namen-, Stimmen- oder Plattformabnahme.

### Erhaltener früherer Katja-Namenscache

Der frühere Katja-Onlinedienst ist in dieser Version entfernt und lässt sich auch mit alten gespeicherten Einwilligungen nicht aktivieren. Es werden darüber keine Namen abgerufen, keine Sprachdienstanfragen begonnen und keine alten Audiodaten automatisch nachgesprochen. Die gespeicherten Einwilligungs- und Auswahldaten werden dadurch nicht automatisch umgeschrieben.

Schon vorhandene Katja-Namensaufnahmen können im eigenen privaten Namenscache dieses Browserprofils erhalten bleiben. Sie wurden mit AES-GCM verschlüsselt und über HMAC-Prüfwerte gesucht; ihre eigenen lokalen Profilschlüssel sind von Galerie- und Uploadschlüsseln getrennt. Es erfolgt keine Synchronisierung oder Übertragung dieses Altbestands nach OneDrive. Die Schutzgrenzen bei Zugriff auf den laufenden Browser oder das gesamte Profil bleiben bestehen.

Die Stimmenverwaltung zeigt bei vorhandenem Altbestand ausschließlich lokale Cachezahlen ohne Namen. Nach deiner ausdrücklichen Bestätigung leert sie nur die eigenen alten Audio- und Vorgangsdatensätze. Die zugehörigen Schlüssel bleiben erhalten; Galerie, Stimmwahl, Einwilligungen, Cloudarchive und andere Browserdaten werden nicht verändert. Eine reine Statusabfrage legt keinen neuen Cache an und öffnet keine Schlüssel. Bei unbekanntem Schema oder blockiertem Zugriff wird nichts blind gelöscht. Es gibt keine neue automatische Bereinigung dieser nicht mehr verwendeten Namensaufnahmen; sie können bis zur bewussten Entfernung oder browserseitigen Datenlöschung erhalten bleiben.

### Storeupdates

Ein bewusst vorgemerktes fertiges Chrome-Web-Store-Update wird nach tatsächlicher Beendigung aktiver Matches, Aufnahmen und Uploads übernommen. Dadurch wird keine Capture-/Sprach-/Cloudfunktion aktiviert; Storeprüfung oder Auslieferung werden nicht umgangen.

### Lokale OneDrive-Bediensperre

Die OneDrive-Bedienung ist standardmäßig gesperrt. Die lokale PIN-Freischaltung wird nur in diesem Browserprofil gespeichert und bleibt über Neustarts und normale Updates erhalten. Sie wird weder synchronisiert noch an einen Server gesendet; die eingegebene PIN wird nicht gespeichert. Mit „Entwicklerbereich sperren“ wird die lokale Freischaltung aufgehoben. Bestehende Cloudzugänge, Einstellungen, Wartedaten und Archive werden dadurch nicht gelöscht.

Die Sperre ist eine lokale Bediensperre. Ihr Prüfwert ist Teil des veröffentlichten Erweiterungscodes; gezielte Codeanalyse oder Codeänderungen können sie umgehen. Sie ersetzt keine serverseitige Berechtigungsprüfung. Die OneDrive-Bediensperre ändert keine bestehenden Cloudzugänge, Stimmen oder Einwilligungsdaten. Galerie, History und lokale Namensansage benötigen keine Entwicklerfreischaltung. Widerruf, Status und notwendige Abbruch-/Nachbereinigung bleiben zugänglich.

## 5. Optionale Cloud-Übertragung und Empfänger

Ab Version 2.7.4 wird nach gesonderter Galerieeinwilligung und ausdrücklich gewählter Cloudverbindung, dem Speichern eines automatischen Uploadmodus oder vor einem manuell gestarteten Upload ein eigener Zugang über HTTPS eingerichtet. Es ist kein zusätzlicher Benutzeraccount, keine weitere App und keine einzelne Betreiberfreigabe erforderlich. Installation oder bloßes Laden der Einstellungen registriert noch keinen Zugang. Bestehende gültige Uploadanmeldungen werden weiterverwendet. Ein gesperrter Zugang wird nicht automatisch durch einen neuen ersetzt. Eine bestätigte Registrierung ist noch kein bestandener OneDrive-Schreib-/Lesetest.

Automatische Cloud-Uploads sind standardmäßig ausgeschaltet. Nach gesonderter Aktivierung oder beim ausdrücklich gestarteten manuellen Diagnose-Upload übermittelt die Erweiterung die ausgewählten Daten per HTTPS an den privaten Upload-Dienst bei Railway. Von dort speichert der Dienst die ZIP-Archive in einem vom Betreiber verwalteten Microsoft OneDrive. Menschliche Einsicht in konkrete Diagnoseinhalte zum technischen Support erfolgt nur nach ausdrücklicher Zustimmung für die betreffenden Daten und diesen Zweck oder aufgrund einer konkret anwendbaren Ausnahme, etwa für Sicherheit oder gesetzliche Pflichten. Ein allgemeiner Cloud- oder Diagnoseupload ist keine pauschale Zustimmung zu beliebiger menschlicher Dateneinsicht. Vor einem Supportzugriff werden Empfänger, Daten und Zweck erläutert. Für einen optionalen Wochenbericht kann der Maildienst Resend Dateinamen und OneDrive-Verweise an den Betreiber übertragen. Die Archive werden nicht als öffentliche Galerie bereitgestellt.

Manuelle Diagnosearchive sind auf weniger als 45 MiB beschränkt. Neue Zugänge verwenden getrennte Bereiche im zentralen OneDrive-Ziel. Ein manueller Vorgang ist erst vollständig abgeschlossen, wenn höchstens zehn eigene manuelle Archive im jeweiligen Bereich verbleiben. Ist das Archiv bereits gespeichert und die Bereinigung noch offen, wird dies getrennt gemeldet. Normale Matcharchive werden bei erfüllten Alters- und Anzahlbedingungen bereinigt, frühestens nach 14 Tagen und unter Erhalt von mindestens zehn Archiven. Die Bereinigung ist an entsprechende Servervorgänge gebunden; Dateien können länger gespeichert bleiben. Für bestehende Uploadanmeldungen bleibt die bisherige Ablage bestehen. Zusätzliche Anfrage-, Upload- und Speichergrenzen können die weitere Nutzung anhalten. Eine dauerhafte Sicherung oder unbegrenzte Cloudnutzung wird nicht zugesagt.

Registrierungs- und Sperrdatensätze haben keine automatische Löschfrist. Das Abschalten der Uploadautomatik oder die Deinstallation entfernt weder diese technischen Datensätze noch Cloudarchive. Anfragen zur Löschung dieser Daten und Archive können an die Kontaktadresse gerichtet werden. Ein bewusst gestarteter manueller Upload bleibt auch bei ausgeschalteter Automatik eine gesonderte Entscheidung.

## 6. Rechtsgrundlagen

Die optionale Aktivierung, Diagnose, lokale Spielernamenansage und Cloud-Funktion erfolgt nach Information des Nutzers und gegebenenfalls auf Grundlage einer Einwilligung nach Art. 6 Abs. 1 lit. a DSGVO. Für technische Betriebssicherheit und auf den beschriebenen Zweck beschränkte Fehlerbehandlung kommen berechtigte Interessen nach Art. 6 Abs. 1 lit. f DSGVO in Betracht. Die Verarbeitung von Aufnahmen und Kennungen anderer Matchteilnehmer muss auf eine jeweils einschlägige Rechtsgrundlage gestützt sein; ihre Interessen sind zu berücksichtigen.

## 7. Zweckbindung, Sicherheit und internationale Übermittlung

Die Nutzung der erfassten Daten ist auf die Galerie, die freiwillig gewählte lokale Spielernamenansage, den bewussten Abruf öffentlicher Modell- und Profildaten sowie zugehöriger Lizenz- und Quelleninformationen, die gewählte technische Diagnose und Cloudarchivierung sowie deren erforderlichen Betrieb beschränkt. Wir halten die Limited-Use-Beschränkungen der Chrome-Web-Store-Nutzerdatenrichtlinie ein. Daten werden weder verkauft noch für Werbung, Werbeprofile oder andere nicht offengelegte Zwecke verwendet. Eine Übermittlung erfolgt nur für diese Funktionen oder aufgrund einer anwendbaren, offengelegten Ausnahme.

Die automatische lokale Verschlüsselung schützt die gespeicherten Inhalte gegen das bloße Lesen ihrer verschlüsselten Datensätze. Sie garantiert keinen vollständigen Schutz bei Zugriff auf das gesamte Browserprofil, den laufenden Browser oder einen kompromittierten PC. Chrome und Edge können auf verschiedenen PCs mit ihrem jeweiligen lokalen Profil verwendet werden; lokale Daten und Schlüssel werden dadurch nicht automatisch auf ein anderes Profil übertragen. Die Erweiterung benötigt entschlüsselte Inhalte während der Nutzung. Heruntergeladene Diagnose-ZIPs und an Railway oder OneDrive übertragene Archive erhalten durch diese lokale Speicherverschlüsselung keine zusätzliche Ende-zu-Ende-Verschlüsselung.

Die Übertragung zu Railway erfolgt verschlüsselt über HTTPS. Die Erweiterung verkauft keine Daten, enthält keine Werbung und erstellt keine Werbeprofile. Für die verwendeten Hosting-, Cloud- und Maildienste sowie öffentlichen Downloadhosts kann eine Verarbeitung auch außerhalb des Europäischen Wirtschaftsraums erfolgen; die dort jeweils anwendbaren Übermittlungsmechanismen richten sich nach Anbieter und Infrastruktur. Weitere Informationen können beim Verantwortlichen angefragt werden.

## 8. Rechte betroffener Personen

Nach Maßgabe der DSGVO bestehen insbesondere Rechte auf Auskunft, Berichtigung, Löschung, Einschränkung, Widerspruch und gegebenenfalls Datenübertragbarkeit. Einwilligungen können mit Wirkung für die Zukunft widerrufen werden. Anfragen an [andi0486@gmail.com](mailto:andi0486@gmail.com). Es besteht ein Beschwerderecht bei der [Österreichischen Datenschutzbehörde](https://www.dsb.gv.at/).

## 9. Unabhängiges Projekt

„Autodarts plugin by RA“ ist keine offizielle Erweiterung von Autodarts und wird weder von Autodarts betrieben noch unterstützt. Diese Erklärung wird bei Änderungen der Datenverarbeitung aktualisiert.

Autodarts plugin by RA · 15.11.2026
