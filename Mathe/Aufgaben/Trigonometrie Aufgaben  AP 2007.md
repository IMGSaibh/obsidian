***
## Aufgabe 4.1.1
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

##### Fall 1: $2\cos(x) \implies \cos(x) = 0$
+ cos(x)=0 bedeutet der Punkt hat x-Koordinate 0
	+ cos(x) meint hier $\cos(\alpha)=0$
	+ also Winkel ist 0 und damit ist man auf der x--Achse unterwegs
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
$$\color{green}S_1 = \left(\frac{\pi}{2};\, -1\right), \qquad S_2 = \left(\frac{3\pi}{2};\, -1\right)$$

---

#### Fall 2: $1-2\sin(x) = 0 \implies 2\sin(x) = 1 \implies \sin(x) = \dfrac{1}{2}$
+ Im TR $\implies x=\arcsin\left( \frac{1}{2} \right) \implies \sin^{-1}\left( \frac{1}{2} \right) = 30 \degree = \frac{\pi}{6}$

$$x_3 = \frac{\pi}{6}, \qquad x_4 = \pi - \frac{\pi}{6} = \frac{5\pi}{6}$$

+ Sobald man die **erste** Lösung kennt $x_3 = \frac{\pi}{6}$, findet man die zweite nicht durch erneutes Rechnen, sondern durch eine **Symmetrieeigenschaft** des Sinus.
+ zeichne eine **waagrechte Linie** auf der Höhe $y=12y = \frac12 y=21$​ ein. Diese Linie schneidet den Kreis an **zwei** Stellen:

- einmal **rechts** von der senkrechten Achse (das ist unser $\frac{\pi}{6}$, also 30°)
- einmal **links** von der senkrechten Achse (spiegelverkehrt dazu)
- Diese Spiegelung wird durch folgende Identität beschrieben:
	- $sin⁡(π−x)=sin(x)$
- **Warum das gilt:** Der Punkt bei Winkel $x$ und der Punkt bei Winkel $(π−x)$ sind Spiegelbilder zueinander
- Wenn $x3=\frac{\pi}{6}$ ​ eine Lösung von $sin⁡(x)=\frac{1}{2}$​ ist, dann ist automatisch auch: 
$$
\begin{align*}
x_{4}&=\pi - x_{3} \\
&=\pi-\frac{\pi}{6} \\
&=\frac{6\pi}{6} - \frac{\pi}{6} \\
&=\frac{5\pi}{6}
\end{align*}
$$
***

```tikz
\usepackage{tikz}
\begin{document}
\begin{tikzpicture}[scale=5]

% Einheitskreis
\draw[thick] (0,0) circle (1);

% Achsen
\draw[->] (-1.3,0) -- (1.3,0) node[right] {$\cos(x)$};
\draw[->] (0,-1.3) -- (0,1.3) node[above] {$\sin(x)$};

% Waagrechte Hilfslinie bei y = 0.5
\draw[dashed, gray] (-1.1,0.5) -- (1.1,0.5) node[right, black] {$y=\frac{1}{2}$};

% Punkt bei pi/6 (30°)
\coordinate (P1) at (cos{30}, sin{30});
\filldraw[red] (P1) circle (0.02);
\draw[red, thick] (0,0) -- (P1);
\node[above right, red] at (P1) {$x_3=\frac{\pi}{6}$};

% Punkt bei 5pi/6 (150°)
\coordinate (P2) at (cos{150}, sin{150});
\filldraw[blue] (P2) circle (0.02);
\draw[blue, thick] (0,0) -- (P2);
\node[above left, blue] at (P2) {$x_4=\frac{5\pi}{6}$};

% Winkelbögen
\draw[red] (0.3,0) arc (0:30:0.3);
\draw[blue] (0.3,0) arc (0:150:0.3);

% Senkrechte Linien zur x-Achse (zeigen cos-Wert = unterschiedlich)
\draw[red, dotted] (P1) -- (cos{30}, 0);
\draw[blue, dotted] (P2) -- (cos{150}, 0);

% Gemeinsame Höhe (sin-Wert) hervorheben
\draw[green!60!black, thick, <->] (1.15,0) -- (1.15,0.5);
\node[right, green!60!black] at (1.15,0.25) {$\sin=\frac12$};

\end{tikzpicture}
\end{document}
```
***
**Für $x_3 = \dfrac{\pi}{6}$:**
$$\cos\left(\frac{\pi}{6}\right) = \frac{\sqrt{3}}{2}$$
$$y_3 = -1 + 2\cdot\frac{\sqrt{3}}{2} = \sqrt{3} - 1 \approx 0{,}73$$

**Für $x_4 = \dfrac{5\pi}{6}$:**
$$\cos\left(\frac{5\pi}{6}\right) = -\frac{\sqrt{3}}{2}$$
$$y_4 = -1 + 2\cdot\left(-\frac{\sqrt{3}}{2}\right) = -\sqrt{3} - 1 \approx -2{,}73$$

**Schnittpunkte:**
$$\color{green}S_3 = \left(\frac{\pi}{6};\, \sqrt{3}-1\right), \qquad S_4 = \left(\frac{5\pi}{6};\, -\sqrt{3}-1\right)$$
***
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
***
## Aufgabe 4.1.1
```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[scale=1]
\begin{axis}[
axis lines = middle,
xlabel = $x$,
ylabel = $y$,
xtick = {0, pi/2, pi, 3*pi/2, 2*pi},
xticklabels = {$0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$},
ytick = {-3,-2,-1,1,2,3},
ymin = -4,
ymax = 4,
domain = 0:2*pi,
samples = 200,
width = 14cm,
height = 6cm,
xlabel style={below right},
ylabel style={above left},
legend style={at={(1.02,0.5)}, anchor=west},
]
% Parameter a festlegen
\pgfmathsetmacro{\a}{1}

\addplot[blue, thick] {-\a + 2*\a*cos(deg(x))};
\addlegendentry{$f_a(x) = -a+2a\cos(x)$}

\addplot[red, thick] {-\a + 2*sin(deg(2*x))};
\addlegendentry{$g_a(x) = -a+2\sin(2x)$}

\end{axis}
\end{tikzpicture}
\end{document}
```

