# Dalla Capitalizzazione Composta alla Capitalizzazione Continua
## Come nasce il numero e: l'esperimento mentale del reinvestimento continuo

---

### 1. Il Gancio Didattico per la Classe (L'Esperimento Mentale)

> **La domanda provocatoria per gli studenti:**  
> *"Immaginiamo che una banca ci riconosca un tasso di interesse annuo nominale del 100% su un deposito di 1.000 €. Se ritiriamo capitale e interessi solo dopo 1 anno, otteniamo 2.000 €.  
> Ma cosa succede se ritiriamo e reinvestiamo ogni 6 mesi? E se lo facciamo ogni mese? Ogni giorno? Ogni secondo?  
> Se potessimo reinvestire **a ogni istante infinitesimo di secondo**, diventeremmo infinitamente ricchi?"*

La risposta intuitiva di molti ragazzi è: *"Con infiniti reinvestimenti il capitale diventerà enorme, forse infinito!"*.  
La realtà matematica è sbalorditiva: **il montante converge a un limite finito**, e da questa convergenza nasce storicamente il **numero di Nepero e** (Jacob Bernoulli, 1683).

---

### 2. Il Meccanismo Matematico

Siano:
- $C_0$: Capitale iniziale investito.
- $r$: Tasso di interesse nominale annuo (es. $100\% \to r = 1$; $10\% \to r = 0{,}10$).
- $n$: Numero di volte in cui l'anno viene frazionato (frequenza di capitalizzazione).
- $t$: Tempo in anni (nel nostro schema $t = 1$).

A ogni frazione di anno:
1. La durata del periodo è $\Delta t = \frac{1}{n}$ di anno.
2. Il tasso di interesse applicato a ciascun periodo è proporzionale:
   $$i_n = \frac{r}{n}$$
3. Alla scadenza di ogni periodo gli interessi maturati vengono aggiunti al capitale (*capitalizzazione*) e generano a loro volta nuovi interessi nel periodo successivo (*interesse composto*).

Dopo 1 anno ($n$ periodi), il montante finale è:
$$M_n = C_0 \cdot \left(1 + \frac{r}{n}\right)^n$$

Se facciamo tendere la frequenza di capitalizzazione all'infinito ($n \to +\infty$, cioè $\Delta t \to 0$, ogni istante infinitesimo):
$$M_{\text{continuo}} = \lim_{n \to +\infty} C_0 \left(1 + \frac{r}{n}\right)^n = C_0 \cdot e^r$$

Per un orizzonte temporale qualsiasi di $t$ anni:
$$M(t) = C_0 \cdot e^{r \cdot t}$$

---

### 3. Schema Comparativo 1: Il Caso Didattico di Bernoulli ($C_0 = 1.000\ €$, $r = 100\%$)

In questo caso $r = 1$, quindi la formula diventa esattamente:
$$M_n = 1.000 \cdot \left(1 + \frac{1}{n}\right)^n$$

Notare come all'aumentare di $n$ compaiano progressivamente le cifre decimali del numero di Nepero $e = 2{,}718281828...$:

| Frequenza di reinvestimento | Intervallo temporale ($\Delta t$) | Numero di periodi ($n$) | Formula applicata | Montante dopo 1 anno ($M$) | Guadagno extra rispetto all'annuale |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Annuale** | 1 anno | $n = 1$ | $1.000 \cdot (1 + 1)^1$ | **2.000,00 €** | $+ 0,00\ €$ (base) |
| **Semestrale** | 6 mesi | $n = 2$ | $1.000 \cdot (1 + 0{,}5)^2$ | **2.250,00 €** | $+ 250,00\ €$ |
| **Quadrimestrale** | 4 mesi | $n = 3$ | $1.000 \cdot \left(1 + \frac{1}{3}\right)^3$ | **2.370,37 €** | $+ 370,37\ €$ |
| **Trimestrale** | 3 mesi | $n = 4$ | $1.000 \cdot (1 + 0{,}25)^4$ | **2.441,41 €** | $+ 441,41\ €$ |
| **Bimestrale** | 2 mesi | $n = 6$ | $1.000 \cdot \left(1 + \frac{1}{6}\right)^6$ | **2.521,63 €** | $+ 521,63\ €$ |
| **Mensile** | 1 mese | $n = 12$ | $1.000 \cdot \left(1 + \frac{1}{12}\right)^{12}$ | **2.613,04 €** | $+ 613,04\ €$ |
| **Settimanale** | 7 giorni | $n = 52$ | $1.000 \cdot \left(1 + \frac{1}{52}\right)^{52}$ | **2.692,60 €** | $+ 692,60\ €$ |
| **Giornaliero** | 1 giorno (24 h) | $n = 365$ | $1.000 \cdot \left(1 + \frac{1}{365}\right)^{365}$ | **2.714,57 €** | $+ 714,57\ €$ |
| **Orario** | 1 ora | $n = 8.760$ | $1.000 \cdot \left(1 + \frac{1}{8.760}\right)^{8.760}$ | **2.718,13 €** | $+ 718,13\ €$ |
| **Al minuto** | 1 minuto | $n = 525.600$ | $1.000 \cdot \left(1 + \frac{1}{525.600}\right)^{525.600}$ | **2.718,28 €** | $+ 718,28\ €$ |
| **Al secondo** | 1 secondo | $n = 31.536.000$ | $1.000 \cdot \left(1 + \frac{1}{31.536.000}\right)^{31.536.000}$ | **2.718,2818 €** | $+ 718,2818\ €$ |
| **Continuo (infinitesimo)** | $dt \to 0$ | $n \to +\infty$ | $1.000 \cdot e^1$ | **2.718,2818 €** | $+ 718,2818\ €$ |

