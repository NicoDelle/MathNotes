Approfondimento: [[IntegraleDefinitoTeoria.pdf]] 

#### Trapezoide
> Sia $f:[a,b] \rightarrow \mathbb{R}$ una funzione.
> Si chiama *trapezoide* di $f$ su $[a,b]$ la regione di piano cartesiano $Oxy$ delimitata dall'intervallo $[a,b]$, dalle rette $x=a$ e $x=b$ e dal grafico di $f$. Si indica con $T(f;a,b)$ 
> $$ 
 T(f;a,b)= \{(x, y)\in \mathbb{R}^2:\: a\leq x \leq b, \:0\leq y \leq f(x)\: \lor\: f(x)\leq y\leq 0 \}
$$


#### Funzione a scala
 >Sia $f:[a,b] \rightarrow \mathbb{R}$ una funzione.
 Diciamo che $f$ è una *funzione a scala* se esiste una suddivisione $a=x_0<x_1<...<x_{n-1}<x_n=b$ di $[a,b] : f$ sia costante su ciascuno degli intervalli aperti $]x_{i-1},\:x_i[ \:\forall\: i=1,\:...\:,n$.

 ![[Pasted image 20230413204943.png]]

Una divisione in intervalli di una funzione a scala $f$ si dice *adattata* ad essa se è costante su ciascuno degli intervalli aperti. (Una funzione a scala ha sempre una suddivisione in intervalli sulla quale è costante -la quale, per inciso, può essere raffinata ad intervalli più piccoli-, tuttavia non è detto che la suddivisione presa in considerazione sia la stessa della definizione) .

#### Integrale definito di una funzione a scala
> Siano $f:[a,b]\rightarrow \mathbb{R}$ una funzione a scala e $a=x_0<x_1<...<x_{n-1}<x_n=b$ una suddivisione adattata di $[a,b]$ a $f$. $\forall\: i=1,\:...\:,n$, indichiamo con $c_i$ il valore costante assunto dalla funzione sull'intervallo $]x_{i-1},\:x_i[$. 
> Si chiama *integrale definito* di $f$ su $[a,\:b]$ il numero reale
> $$
 \int{f=c_1(x_1-x_0)+c_2(x_2-x_1)+\:...\:+c_n(x_n-x_{n-1})} = \sum\limits_{i=1}^{n}{c_i(x_i-x_{i-1})}.
 $$

### Integrale di Riemann
Sia $f:[a,b]\rightarrow \mathbb{R}$ una funzione limitata. La sua immagine è quindi un insieme limitato che ammette minimo $m$ e massimo $M$, e $m\leq f(x)\leq M$. Definiamo:
- $H_f^+ = \{ h:[a,b]\rightarrow \mathbb{R}$ funzione a scala $:f(x)\leq h(x) \:\forall \: x\in [a,b]\}$ 
- $H_f^- = \{ g:[a,b]\rightarrow \mathbb{R}$ funzione a scala $:f(x)\geq h(x) \:\forall \: x\in [a,b]\}$ 
Il primo insieme contiene la funzione costante $k(x)=M$ e il seconda contiene $\phi(x)=m$, e $g(x)\leq f(x)\: \forall \:x\in [a,b]$.

Chiamiamo integrale superiore di $f$ su $[a,b]$ il numero reale
$$
\int\limits_{[a,b]}^{-}{f} = \inf{\{\int\limits_{[a,b]}{h:h\in H_f^+}\}} 
$$
Mentre chiamiamo integrale inferiore di $f$ su $[a,b]$ il numero reale
$$
\int\limits_{-[a,b]}{f} = \sup{\{\int\limits_{[a,b]}{g:g\in H_f^-}\}}
$$
Ossia, l'integrale superiore è l'estremo inferiore degli integrali delle funzioni a scala maggioranti di f (insieme di numeri reali), è quello che meglio approssima per eccesso l'aera del trapezoide di f. Viceversa, l'integrale inferiore è quello che meglio approssima per difetto l'aera (con segno) del trapezoide.

## Integrabilità
### Integrabilità con integrale superiore ed inferiore
>Una funzione $f:[a,b]\rightarrow \mathbb{R}$ si dice integrabile secondo Riemann su $[a,b]$ se 
>$$
\int\limits_{-[a,b]}{f}=\int\limits_{[a,b]}^{-}{f}
$$
In tal caso, denotiamo il valore comune con $\int\limits_{[a,b]}{f}$ , che chiamiamo integrale definito di $f$ su $[a,b]$.

>Si ha anche che, se $f:[a,b]\rightarrow \mathbb{R}$ è una funzione limitata, allora $f$ è integrabile su $[a,b] \iff \: \forall \:\epsilon >0 \:\exists \: h\in H_f^+ \land g\in H_f^-:\int\limits_{[a,b]}{(h-g)}<\epsilon$   

### Funzioni localmente integrabili
> Siano $I\subseteq\mathbb{R}$ un intervallo e $f:I\rightarrow\mathbb{R}$ una funzione.
> $f$ è *localmente integrabile* su $I$ se $f$ è integrabile su ogni intervallo $[a,b]\subseteq I$.
 
Vedi anche [[TeoremiIntegraliDefiniti#Teorema di integrabilità secondo Riemann]]

## Proprietà degli integrali definiti
--

## Media integrale
> Sia $f:[a,b]\rightarrow \mathbb{R}$ una funzione integrabile.
> Si chiama *media integrale di* $f$ *su* $[a,b]$ il numero reale
> $$
m(f;a,b)=\frac{1}{b-a}\int\limits_a^b{f(x)\:dx}$$

$m(f;a,b)$ corrisponde all'altezza di un rettangolo di base $b-a$ 
Vedi anche il [Teorema della media integrale](<Teoremi Integrali Definiti#Teorema della media integrale>).

## Funzione Integrale
> Siano $I\subseteq\mathbb{R}$ un intervallo e $f:I\rightarrow\mathbb{R}$ una funzione localmente integrabile su $I$ e $x_0\in I$.
> Si chiama *funzione integrale di* $f$ *su* $I$ associata a $x_0$ la funzione $F:I\rightarrow\mathbb{R}$ definita da:
> $$
\forall x\in I:\:\: F(x)=\int\limits_{x_0}^x{f(t)\:dt}
$$

La variabile della funzione integrale è l'estremo superiore di integrazione: associa ad ogni punto $x\in I$ l'area con segno del trapezoide di $f$ delimitato dal centro $x_0$ e $x$ stesso.
$F$ è continua.