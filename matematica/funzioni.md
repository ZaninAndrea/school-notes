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

### Caratteristiche delle funzioni
- **iniettive:** $$\forall \: x,y \in A \Rightarrow f(x)\ne f(y)$$
    - una funzione è reversibile se è iniettiva
- **suriettiva:** $$\forall \: y \in B \; \exists \: x \mid f(x)=y$$
- **biettiva:** sia iniettiva che suriettiva
- **crescente:** $$\forall \: x_1, x_2 \in A \mid x_1 < x_2 \Rightarrow f(x_1) \lt f(x_2)$$
- **monotòna:** una funzione si dice monotona se è sempre crescente o sempre decrescente nel suo dominio
- **periodica:** $$\exists \: T \mid f(x)=f(x+kT) \; k \in \mathbb{Z}$$
- **pari:** $$\forall \: x \in A \; f(-x)=f(x)$$
- **dispari:** $$\forall \: x \in A \; f(-x)=-f(x)$$