# Canvas Didattici

Raccolta di canvas interattivi ed esperimenti didattici per l'apprendimento visivo e pratico della matematica e delle scienze.

## 🚀 Live Demo su GitHub Pages

Puoi provare il laboratorio direttamente online al seguente link:

👉 **[https://biodanzalberto-bot.github.io/Canvas-didattici/](https://biodanzalberto-bot.github.io/Canvas-didattici/)**

---

## 📐 Laboratori Disponibili

### 1. La Sinusoide in Gradi ($y = \sin(x)$)
- **File:** [`laboratorio_sinusoide.html`](laboratorio_sinusoide.html)
- **Funzionalità:**
  - **Circonferenza goniometrica interattiva:** visualizzazione dinamica del raggio, dell'angolo in gradi e della proiezione verticale (seno).
  - **Grafico sinusoide in tempo reale:** tracciamento coordinato dell'onda sinusoidale su intervallo da 0° a 360°.
  - **Esplorazione libera & Animazione automatica:** controllo tramite slider, rotazione a mouse/touch e riproduzione continua.
  - **Modalità Sfida ("Becca i Gradi"):** minigioco con domande a punteggio per mettere alla prova la comprensione degli angoli notevoli e dei valori del seno nei quattro quadranti.

### 2. Dalla Capitalizzazione Composta alla Continua ($M = C_0 \cdot e^{rt}$)
- **File:** [`laboratorio_capitalizzazione.html`](laboratorio_capitalizzazione.html)
- **Funzionalità:**
  - **Esperimento Mentale di Bernoulli & Scenari Reali:** transizione da capitalizzazione annuale ($n=1$) a infinitesima ($n \to \infty$) attraverso 11 livelli discreti (6 mesi, 1 mese, 1 giorno, 1 secondo, continuo).
  - **Doppio Grafico Dinamico (Canvas 2D):**
    1. *Evoluzione temporale a gradini vs curva limite continua $e^{rt}$*: visualizza come i gradini discreti si fondono nella curva differenziabile all'aumentare di $n$.
    2. *Convergenza asintotica & Istogramma utilità marginale*: evidenzia visivamente l'asintoto del capitale e il crollo a zero del guadagno incrementale.
  - **Animazione Continua & Quiz Interattivo:** simulazione automatica della convergenza e minigioco a risposta multipla con punteggio e spiegazioni didattiche.

---

## 🛠️ Come aggiungere nuovi laboratori

1. Aggiungi il nuovo file `.html` (es. `laboratorio_nuovo.html`) in questa cartella.
2. Esegui il commit e il push su GitHub:
   ```bash
   git add .
   git commit -m "Aggiunto nuovo laboratorio"
   git push
   ```
3. Il nuovo file sarà subito accessibile su:
   `https://biodanzalberto-bot.github.io/Canvas-didattici/laboratorio_nuovo.html`
