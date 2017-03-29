# Funzioni
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

### Esercizio
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
    "title": "Grafico",
    "grid": true,
    "xAxis": {
        "label": "x",
        "domain": [0, 300]
    },
    "yAxis": {
        "label": "y",
        "domain": [-1.5, 1.5]
    },
    "data": [{
        "fn": "( 2 - x )/( x + 5 )"
    }],
    "annotations": [{
        x: -5,
        text: 'x = -5'
    }, {
        y: -1,
        text: 'y = -1'
    }]
}
{% endgraph %}

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
- $$\forall \epsilon \gt 0 \; \exists x \in A \mid M - \epsilon \le x \le M $$

$$\epsilon$$ e $$\delta$$ in matematica indicano un numero positivo arbitrariamente piccolo

L'insieme $$A$$ (vedi sopra) ha come estremo superiore 1, ma non ha un estremo inferiore.

### Intorno
Si dice **intorno** di un punto $$ x_0 $$ un qualsiasi intervallo aperto contenente $$x_0$$, e.g. $$(x_0 - \delta \; , \; x_0 + \delta ) $$. Posso definire anche un intorno di infinito:
- intorno di $$+ \infty$$: $$(M \; , \; + \infty)$$
- intorno di $$- \infty$$: $$(- \infty \; , \; -M)$$


### Punto isolato
$$x_0$$ è detto **punto isolato** se esiste un intorno di $$x_0$$ che non contiene elementi di $$A$$$ diversi da $$x_0$$




