***
+ AP 2007
+ Gegeben sind die reellen Funktionen:
$$
\begin{align*}
&f_a: f_a(x) = -a + 2 \cdot a \cdot \cos(x)
&g_a: g_a(x) = -a + 2 \cdot \sin(2x) \\
&\quad \text{mit } a \in \mathbb{R},\ a>0 
&\text{im Intervall} \quad  [0;2\pi]
\end{align*}
$$

+ 4.1.0 In dieser Teilaufgabe gilt $a=1$
+ 4.1.1 Berechnen sie die Koordinaten der Schnittpunkte der Funktion $f_{1}$ und $g_{1}$

# Schnittpunkte von $f_1$ und $g_1$

Gegeben mit $a=1$:
$$f(x) = -1 + 2\cos(x), \qquad g(x) = -1 + 2\sin(2x), \qquad x \in [0;2\pi]$$

## Gleichsetzen

$$
\begin{align*}
-1 + 2\cos(x) &= -1 + 2\sin(2x) \\
2\cos(x) &= 2\sin(2x)
\end{align*}
$$

Doppelwinkelsatz $\sin(2x) = 2\sin(x)\cos(x)$ einsetzen:

$$
\begin{align*}
2\cos(x) &= 4\sin(x)\cos(x) \\
2\cos(x)\big[1 - 2\sin(x)\big] &= 0 \quad \text{2cos(x) ausklammern}
\end{align*}
$$

Ein Produkt ist Null, wenn mindestens ein Faktor Null ist $\Rightarrow$ zwei Fälle.

---

## Fall 1: $2\cos(x) \implies \cos(x) = 0$
+ cos(x)=0 bedeutet der Punkt hat x-Koordinate 0
+ Das ist oben und unten auf den Kreis bei genau diesen Winkeln

$$x_1 = \frac{\pi}{2}, \qquad x_2 = \frac{3\pi}{2}$$

Einsetzen in $f(x) = -1 + 2\cos(x)$:

$$
\begin{align*}
&y = -1 + 2\cdot 0 \\ 
&y= -1
\end{align*}
$$

**Schnittpunkte:**
$$S_1 = \left(\frac{\pi}{2};\, -1\right), \qquad S_2 = \left(\frac{3\pi}{2};\, -1\right)$$

---

## Fall 2: $1-2\sin(x) = 0 \implies 2\sin(x) = 1 \implies \sin(x) = \dfrac{1}{2}$

$$x_3 = \frac{\pi}{6}, \qquad x_4 = \pi - \frac{\pi}{6} = \frac{5\pi}{6}$$

**Für $x_3 = \dfrac{\pi}{6}$:**
$$\cos\left(\frac{\pi}{6}\right) = \frac{\sqrt{3}}{2}$$
$$y_3 = -1 + 2\cdot\frac{\sqrt{3}}{2} = \sqrt{3} - 1 \approx 0{,}73$$

**Für $x_4 = \dfrac{5\pi}{6}$:**
$$\cos\left(\frac{5\pi}{6}\right) = -\frac{\sqrt{3}}{2}$$
$$y_4 = -1 + 2\cdot\left(-\frac{\sqrt{3}}{2}\right) = -\sqrt{3} - 1 \approx -2{,}73$$

**Schnittpunkte:**
$$S_3 = \left(\frac{\pi}{6};\, \sqrt{3}-1\right), \qquad S_4 = \left(\frac{5\pi}{6};\, -\sqrt{3}-1\right)$$

---

## Zusammenfassung

| Punkt | $x$-Wert | $y$-Wert (exakt) | $y$-Wert (gerundet) |
|---|---|---|---|
| $S_1$ | $\dfrac{\pi}{2}$ | $-1$ | $-1$ |
| $S_2$ | $\dfrac{3\pi}{2}$ | $-1$ | $-1$ |
| $S_3$ | $\dfrac{\pi}{6}$ | $\sqrt{3}-1$ | $0{,}73$ |
| $S_4$ | $\dfrac{5\pi}{6}$ | $-\sqrt{3}-1$ | $-2{,}73$ |

---

## Probe (Beispiel $S_3$)

$$f\left(\frac{\pi}{6}\right) = -1 + 2\cos\left(\frac{\pi}{6}\right) = -1 + \sqrt{3}$$

$$g\left(\frac{\pi}{6}\right) = -1 + 2\sin\left(\frac{\pi}{3}\right) = -1 + 2\cdot\frac{\sqrt{3}}{2} = -1 + \sqrt{3}$$

$$\Rightarrow f\left(\frac{\pi}{6}\right) = g\left(\frac{\pi}{6}\right) \checkmark$$