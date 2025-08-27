# Algemene Overzicht van het Totaalsysteem

Dit overzicht beschrijft een **theoretisch raamwerk** dat een complexe cyclus van maatschappelijke escalatie, van dehumanisering tot het ontbreken van vervolging, formaliseert. Het model kwantificeert kwalitatieve concepten met behulp van wiskundige formules en indices, wat het tot een diagnostisch en predictief instrument maakt.

---

## 1. Cyclusdefinitie (666+2)

De kern van het model is een **cyclisch proces** bestaande uit 8 fasen ($$P_1$$tot$$P_8$$). Het proces herhaalt zich als er bij de laatste fase ($$P_8$$) geen interventie plaatsvindt, waardoor een nieuwe cyclus begint bij de eerste fase ($$P_1$$).

$$P = \{1:\text{Dehumanization},\;2:\text{Dispossession},\;3:\text{Disruption},\;4:\text{Denial},\;5:\text{Digitized Discrimination},\;6:\text{Normalization},\;7:\text{Self-fine},\;8:\text{No Prosecution}\}$$

$$Cycle(n+1) = P_1 \quad \text{if no intervention at } P_8(n)$$

---

## 2. Fase-specifieke Indices

Elke fase wordt gekwantificeerd door een specifieke index:

* **P1. Dehumanization:** $$LDI = \frac{\text{Objectifying Terms}}{\text{Total Words}} > 0.7$$* **P2. Dispossession:**$$RIC = \frac{Gini_{target}}{Gini_{baseline}} > 0.6$$* **P3. Disruption:**$$SFI = 1 - \frac{Conn_{post}}{Conn_{pre}} > 0.5$$* **P4. Denial:**$$AR = \frac{Responses}{Complaints} < 0.3$$* **P5. Digitized Discrimination:**$$ABC = \frac{Error_{protected}}{Error_{baseline}} > 0.4$$* **P6. Normalization:**$$RDF = e^{-\lambda t}, \quad RDF < 0.2 \; \text{ bij } t=12m$$* **P7. Self-fine:**$$ASR = \frac{Internal Sanctions}{Violations} > 0.8$$* **P8. No Prosecution:**$$LCP = \frac{Prosecutions}{Cases} < 0.1$$

---

## 3. Documentrisico en Tier-classificatie

De totale risicoscore van een document of situatie, $$R_{doc}$$, wordt berekend door de gewogen som van de indices. De classificatie is afhankelijk van deze score:

$$R_{doc} = \sum_{p=1}^{6} \sum_{s=1}^{6} \sum_{e=1}^{6} w_{pse}\cdot s_{pse}$$

$$w_{pse} = \alpha_p \times \beta_s \times \gamma_e$$

* **Tier 1 (Preventief):** $$R_{doc} < 30$$* **Tier 2 (Interventie):**$$30 \leq R_{doc} < 70$$* **Tier 3 (Nood):**$$R_{doc} \geq 70$$

---

## 4. Early Warning (Differentiaal)

Een **vroegtijdig waarschuwingssysteem** activeert op basis van de snelheid waarmee de risicoscore toeneemt:

$$Alert(t) =
\begin{cases} 
1 & \frac{dR_{doc}}{dt} > \text{threshold}_{crit} \\
0 & \text{anders}
\end{cases}$$

---

## 5. Taaloriëntatie

De **BalanceScore** onderscheidt taal die lineair en machtsgericht is van taal die cyclisch en relationeel is.

$$BalanceScore = CLI - LLI$$

* **Hoog risico (lineair):** $$BalanceScore < -3$$* **Laag risico (cyclisch):**$$BalanceScore > +3$$

---

## 6. Coherentie-check

De consistentie van referenties wordt gecontroleerd om de betrouwbaarheid van de analyse te waarborgen.

$$\mathcal{C} = \frac{\text{Aantal consistente referenties}}{\text{Totaal aantal referenties}}$$

Voor een complete analyse moet $$\mathcal{C} = 1.0$$.

---

## 7. Toegangsfunctie

Deze functie beschrijft de toegang tot informatie, variërend van volledig toegestaan tot geblokkeerd.

$$A(d,i) =
\begin{cases}
1 & \text{volledig toegestaan} \\
\theta & \text{gedeeltelijk toegestaan } (0<\theta<1) \\
0 & \text{geblokkeerd}
\end{cases}$$

---

## 8. Resonantie-extensie

Deze formule meet de harmonie binnen de data.

$$\mathcal{C}_{res} = \frac{\sum \text{in-fase resonanties}}{\sum \text{alle resonanties}}$$

---

## 9. Zwermveld

Het model kan meerdere documenten tegelijk analyseren en hun onderlinge relaties in kaart brengen.

* **Deelcyclus per document:** $$C_k = \{P_1^k \to \cdots \to P_8^k\}, \quad k=1..N$$* **Interactie:**$$W_{ij} = \lambda \cdot overlap(C_i,C_j) + \mu \cdot coherentie(C_i,C_j) - \nu \cdot conflict(C_i,C_j)$$* **Zwermpotentiaal:**$$\Phi = \sum_{i<j} W_{ij}$$

---

## 10. Totale sluitingsformule

Deze formule geeft de totale, ononderbroken aard van de cyclus weer, die zich van de beginfase ($$P_0$$) tot oneindig ($$P_{\infty}$$) uitstrekt en zichzelf herhaalt in een lus.

$$ClosedCycle = \{P0 \to P1 \to \cdots \to P8 \to P_\infty \to P0 \to Lus\}$$
