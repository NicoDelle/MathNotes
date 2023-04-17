Vari metodi per calcolare [[Integrali indefiniti]]
Esercizi a: [[ZwScPrimitive2Esercizi.pdf]]

## Sostituzioni
Anche le [[#Funzioni Irrazionali]] si risolvono spesso per sostituzione

#### Seni e Coseni
Dato $\int R(\sin{x},\cos{x})\:dx$, con $R$ funzione razionale
- Se $R(-\sin{x}, \cos{x})=-R(\sin{x}, \cos{x})\:\Rightarrow\:\cos{x}=t$ 
- Se $R(\sin{x}, -\cos{x})=-R(\sin{x}, \cos{x})\:\Rightarrow\:\sin{x}=t$ 
- Se $R(-\sin{x}, -\cos{x})=R(\sin{x}, \cos{x})\:\Rightarrow\:\tan{x}=t$

Dati $\int\sin{(mx)}\sin{(nx)}\:dx, \: \int\cos{(mx)}\sin{(nx)}\:dx,\:\int\sin{(mx)}\cos{(nx)}\:dx$ 
- si usano le [[FormuleTrigonometriche##Werner]] 

Dato $\int\sin^m{x}\cos^n{x}\:dx$
- Se m è dispari pongo $\cos{x}=t$
- Se n è dispari pongo $\sin{x}=t$ 
- Se $m+n<0$ e pari, pongo $\tan{x}=t$
- Se $m, n$ sono pari e positivi, si usano le formule di duplicazione

### Sostituzioni iperboliche
integrale | sostituzione
-- | --
$\int R(x, \sqrt{a^2+x^2})\:dx$ | $x=a \tan{t} \lor x = a\sinh{t}$
$\int{R(x, \sqrt{x^2-a^2})\:dx}$ | $x=a\sec{t} \lor x=a\cosh{t}$
$\int{R(x, \sqrt{a^2-x^2})}\:dx$ | $x=a\sin{t} \lor x=\tanh{t}$


## Funzioni Irrazionali
Teoria ed esempi a: [[ZwScPrimitive2.pdf]]
Si risolvono generalmente per sostituzione, esistono sostituzioni opportune in base ai diversi casi.

### Funzione irrazionale fratte
Dato
$$
\int \sqrt[N]({\frac{ax + b}{cx + d}})^m\: dx
$$
con radice di indice N (volendo trasformarla in potenza, con denominatore N), sostituiamo
$$
t^N = \frac{ax + b}{cx + d}
$$
dove N è il minimo comune multiplo tra gli indici di tutte le radici nell'integrale (devono avere tutte lo stesso radicando).

### Prima sostituzione di Eulero
Dato
$$
\int \sqrt{ax^2 + bx + c} \: dx
$$
con $a>0$, sostituiamo
$$
\sqrt{ax^2 + bx + c} = \pm \sqrt{a}x + t
$$
da questa espressione si ricava $x(t)$ e da questa $dx$. Si sostituisce poi $x(t)$ con la x al secondo membro dell'equazione di sostituzione, per poi sostituire il secondo membro (in t) al posto dell'integrale (che equivale al primo membro).

### Seconda sostituzione di Eulero
Dato
$$
\int \sqrt{ax^2 + bx + c} \: dx
$$
con $c>0$, sostituiamo
$$
\sqrt{ax^2 + bx + c} = xt \pm c
$$
e operiamo un procedimento analogo

### Terza sostituzione di Eulero
Dato
$$
\int \sqrt{ax^2 + bx + c} \: dx
$$
se $ax^2+bx+c=0$ ha due soluzioni reali, sostituiamo
$$
\sqrt{ax^2 + bx + c} = (x-\alpha)t \pm c
$$
dove $\alpha$ è una delle due radici, e operiamo un procedimento analogo. In generale, dopo aver elevato al quadrato e scomposto il radicando, si può semplificare un fattore ad ambo i membri, permettendo di ricavare x.

## Funzioni Razionali Fratte
Sono integrali del tipo $\int \frac{A(x)}{B(x)}\:dx$.
Nel caso in cui il grado di $A(x)$ sia maggiore del grado di $B(x)$, allora potrebbe essere necessario operare una [[divisione tra polinomi]] , in modo tale da ricondursi ad un integrale del tipo $\int \frac{B(x)·Q(x)+R(x)}{B(x)}\:dx$, con $A(x)=B(x)·Q(x)+R(x)$ e $\deg{R(x)}<\deg{B(x)}$.
Si ottiene un integrale del tipo:
$$
\int (Q(x) + \frac{R(x)}{B(x)})\:dx
$$

A seconda del grado di $B(x)$ (che abbiamo detto essere sempre minore del grado di $R(x)$) si distinguono 4 casistiche:
Tipo denominatore | Forma | Si ricondiuce a
--| -- | --
Denominatore di primo grado | $\int \frac{k}{ax+b}\:dx$ | $\int \frac{f'(x)}{f(x)}\:dx$ 
Denominatore di secondo grado, $\Delta > 0$ | $\int \frac{mx+n}{ax^2+bx+c}\:dx$ | $\int \frac{A}{x-x_1} \:dx \: + \: \int \frac{B}{x-x_2}\:dx$ 
Denominatore di secondo grado, $\Delta = 0$ | $\int \frac{mx+n}{(px+q)^2}\:dx$ | $\int \frac{A}{px+q} \:dx \: + \: \int \frac{B}{(px+q)^2}\:dx$
Denominatore di secondo grado, $\Delta <0$ | $\int{\frac{mx+n}{ax^2+bx+c}\:dx}$ | logaritmi, arcotangenti, [[#Ricorrenze]]
Con A, B scelti opportunamente (vedi metodo dei [[#Fratti semplici]]). 

#### Fratti semplici
Una volta operate le dovute divisioni e fattorizzato il denominatore, questo si può scomporre in somme di diverse frazioni, con un preciso tipo di numeratore a seconda del tipo del denominatore. 

### Ricorrenze
integrale | ricorrenza | caso base 
-- | -- | --
$J_n = \int \frac{dx}{(1+x^2)^n}$| $J_n = \frac{2n-3}{2(n-1)}J_{n-1}+\frac{x}{2(n-1)(x^2+1)^{n-1}}$ | $J_1=\arctan{x}$ 


## Integrali Notevoli
integrale | risultato
-- | --
$\int \tan{x}\:dx$ | $-\ln{\|{\cos{x}}\|}$ 
$\int{\frac{1}{\cos{x}}\:dx}$ | $\ln{\|\frac{1+\tan{\frac{x}{2}}}{1-\tan{\frac{x}{2}}}\|}$
$\int{\frac{1}{\sin{x}}\:dx}$ | $\ln{\|\tan{\frac{x}{2}}\|}$
