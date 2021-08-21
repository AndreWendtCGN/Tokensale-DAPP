# Yield Farming

UC Staking ermöglicht es regulären DeFI-Investoren, Impact-Investoren zu werden. Beim UC Staking wird die bereitgestellte Liquidität an Yieldaggregatoren \(z. B. Autofarm\) weitergeleitet und 3% der Gewinne werden dem UC Treasury zum Zweck der Entwicklung und des Wachstums der UnitedCrowd zugeführt. UC Treasury investiert außerdem in UC-Fonds, um reale Projekte mit sozialer Wirkung zu unterstützen.

Es gibt auch UC-Core Vaults, die keine Liquidität bereitstellen. Diese Core Vaults bestehen aus Tokens von UnitedCrowd \(z.B. UC Pool Tokens, UC Governance Tokens\). Sie können ein unterschiedliches Verhalten aufweisen \(z. B. Zeitsperre\). Alle Core Vaults werden auf dem Dashboard deutlich angezeigt.

Farmer und Lender erhalten UC-Token \(Governance-Token\) als Belohnung für die Nutzung von UC Staking. Das Liquidity-Mining-Programm endet ungefähr im Februar 2024.

Zusätzliche Einnahmen aus zukünftigen UnitedCrowd DeFi-Produkten können verwendet werden, um das bestehende Liquidity-Mining-Programm zu erweitern.

### **Auto compounding**

UC Staking \(außer Core Vaults\) werden automatisch durch das angegebene Auto-Compounding-Protokoll \(z. B. Autofarm\) zusammengesetzt. Die an UC Staking bereitgestellte Liquidität wird an die angegebenen Auto-Compounding-Protokolle weitergeleitet. Gefarmte Governance-Token \(3rd-Party\) können an UC Treasury weitergeleitet werden.

### **Gebühren**

Für UC-Vaults werden folgende Gebühren erhoben:

| Gebühr | Auf | Höhe |
| :--- | :--- | :--- |
| Einzahlungsgebühr | Einzahlbetrag | Bis zu 0,05% |
| Auszahlungsgebühr | Auszahlungsbetrag | Bis zu 0,2% |
| Beitrag zur sozialen Wirkung | Ertrag | 3% |

Alle Gebühren werden an den UC Treasury geleitet. Der UC Treasury wird letztendlich von der Gemeinschaft verwaltet und verwendet, um in UC-Fonds zu investieren, UC-Token zu kaufen und zu verbrennen und für weitere Operationen, die dem UC-Netzwerk zugutekommen. Um mehr über UC Treasury zu erfahren, klicken Sie hier.

**Einzahlungsgebühr Formel**

Die Formel für die Einzahlungsgebühr stellt sicher, dass bei einem niedrigen Einzahlungs-TVL-Verhältnis die Gebühr höher ist und umgekehrt.



$$
Gebühr_{Einzahlung} = (1-\frac{Einzahlung_{Betrrag}}{Einzahlung_{Betrag}+vault_{tvl}})*0.05
$$



**Auszahlungsgebühr Formel**



$$
Gebühren_{Auszahlung} = \frac{Auszahlung_{Betrag}}{vault_{tvl}}*0.2
$$

Die Formel für die Auszahlungsgebühr stellt sicher, dass bei einem hohen Verhältnis von Auszahlungsbetrag und TVL eine höhere Gebühr erhoben wird und umgekehrt.

 Formeln stehen hier nicht müss zt auch übersetzet werden – in github direkt machen

