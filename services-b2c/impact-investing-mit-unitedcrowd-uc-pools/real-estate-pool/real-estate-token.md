# Real Estate Token

Real Estate Token ist ein Pool-Token, der einen Anteil am Real Estate -Pool darstellt. Impact-Investoren können Stablecoins im Real Estate Pool hinterlegen, die zur Finanzierung von Immobilienprojekten und zur Hinterlegung ihrer Liquidität in DeFi-Protokollen auf Basis von Stablecoins verwendet werden. Jeder Impact Investor des Real Estate Pool erhält Real Estate Pool Token, die seinen Anteil am Pool repräsentieren. Der Preis des Immobilien-Tokens wird anhand der Bewertungsformel berechnet.

Es wird erwartet, dass Real Estate Token für Impact-Investoren eine durchschnittliche Rendite von 9 - 13% bieten. Die Rendite wird durch die tokenisierten Kredite an Projektkoordinatoren und die zusätzliche Liquidität für DeFi-Protokolle generiert.

Darüber hinaus haben Inhaber von Real Estate Token die Möglichkeit, diese in UC Pool Vaults zu investieren und erhalten einen potenziell deutlich höheren APY \(je nach UC Token Preis\).

Der Real Estate-Token hat die folgenden Eigenschaften:

* Es gibt keine Dividendenausschüttungen. Der Wert des Pools steigt durch auto-compounding und damit auch der Real Estate -Token-Preis.
* Der Preis des Real Estate -Tokens wird basierend auf der Bewertungsformel berechnet.
* Es gibt keinen maximalen Supply an Real Estate Token. Real Estate -Token werden für jede neue Einzahlung gemintet und bei jeder Auszahlung von Deposit Token von verbrannt.
* Der Marktpreis kann vom internen Real Estate -Token-Preis abweichen.

### **Bewertungsformel**

Der Real Estate Token repräsentiert einen Anteil des Real Estate Pools. Daher hängt der Wert des Real Estate -Tokens von der Bewertung des Real Estate Pools ab.

Aufgrund der verfügbaren Liquiditätsreserve gibt es eine maximale Anzahl an Real Estate Token, die Anleger einlösen können. Die folgende Formel wird verwendet, um den Wert des Pools, den Wert eines Anteils und die maximale Anzahl einlösbarer Token zu berechnen.

In zukünftigen Versionen des Real Estate Pools können Impact-Investoren Token auch dann zurückgeben, wenn die Liquiditätsreserve erschöpft ist \(siehe Roadmap\).



$$
UC_{fund} = UC_{Liquidität}+\sum_{ }Projekt_{Investment}-\sum_{ }Projekt_{Tilgung}
$$

$$
UC_{share} = \frac{UC_{fund}}{UC_{supply}}
$$

In den nächsten Abschnitten werden wir einige praktische Beispiele für den Kauf und das Einlösen von Real Estate -Token durchgehen.

### Einzahlung

Impact-Investoren können Real Estate Tokens direkt über den UC Pool erwerben. Der ermittelte Anteilswert basiert auf der Berechnung des Real Estate Pool Value. Es kann eine Einzahlgebühr anfallen.

#### **Beispiel 1**

100 Investoren haben jeweils 1.400 US-Dollar in den Real Estate Pool investiert, und es wurden 0 Projekte umgesetzt. Alice möchte 5 Aktien des Immobilienfonds kaufen.

```text
Liquidity Reserve: 100 * $1.400 = $140.000
Real Estate Token Supply: 100 Real Estate Tokens
Investiert in Projekte: $0
Projekt Rückzahlungen: $0
Wert des Real Estate Pools: $140.000 + 0 - 0 = $140.000
Wert der Real Estate Token: $140.000/100 = $1.400
```

Alice zahlt 7.000 $ \(5 \* 1.400 $\), um 5 Real Estate -Token zu erhalten. Der Liquiditätsreserve werden 7.000 US-Dollar hinzugefügt. Insgesamt werden 5 neue Real Estate -Token geprägt.

#### **Beispiel 2**

Bob will nach Alice 100 Dollar in den Real Estate Pool investieren \(siehe Beispiel 1\).

```text
Liquidity Reserve: $140.000 + $7.000 = $147.000
Real Estate Token Supply: 105 Real Estate Tokens
Investiert in Projekte: $0
Projekt Rückzahlungen: $0
Wert des Real Estate Pools $147.000 + $0 - $0 = $147.000
Wert der Real Estate Token: $147.000/105 Real Estate Tokens = $1.400
```

