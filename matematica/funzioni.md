# Studio di funzione
Una funzione è una relazione tra 2 insieme che associa un elemento di $$A$$ ad un solo elemento di $$B$$.
$$
\forall \: x \in A \; \exists! \; y \in B \mid y=f(x) 
$$

## Ripasso
**DOMINIO:** l'insieme di tutti gli elementi dell'insieme $$A$$ che sono legati ad un elemento di $$B$$
**CODOMINIO:** l'insieme di tutti gli elementi dell'insieme $$B$$ che sono legati a uno o più elementi di $$A$$
Funzioni algebriche:
- razionali intere $$y=x$$
- razionali fratte $$y=\frac{1-x}{x+3}$$
- irrazionali $$y=\sqrt{x^2 - 1}$$

Funzioni trascendenti:
- logaritmiche
- esponenziali
- goniometriche

### Esercizi
#### Esercizio 1
Studio la funzione $$y=\frac{2-x}{x+5}$$
**DOMINIO:** $$x \ne -5 $$
**INTERSEZIONE CON GLI ASSI**
$$
\begin{cases}
x=0 \\
y = \frac{2-x}{x+5}
\end{cases}
\qquad
\begin{cases}
y=0 \\
y = \frac{2-x}{x+5}
\end{cases}
\\
\begin{cases}
x=0 \\
y = \frac{2}{5}
\end{cases}
\qquad
\begin{cases}
y=0 \\
x = 2
\end{cases}
$$
**STUDIO DEL SEGNO**
$$
\frac{2-x}{x+5}\gt 0 \\
-5 \lt x \lt 2
$$
**ASINTOTI**
$$
\begin{align*}
y&=\frac{2-x}{x+5} \\
&= -1 + \frac{7}{x+5} \\
y + 1 &= \frac{7}{x+5} \\
\text{asintoti: } x&=-5 \\ y&=-1
\end{align*}
$$

{% graph %}
{
    "grid": false,
    "xAxis": {
        "label": "x",
        "domain": [0, 30]
    },
    "yAxis": {
        "label": "y",
        "domain": [-1.5, 1.5]
    },
    "data": [{
        "fn": "( 2 - x )/( x + 5 )"
    }],
    "annotations": [{
        "x": -5,
        "text": "x = -5"
    }, {
        "y": -1,
        "text": "y = -1"
    }]
}
{% endgraph %}

#### Esercizio 2
$$
y=2^\sqrt{x} - \sqrt{2^x}
$$
**DOMINIO: ** $$x\ge0$$

$$
\begin{cases}
x\ge0 \\
2^x \ge 0
\end{cases}
\\
\Downarrow \\
x\ge0
$$

**INTERSEZIONI: ** (0,0) (4,0)
Con asse y
$$
\begin{cases}
x=0 \\
2^0 - \sqrt{2^0}
\end{cases}
\\
\Downarrow \\
y=0
$$

Con asse x
$$
\begin{cases}
y=0 \\
0 = 2^\sqrt{x} - \sqrt{2^x}
\end{cases} 
\\
\Downarrow \\
x_1 = 0 \quad x_2=4
$$

**SEGNO: ** $$0 \lt x \lt 4$$
$$
2^{\sqrt{x}}-\sqrt{2^x}\gt 0 \\
\Downarrow \\
0 \lt x \lt 4
$$
![](/assets/studio.png)

#### Esercizio 3
**DOMINIO: ** $$x\ne \frac{\pi}{6},\frac{11\pi}{6}$$

$$
2\cos{x}-\sqrt{3}\ne0 \\
x\ne \frac{\pi}{6},\frac{11\pi}{6}
$$

**INTERSEZIONI: ** (0,0) ($$\pi$$,0) ($$2\pi$$,0)
con x
$$
\begin{cases}
y=0\\
\sin{x}=0
\end{cases}
\\
\Downarrow
\\
x=0,\pi,2\pi
$$

### Caratteristiche delle funzioni
- **iniettive:** $$\forall \: x,y \in A \Rightarrow f(x)\ne f(y)$$
    - una funzione è reversibile se è iniettiva
- **suriettiva:** $$\forall \: y \in B \; \exists \: x \mid f(x)=y$$
- **biettiva:** sia iniettiva che suriettiva
- **crescente:** $$\forall \: x_1, x_2 \in A \mid x_1 < x_2 \Rightarrow f(x_1) \lt f(x_2)$$
- **monotòna:** una funzione si dice monotona se è sempre crescente o sempre decrescente nel suo dominio
- **periodica:** $$\exists \: T \mid f(x)=f(x+kT) \quad k \in \mathbb{Z}$$
- **pari:** $$\forall \: x \in A \; f(-x)=f(x)$$
- **dispari:** $$\forall \: x \in A \; f(-x)=-f(x)$$

