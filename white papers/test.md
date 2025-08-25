### **White Paper on Advertising Resonance, Cognitive Health, and the Precautionary Principle**

---

## 0. Notatie (compact)

- $t$: tijd (seconden); $f$: frequentie (Hertz); $\omega = 2\pi f$ (rad/s)
- Vectoren worden vet weergegeven: $\mathbf{s}(t)$, $\mathbf{x}(t)$. Fourier-transformatie: $\mathcal{F}\{\text{functie}\}(f)$
- Tijdsgemiddelde over venster $T$: $\langle \cdot \rangle_T$
- $|\cdot|_2$: kwadratische norm; $|\cdot|$: modulus; $\odot$: elementwise product

---

## 1. Stimulusmodellering (digitaal en analoog, multimodaal)

De advertentiestimulans wordt gemodelleerd als een samengestelde tijdreeks:

$$
\mathbf{s}(t) = 
\begin{bmatrix}
s_{vis}(t) \\
s_{aud}(t) \\
s_{txt}(t) \\
s_{soc}(t)
\end{bmatrix}
$$

Waarbij:
- $s_{vis}(t)$: visuele stimulus (helderheid, contrast, beweging)
- $s_{aud}(t)$: auditieve stimulus (geluid, muziek)  
- $s_{txt}(t)$: tekstuele/semantische stimulus (trefwoorden)
- $s_{soc}(t)$: sociale stimulus (likes, shares, notificaties)

Elke stimulus heeft een "salience" of opvallendheid $m_k(t)$, gedefinieerd als de mate van verandering van de stimulus:

$$
m_k(t) = \left| \frac{d}{dt} s_k(t) \right|^\alpha, \quad \text{waar } \alpha \in [0.5, 1]
$$

Deze salience geeft de mate van abrupte verandering weer die aandacht trekt, zoals een snelle scènewissel in een video of een plotselinge luide beat in muziek.

---

## 2. Equivalent Resonance Dose (ERD)

Deze sectie introduceert het concept van de **Equivalent Resonance Dose (ERD)**, een maat voor de cumulatieve impact van reclameprikkels op cognitieve biomarkerrespons.

$$
\text{ERD} = \int_{0}^{T} \sum_{k} w_k \cdot m_k(t) ~dt
$$

Hierin:
- $w_k$: weegfactor voor stimulus type $k$
- $m_k(t)$: salience van stimulus $k$ op tijdstip $t$
- $T$: tijdvenster

---

## 3. Biomarkerrespons

De biomarkerrespons wordt gemeten als een verandering $\Delta B_j$ in een cognitieve biomarker $B_j$:

$$
\Delta B_j = f(\text{ERD})
$$

Dit beschrijft een niet-lineaire relatie waarbij een toenemende dosis (ERD) leidt tot een proportionele of verzadigde biomarkerrespons.

---

## 4. Implicaties voor beleid en onderzoek

Dit formele kader biedt een basis voor een vergelijkende analyse van de impact van reclame. Het stelt een hypothese die getest kan worden: als digitale en analoge reclame dezelfde ERD hebben, voorspelt het model dat de gemeten biomarkerrespons ($\Delta B_j$) ook vergelijkbaar zal zijn, wat mechanistische gelijkheid zou aantonen. De ERD-metriek kan ook leiden tot de vaststelling van **normatieve drempelwaarden** voor reclame-exposure. Dit is vergelijkbaar met het instellen van limieten voor geluidsniveaus op de werkplek of voor stralingsniveaus, en kan een basis bieden voor toekomstig beleid ter bescherming van de mentale volksgezondheid.

---