Bob erhält 0,0714285714 Real Estate -Token \(100 $/1.400 $\) für seine 100 $-Investition.

#### **Beispiel 3**

Insgesamt werden 3 Projekte mit einem Investitionskapital von 15.000 USD umgesetzt. Von den Projektkoordinatoren wurden bisher keine Tilgungszahlungen geleistet. Bob möchte 2 Immobilienmarken kaufen.

```text
Liquidity Reserve: $147.100 - $15.000 = $132.100
Real Estate Token Supply: 105,0714285714 Real Estate Tokens
Investiert in Projekte $15.000
Projekt Rückzahlungen: $0
Wert des Real Estate Pools: $132.100 + $15.000 - $0 = $147.100
Wert der Real Estate Token: $147.100/105,0714285714 Real Estate Tokens = $1.400
```

Um 3 Token zu kaufen, muss Bob 4200 $ bezahlen.

#### **Beispiel 4**

Alle drei Projekte in Beispiel 3 lieferten Zahlungen in Höhe von insgesamt 11.000 USD. 1.000 USD der Zahlungen sind Zinsen und 10.000 USD Rückzahlungszahlungen. Alice möchte noch 1 Token kaufen.

```text
Liquidity Reserve: $132,100 + $4,200 = $136,300
Real Estate Token Supply: 108.0714285714 Real Estate Tokens
Invested in projects: $15,000
Projects Redemption Payments: $10,000
Interest payment: $1,000
Value of Real Estate Fund: $147,300 + $15,000 - $10,000 = $152,300
Value of Real Estate Token: $152,300/108.0714285714 Real Estate Tokens = $1,409.25313946
```

Um 1 Real Estate -Token zu kaufen, muss Alice 1409,25 $ bezahlen.

### **Auszahlung \(Real Estate-Token zurückgeben\)**

Impact-Investoren haben die Möglichkeit, ihre Real Estate-Tokens direkt an den UC Pool zurückzugeben. Der Anteilspreis des Pools richtet sich nach der Bewertungsformel. Es kann eine Abhebungsgebühr erhoben werden.

Die Liquiditätsreserve des Real Estate-Pools ist begrenzt. Für den Fall, dass nicht genügend Liquidität in der Liquiditätsreserve vorhanden ist, können Token-Inhaber Real Estate -Token auf dem Sekundärmarkt handeln. Die maximale Anzahl der einlösbaren Real Estate -Token wird durch die Bewertungsformel bestimmt.

In zukünftigen Versionen des Real Estate Fund können Impact-Investoren Token auch bei erschöpfter Liquiditätsreserve einlösen \(siehe Roadmap\)

#### **Beispiel 1**

Mehrere Projekte wurden umgesetzt. Der Wert des Real Estate-Pools beträgt 150.000 USD und die Liquiditätsreserve beträgt 120.000 USD. Der Preis für Real Estate -Token beträgt 1.400 USD und das Token-Angebot beträgt 100 Real Estate -Token. Alice möchte 3 Immobilienmarken zurückgeben.

```text
Real Estate Fund Wert: $150.000
Liquiditätsreserve: $120.000
Der des Real Estate Token: $1.400
Einlösbare Real Estate Tokens: $120.000/$1.400 = 85,7142857 Real Estate Token
```

Aufgrund der gegebenen Liquiditätsreserve können maximal 85.7142857 Real Estate Tokens abgehoben werden. Alice erhält $4200 für ihre 3 Token. Der Wert der Real Estate Tokens wird durch die Auszahlung nicht beeinflusst.

#### **Beispiel 2**

In der gleichen Situation wie im vorherigen Beispiel möchte Bob 90 Token abheben.

```text
Real Estate Fund Wert: $150.000
Liquiditätsreserve: $120.000
Value of Real Estate Token:  $1.400
Einlösbare Real Estate Tokens: $120.000/$1.400 = 85,7142857 Real Estate Tokens
```

Bob kann 85.7142857 Real Estate -Token nur direkt über UnitedCrowd einlösen. Die verbleibende Menge von 4.2857143 Real Estate Tokens könnte er auf dem Sekundärmarkt verkaufen.

Wie in der Roadmap festgehalten, wird es Bob in Zukunft durch ein System auf Basis dynamischer Gebühren und tokenisierter Projektschulden möglich sein, alle seine Anteile auch bei erschöpfter Liquiditätsreserve \(siehe Roadmap\) zurückzukaufen.

### **Gebühren**

Alle Gebühren im Zusammenhang mit Real Estate Token und Real Estate Pool finden Sie hier