## Sottoinsiemi di R
### Intervalli
Intervalli in $$\mathbb{R}$$
- **intervallo chiuso:** estermi inclusi $$[a,b]=\{x \mid x \in \mathbb{R} \quad a \ge x \ge b \}$$
- **intervallo aperto:**  estremi non inclusi $$(a,b) = ]a,b[$$
    - l'infinito non può mai essere incluso $$(- \infty, 5)$$
- **intervallo misto:** $$(a,b]$$

### Superiormente limitato
Un insieme $$A \subseteq \mathbb{R}$$ si dice **superiormente limitato** se $$\exists \; k \in \mathbb{R} \mid \forall \; x \in A \quad x \le k $$
$$k$$ non necessariamente deve appartenere ad $$\mathbb{R}$$, e.g.

$$
\begin{align*}
A &= \{ x \mid x = \frac{n}{n+1} \quad n \in \mathbb{N} \} \\
&= \{0,\frac{1}{2},\frac{2}{3},\frac{3}{4},...\}
\end{align*}
$$

$$A$$ è superiormente limitato da 1, anche se 1 non è incluso nell'insieme.
Analogamente un insieme può essere **inferiormente limitato**

### Estremo superiore
Dato $$A$$ superiormente limitato, si dice **estremo superiore** di $$A$$ quel numero $$M$$ tale che
- $$\forall x \in A \quad x \le M $$
- $$\forall \epsilon \gt 0 \; \exists x \in A  (x \ne M) \mid M - \epsilon \le x \le M $$

$$\epsilon$$ e $$\delta$$ in matematica indicano un numero positivo arbitrariamente piccolo

L'insieme $$A$$ (vedi sopra) ha come estremo superiore 1, ma non ha un estremo inferiore.

### Intorno
Si dice **intorno** di un punto $$ x_0 $$ un qualsiasi intervallo aperto contenente $$x_0$$, e.g. $$(x_0 - \delta \; , \; x_0 + \delta ) $$. Posso definire anche un intorno di infinito:
- intorno di $$+ \infty$$: $$(M \; , \; + \infty)$$
- intorno di $$- \infty$$: $$(- \infty \; , \; -M)$$


### Punto isolato
$$x_0$$ è detto **punto isolato** se esiste un intorno di $$x_0$$ che non contiene elementi di $$A$$ diversi da $$x_0$$

### Punto di accumulazione
$$x_0$$ si dice **punto di accumulazione** dell'insieme $$\mathbb{A}$$ se ogni intorno di $$x_0$$ contiene un elemento dell'insieme $$\mathbb{A}$$

$$
\forall \epsilon \gt 0\quad \exists x \in \mathbb{A} \mid x \in (x_0 - \epsilon, x_0 + \epsilon)
$$

E.g.
$$
\begin{align*}
A&=\{x \mid x = \frac{1}{n} \text{ con } n \in \mathbb{N} -\{0\}\} \\
&=\{0,\frac{1}{2},\frac{1}{3},\frac{1}{4}, \dots\}
\end{align*}
$$
A è superiormente e inferiormente limitato, non ha un estremo superiore, ma ha come estremo inferiore e punto di accumulazione 0.

## Limiti
### Comprensione intuitiva dei limiti
$$
\lim_{x \to 2} \frac{x^2-4}{x-2} \qquad \text{generica} \\
\lim_{x \to 2^-} \frac{x^2-4}{x-2} \qquad \text{da sinistra} \\
\lim_{x \to 2^+} \frac{x^2-4}{x-2} \qquad \text{da destra} \\
$$

**Valori della funzione avvicinandomi da sinistra**

| x | 1.9 | 1.99 | 1.999 |
| --- | --- | --- | --- |
| y | 3.9 | 3.99 | 3.999 |

Intuitivamente per $$x=2$$ attribuiremmo il valore 4, ma la funzione non vale 4, anzi la funzione non è nemmeno definita per $$x=2$$

$$
\lim_{x \to 2^-} \frac{x^2-4}{x-2} = 4
$$

**Valori della funzione avvicinandomi da destra** 

| x | 2.1 | 2.01 | 2.001 |
| --- | --- | --- | --- |
| y | 4.1 | 4.01 | 4.001 |

Anche in questo caso intuitivamente attribuiremmo valore 4 per $$x=2$$

$$
\lim_{x \to 2^+} \frac{x^2-4}{x-2} = 4
$$

### Definizione di limite
#### CASO l FINITO
$$
\lim_{x \to x_0} f(x) = l
$$
$$x_0$$ può essere sia un numero che infinito
$$I(x_0)$$ è un intorno di $$x_0$$
$$\forall$$ intorno di $$l$$ ($$\forall \epsilon \gt 0$$ arbitrariamente piccolo) $$\exists I(x_0) \text{ t.c. } \forall x \ne x_0 \in I(x_0) \Rightarrow \mid F(x) - l \mid  \lt \epsilon $$

**Verifica con la definizione il seguente limite**
$$
\lim_{x \to 2} \frac{x^2 -4}{x-2} = 4
$$

DEFINIZIONE
$$
\forall \epsilon \gt 0 \; \exists I(2) \text{ t.c. } \forall x \ne 2 \in I(2) \Rightarrow \mid \frac{x^2 -4}{x-2} - l \mid  \lt \epsilon 
$$

SVILUPPO LA CONDIZIONE
$$
\mid \frac{x^2 -4}{x-2} - l \mid \lt \epsilon \\
\mid \frac{x^2 -4 -4x + 8}{x-2} \mid \lt \epsilon \\
\mid \frac{x^2 -4x +4}{x-2} \mid \lt \epsilon \\
\mid \frac{(x-2)^2}{x-2} \mid \lt \epsilon \\
\mid x-2 \mid \lt \epsilon
$$

Sviluppando, ho verificato che x è molto vicino a 2, infatti la differenza tra 2 ed x è di minima (inferiore ad $$\epsilon$$)









