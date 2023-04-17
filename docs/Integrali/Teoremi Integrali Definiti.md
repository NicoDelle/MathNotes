#### Teorema di integrabilità secondo Riemann
> Sono integrabili secondo Riemann:
1) Le funzioni continue su un intervallo $[a,b]$
2) le funzioni limitate su un intervallo $[a,b]$ aventi un numero finito di punti di discontinuità di prima specie
3) le funzioni monotone su un intervallo $[a,b]$

#### Teorema della media integrale
> Sia $f:[a,b]\rightarrow \mathbb{R}$ una funzione integrabile.
> Allora:
> a) $\inf\limits_{[a,b]}{f} \leq m(f;a,b) \leq \sup\limits_{[a,b]}{f}$
> b) se $f$ è continua in $[a,b] \Rightarrow \exists\: x_0\in [a,b]:f(x_0)=m(f;a,b)$

Dove la a significa che $f$ assume almeno un valore minore o uguale a m, e almeno uno maggiore o uguale a m, all'interno di $[a,b]$.
La b si ha invece per il [Teorema di Weierstass](<TeoremiContinuità##Teorema di Weierstass>).

## Teorema fondamentale del calcolo integrale
> Siano $I \subseteq\mathbb{R}$ un intervallo, $f:I\rightarrow\mathbb{R}$ una funzione continua e $x_0\in I$.
> Allora la [funzione integrale](<Integrali definiti#Funzione Integrale>) $F$ di $f$ su $I$ associata a $x_0$ è derivabile su $I$ con $F'(x)=f(x)\:\forall x\in I$.
> In particolare F è una primitiva di $f$ su $I$

In altre parole, le funzioni continue in un intervallo hanno sempre primitiva nell'intervallo, data dalla loro funzione integrale (+ c).

### Primo corollario
> Siano $I \subseteq\mathbb{R}$ un intervallo, $f:I\rightarrow\mathbb{R}$ funzione continua, $x_0\in I$, $G:I\rightarrow\mathbb{R}$ una primitiva di $f$ su $I$ e $F(x)=\int\limits_{x_0}^x{f(t)\:dt}$ la [funzione integrale](<Integrali definiti#Funzione Integrale>) di $f$ su $I$ associata a $x_0$. 
> Allora $F(x)=G(x)-G(x_0)\:\forall x\in I$.
> Inoltre, se $f$ è derivabile con derivata continua su $I$ si ha che
> $$
 \forall x\in I: \:\: f(x)=f(x_0)+\int\limits_{x_0}^x{f'(t)\:dt}
 $$

La prima parte del corollario deriva dal fatto che due primitive di una stessa funzione (F per il teorema fondamentale, G per ipotesi del teorema fondamentale) differiscono, per un teorema degli integrali indefiniti (!!completa), per una costante $c: F(x)=G(x)-c \:\forall x\in I\Rightarrow c=G(x_0)-F(x_0)$. Ma $F(x_0)=0$ per definizione, quindi $c=G(x_0)$.

### Teorema di Torricelli-Barrow
>Siano $I\subseteq\mathbb{R}$ un intervallo, $f:I\rightarrow\mathbb{R}$ una funzione continua, $G:I\rightarrow\mathbb{R}$ una primitiva di $f$ su $I$ e $a,b\in I$.
>Allora
>$$
\int\limits_b^a{f(x)\:dx}=G(b)-G(a)
 $$

Segue quasi direttamente dal corollario del T.F.C.I, e permette di calcolare rapidamente l'area con segno del trapezoide semplicemente come differenza tra i valori assunti dalla primitiva agli estremi della funzione.