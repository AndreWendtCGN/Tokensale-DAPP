# Tokenization Framework

Mit dem Tokenization Framework können digitale Finanzprodukte – beispielsweise zur Unternehmensfinanzierung – herausgegeben werden. 

Dabei lassen sich sowohl bestehende Finanzprodukte wie Wertpapiere, Vermögensanlagen, Investmentfonds etc., als auch Sachwerte und neue Finanzierungsmodelle abbilden. Das Framework ermöglicht es, Finanzprodukte auf Basis von Blockchain-Technologie zu modellieren und über intelligente, templatebasierte Vertragsmuster, sogenannte Smart Contracts zu automatisieren und in Form von Token abzubilden. In enger Zusammenarbeit mit internationalen Regulierungsbehörden werden alle Verträge auf die Einhaltung landesspezifischer Vorschriften validiert und sind regulationskonform. Damit ein Token seinen Bestimmungszweck erfüllen und alle Stakeholder zusammenbringen kann, müssen verschiedene Prozesse dynamisch ineinandergreifen und dabei unterschiedliche Instanzen mit eigenen Zugriffsrechten einräumen.

Zusätzlich ist das Framework auch auf andere Blockchains adaptierbar, um bei möglichen regulatorischen oder technischen Veränderungen reagieren zu können.

![](../../.gitbook/assets/grafik%20%2840%29.png)

### **Framework Architektur**

**Das dem Framework zugrunde liegende 3-Layer-Modell separiert die Teilaufgaben des Netzwerkes und die Zugriffsmöglichkeit von Rechteinhabern auf verschiedene Instanzen. Der Zugriff wird hier allen Rolleninhabern restriktiv nach Ausübungsfunktion sowohl über API als auch über das Frontend und Regulatoren über Direktzugriff gewährt.**