---

### 4. Schema Comparativo 2: Un Caso Finanziario Realistico ($C_0 = 10.000\ €$, $r = 10\%$)

Formula:
$$M_n = 10.000 \cdot \left(1 + \frac{0{,}10}{n}\right)^n \quad \longrightarrow \quad M_{\text{continuo}} = 10.000 \cdot e^{0{,}10} \approx 11.051{,}71\ €$$

| Frequenza | $n$ | Montante ($M$) | Interesse totale maturato | Guadagno extra vs Annuale |
| :--- | :--- | :--- | :--- | :--- |
| **Annuale** | $1$ | **11.000,00 €** | $1.000,00\ €$ | $-$ |
| **Semestrale** | $2$ | **11.025,00 €** | $1.025,00\ €$ | $+ 25,00\ €$ |
| **Trimestrale** | $4$ | **11.038,13 €** | $1.038,13\ €$ | $+ 38,13\ €$ |
| **Mensile** | $12$ | **11.047,13 €** | $1.047,13\ €$ | $+ 47,13\ €$ |
| **Giornaliero** | $365$ | **11.051,56 €** | $1.051,56\ €$ | $+ 51,56\ €$ |
| **Orario** | $8.760$ | **11.051,70 €** | $1.051,70\ €$ | $+ 51,70\ €$ |
| **Al minuto** | $525.600$ | **11.051,71 €** | $1.051,71\ €$ | $+ 51,71\ €$ |
| **Al secondo** | $31.536.000$ | **11.051,71 €** | $1.051,71\ €$ | $+ 51,71\ €$ |
| **Continuo** | $n \to +\infty$ | **11.051,71 €** | $1.051,71\ €$ | $+ 51,71\ €$ |

---

### 5. Il Passaggio Rigoroso al Limite (Livello 4ª/5ª Superiore)

1. Partiamo da:
   $$M_n = C_0 \left(1 + \frac{r}{n}\right)^n$$
2. Eseguiamo il cambio di variabile:
   $$x = \frac{n}{r} \implies n = r \cdot x$$
   Poiché $r > 0$, quando $n \to +\infty$ anche $x \to +\infty$.
3. Sostituiamo nell'espressione:
   $$M = \lim_{n \to +\infty} C_0 \left(1 + \frac{r}{n}\right)^n = C_0 \cdot \lim_{x \to +\infty} \left(1 + \frac{1}{x}\right)^{r \cdot x} = C_0 \cdot \left[ \lim_{x \to +\infty} \left(1 + \frac{1}{x}\right)^x \right]^r$$
4. Riconoscendo il **limite notevole** che definisce il numero $e$:
   $$\lim_{x \to +\infty} \left(1 + \frac{1}{x}\right)^x = e$$
   si ottiene immediatamente:
   $$M(1) = C_0 \cdot e^r$$
   e per un periodo di $t$ anni:
   $$M(t) = C_0 \cdot e^{r \cdot t}$$

---

### 6. Spunti di Riflessione per il Dibattito in Classe

1. **Il conflitto degli infiniti (Forma indeterminata $1^\infty$):**  
   All'aumentare di $n$:
   - La base $\left(1 + \frac{r}{n}\right) \to 1$ (gli interessi per singolo periodo diventano microscopici, tendono a 0).
   - L'esponente $n \to +\infty$ (il numero di volte che capitalizziamo diventa enorme).  
   È la classica forma indeterminata $[1^\infty]$: né l'esponente porta il valore all'infinito, né la base lo tiene schiacciato a 1. Trovano un perfetto equilibrio nel numero $e^r$.

2. **Rendimenti marginali decrescenti:**  
   Frazionare il tempo conviene molto all'inizio (da annuale a mensile si recupera quasi tutto il vantaggio teorico), ma procedere verso il secondo o l'infinitesimo non produce alcun guadagno percepibile.

3. **Perché nei modelli matematici e finanziari si usa $e^{rt}$?**  
   Anche se nella pratica quotidiana le banche accreditano gli interessi con cadenza discreta (annuale o trimestrale), nei modelli matematici avanzati (es. derivati, formule di Black-Scholes per le opzioni, modelli differenziali) si usa **sempre la capitalizzazione continua**:
   - È una funzione continua e differenziabile ovunque: $\frac{d}{dt}(C_0 e^{rt}) = r \cdot C_0 e^{rt}$.
   - Gode della proprietà esponenziale: $e^{r(t_1 + t_2)} = e^{rt_1} \cdot e^{rt_2}$.
   - Rende i calcoli analitici immensamente più semplici ed eleganti rispetto a formule con sommatorie o potenze discrete.