![](https://i1.wp.com/unitedcrowd.com/wp-content/uploads/2020/03/Technische-Spezifikationen-V2-2-2.png?resize=1080%2C698&ssl=1)

### **Zugriff nach Instanzen**

_Issuing_  
Das Initiieren von Verträgen und die damit verbunden Tokenausgabe unterliegt einzig dem Issuer und dem von ihm beauftragten Administrator, dem die technische Umsetzung der Ausgabe zufällt. Die Zugriffsberechtigung der Ausgabe ist über den Settlement Layer sowohl über den API-Zugriff als auch über das Frontend gegeben. Die Überwachung der Regularien und Ausgabebedingungen \(Compliance und Validation\) erfolgt für den Issuer und seine Administration ebenso über das Frontend, wie auch die Daten-Akkumulation über den Service Layer.

_Investing_  
Die Investing-Instanz erklärt seine Vertragsinhaberschaft und der damit verbunden Token Emission über das Frontend auf der Contract Ebene. Die dem Vertrag zu Grunde liegenden Compliance und Validation Regeln lassen sich über das Frontend ebenso einsehen, wie Vertrags- und Verlaufsdaten über den Service-Layer.

_Custody_  
Um die Transaktionsfähigkeit für die Verwahrung sicherzustellen, wird der Zugriff auf den Settlement-Layer benötigt. Die Einhaltung der hohen Sicherheitsstandards und der Regel-Konformität seitens der Regulierungsbehörden kann durch den Zugriff auf den Confidence-Layer gerecht werden. Der Zugriff findet hierbei sowohl über die API als auch über das Frontend statt.

_Exchange_  
Externe Exchange Anbieter benötigen zu Transaktionszwecken den Zugriff auf den Settlement Layer. Um den Marktanforderungen nach Echtzeit-Transaktionen gerecht zu werden, wird der Zugriff über API-Schnittstellen ermöglicht. Der Zugriff für externe Exchanges ist zwingend und wird ebenso wie die Verfolgung der Verlaufsdaten zu Zwecken der Daten-Akkumulation und Statistik über API-Schnittstellen gelöst.

_Delegation_  
Das Delegieren bezieht sich auf das teilweise und zusätzliche Abtreten der Governance zur Anpassung der Regelkonformität durch Vertragspartner. Das zur Delegation bestimmte Committee wird über Smart Contract Ebene demokratisch gewählt, hat eine durch das Netzwerk übertragene Kontrollfunktion und in seiner Funktion einen Lesezugriff auf den Settlement Layer sowie Zugriff auf den Confidence Layer.

_Regulator_  
Der Zugriff von Regulatoren erfolgt als Direktzugriff auf die „Real World Verträge“. Dies ist aufgrund des regulierenden Freigabezwangs unabdinglich.

### **Layer und Komponenten**

**Unterschiedliche Anforderungen von Neuemissionen werden innerhalb des Frameworks über verschiedene Komponenten abgebildet und in Layern organisiert.**

![](https://i2.wp.com/unitedcrowd.com/wp-content/uploads/2020/03/Firmenkonstrukt-Company-cut.jpg?resize=1080%2C436&ssl=1)

_Settlement Layer_  
Der Settlement Layer beinhaltet alle On-Chain-Elemente des Frameworks. Dort werden Assets über Smart Contracts automatisiert und als Token initialisiert. Unterschiedliche Finanzinstrumente stellen jeweils eigene Anforderungen an den Token und werden je nach Produkt in verschiedene Tokenklassen unterschieden. Der Settlement Layer bildet weiterhin die Grundlage der Preisberechnung auf Basis statistischer Preismodelle, die das Risiko, die Dividendenzahlung, die Marktbedingungen und andere Elemente berücksichtigen, die für jeden Token eindeutig sind. Außerdem werden Risikominderungsmechanismen über Absicherungsprotokolle bereitgestellt, welche für verschiedene Modelle gegen das Ausfallrisiko notwendig sind.

_Confidence Layer_  
Der Confidence Layer organisiert die Regelkonformität und Datenvalidierung und definiert Strukturen und Prozesse um sicherzustellen, worunter rechtsverbindliche und ethische Regeln fallen können. Das Validieren der Einhaltung gesetzlicher und finanztechnischer Regularien ist dabei die zentrale Anforderung, die sowohl eine flexible Reaktionsfähigkeit, als auch den Schutz der Rechteinhaber zum Ziel hat. Konsistente Identitätsprotokolle für die Erfassung von Personen-Daten der Emittenten, Anleger und Unternehmen sind unerlässlich und gesetzlich vorgegeben. Das Sicherstellen der Besitzrechte an Token und deren eventueller Übertragung, sowie das Anpassen neuer gesetzlicher Vorschriften ist sowohl in zentralisierter Form durch den Issuer, als auch in Form von „Distributed Governance“ durch die Stakeholder möglich. Konsensprotokolle sind der Schlüssel zur Vergabe von Rechten, deren Übertragung durch Autorisierungsmechanismen ermöglicht wird und die Abstimmungs- und Steuerungsdynamik und die repräsentative, durch Abstimmung entstandene Rechte-Übertragung möglich macht.

_Service Layer_  
Der Service Layer stellt Schnittstellen zur Off-Chain-Kommunikation bereit. Der Datenaustausch findet über Oracles und DAPPs statt, welche die Kommunikation über das Frontend sicherstellen und in kommunikativen Funktionen für alle Rolleninhaber lediglich lesende Rechte verteilen oder Steuerungsfunktionen erhalten. Als Schlüsselkomponente für das Bereitstellen von Off-Chain-Werten stellt ein solider „Data Intelligence-Layer“ eine Schnittstelle für Analysen und Informationen bereit. Neben KYC/AML-Bestimmungen können unterschiedliche Off-Chain-Daten- oder Compliance-Modelle für verschiedene Assets bereitgestellt werden.

### **Emission von Token**

**Die Einhaltung gesetzlicher Rahmenbedingungen und Regulierungsmechanismen werden sowohl Off-Chain, als auch On-Chain gewährleistet.**

**Prüfung des Emittenten**

Bevor UnitedCrowd ein digitales Finanzprodukt erstellt, prüfen wir den Emittenten anhand fester Parameter, die abgefragt und bewertet werden. Dazu zählen beispielsweise eine Due Diligence, Governance und Sicherheit des Unternehmens, aber auch das Management, das unter anderem eine Standardprüfung und eine Hintergrundprüfung der Integrität und des Reputationsrisikos durchläuft.

**Wahl der Finanzierungsart**

Sind die Voraussetzungen erfüllt und wir von der Tragfähigkeit des Projektes überzeugt, so folgt im zweiten Schritt die Entscheidung über die Finanzierungsart. Mit dem Tokenization Framework können verschiedene Werte mit allen in ihnen enthaltenen Rechten und Pflichten digitalisiert werden. Je nach Voraussetzungen und Zielen eines Unternehmens können sich die verschiedenen Varianten unterschiedlich gut eigenen.

Folgende Klassifizierungen sind dabei relevant:

_Asset Token \(Vermögenswerte\)_  
Sowohl liquide, aber auch illiquide Werte lassen sich als Form von Tokenized Securities in Asset Token abbilden. Sie können so in digitales und anteiliges Fractional Ownership \(Teilhaberschaft\) überführt und einem internationalen Markt zugänglich gemacht werden. Die Bandbreite umfasst von Bargeld, Bargeldäquivalenten, Sparkonten über Immobilien, Edelmetallen oder Kunstobjekten alles bis hin zu immateriellen Werten wie Patenten, Urheber- oder Markenrechten.

_Equity Token \(Beteiligungsrechte\)_  
Rechte an Beteiligungen können mit der Vergabe von Anteilen an einem Unternehmen und Stimmrechten in Equity Token abgebildet werden. Nach dem gleichen Prinzip können Token-Anteile an Fonds darstellen.

_Debt Token \(Forderungsrechte\)_  
Debt Token sind Token die Fremdkapitalforderungen auf Rückzahlung des investierten Betrags mit oder ohne Zinsen repräsentieren. Die Bandbreite umfasst dabei Formen von Anleihen, Darlehen und Schuldverschreibungen.

_Utility Token \(Services und Nutzungsrechte\)_  
Utility Token repräsentieren Nutzungsrechte und können beispielsweise dazu verwendet werden, als Community Token Zugang zu einem Netzwerk zu gewähren oder die vom Aussteller des Tokens angebotenen Waren oder Dienstleistungen zu erhalten.

**Regulation und Vertragsausstattung**

Mit der Wahl der Finanzierungsart wird gleichzeitig über den „Real-World-Vertrag“ entschieden, der durch einen Token digital auf der Blockchain abgebildet wird. In diesem Vertrag werden die Rechte und Pflichten definiert. Dabei sind im Einzelnen regulatorische Vorschriften zu beachten und damit geht auch die rechtliche Einstufung einher. Ausgehend von regulationskonformen Standardverträgen wird in diesem Schritt durch Eingabe spezifischer Parameter der individuelle Vertrag modelliert, der dem herauszugebenden Token zugrunde liegt. Parameter sind zum Bespiel der Name des Token, sein Nenn- und Nettowert, Stückelung, eine eventuelle Verzinsung und das Datum der Fälligkeit. Aber auch Geschäftszweck, Jahresabschluss, Marktrisiko, Verschuldungsgrad, Name, Adresse und Handelsregistereintrag des Emittenten.

In Frage kommen dabei insbesondere:

* _VermAnlG \(Vermögensanlagegesetz\)_
* _KWG \(Kreditwesengesetz\)_
* _WpPG \(Wertpapierprospektgesetz\)_
* _KAGB \(Kapitalanlagegesetzbuch\)_

**Emission und Berechtigungen**

Sind alle Parameter des Vertrages festgelegt und eindeutig definiert, kann der Token herausgegeben werden. Der Token muss die Berechtigungen zum Erwerb entweder über einen Off-Chain-Validator oder auf Smart-Contract-Ebene über relevante KYC/AML-Bestimmungen berücksichtigen. Er darf außerdem nur an validierte oder auf der Whitelist stehende berechtigte Adressen übertragen werden, die mit einer Entität verknüpft sind. Während schon akkreditierte Nutzer nicht akkreditiert sein müssen, muss der Token die Investorenakkreditierung bei neuen Nutzern berücksichtigen. Da internationale Kunden zugelassen sind, müssen Berechtigungen enthalten sein, die sich auf den Ort beziehen, an dem der Nutzer ansässig ist. Weiterhin muss der Token die Anzahl der Eigner angeben, wenn dies für das Finanzinstrument relevant ist. Investoren können ihn dann durch Zeichnung über eine elektronische Signatur und Zahlung des Anlagepreises erwerben. Alles was sie hierfür benötigen, finden sie innerhalb seines Accounts auf unserer Plattform. Unter einer elektronischen Signatur versteht man dabei eine verifizierte digitale Identität, welche den Unterzeichner bzw. Signaturersteller identifiziert und die Integrität der signierten elektronischen Informationen prüft.

\*\*\*\*

