***
### Umrechnungen
+ Umfang des Kreises
	+ $U=2\pi * r = 1$
+ $360\degree = 2\pi$
+ Periode: $\pi$
+ $\sin^2(30\degree) = (\sin(30\degree))^2 = 0.5^2 = 0.25$
	+ Es bedeutet, dass du zuerst ganz normal den Sinus von $x$ berechnest und **das Endergebnis** danach hoch 2 nimmst.
+ **Doppelwinkelsatz (oder die Doppelwinkelformeln)** in der Trigonometrie
	+ Sinus des doppelten Winkels
		+ $\sin(2\alpha) = 2 \cdot \sin(\alpha) \cdot \cos(\alpha)$
	+ Kosinus des doppelten Winkels
		+ $\cos(2\alpha)=\cos^2(\alpha)-\sin^2(\alpha)$
		+ $\cos(2\alpha)=2\cdot \cos^2(\alpha)-1$
		+ $\cos(2\alpha)=1-2\cdot \sin^2(\alpha)$
	+ Tangens des doppelten Winkels
		+ $\tan(2\alpha)=\frac{2\cdot \tan(\alpha)}{1-\tan^2(\alpha)}$

### Punkt auf dem Einheitskreis
+ Ein Punkt im Einheitskreis Winkel x hat die Koordinaten:
+ $P(x)=(\cos(x); \sin(x))$
### Im rechtwinkligen Dreieck
+ $\color{green}sin(x) = \frac{Gegenkathete}{Hypothenuse}$
+ $\color{blue}\cos(x) = \frac{Ankathete}{Hypotenuse}$
+ $\color{violet}\tan(x) = \frac{Gegenkathete}{Ankathete}$

```tikz
\begin{document}
\begin{tikzpicture}[>=stealth, scale=3] 
\draw[->, thick] (-3,0) -- (3,0) node[right] {$x$}; 
\draw[->, thick] (0,-3) -- (0,3) node[above] {$y$};
%\node[below left] at (0,0) {$0$}; %
% Einheitskreis zeichnen (Radius r = 1) 
\draw[thick, gray] (0,0) circle (1);
\node[font=\Large\bfseries] at (2, 2) {I};  
\node[font=\Large\bfseries] at (-2, 2) {II}; 
\node[font=\Large\bfseries] at (-2, -2) {III};  
\node[font=\Large\bfseries] at (2, -2) {IV}; 
\draw[lightgray, very thin] (-2.9,-2.9) grid (2.9,2.9);

%Dreieck im 1. Quadranten 
\coordinate (O) at (0,0); 
\coordinate (A) at (0.866,0); 
\coordinate (B) at (0.866,0.5);
\coordinate (T_start) at (1,0); 
% Schnittpunkt Tangente/Hypotenu
% Punkt auf dem Kreis (cos(30°), sin(30°)) 
\coordinate (T_end) at (1,0.577); 
% 4. DRAW: Verlängerung der Hypotenuse bis zur Tangente 
\draw[thick, red, dashed] (B) -- (T_end);
% 5. DRAW: Tangens-Strecke (auf der Berührlinie bei x = 1)
\draw[thick, violet, <->] (T_start) -- (T_end) node[midway, right] {$\tan\alpha$};


% Dreiecksseiten zeichnen 
\draw[thick, red] (O) -- (B) node[midway, above left] {$r=1$};
% Hypotenuse 
\draw[thick, blue] (O) -- (A) node[midway, below] {$\cos\alpha$}; 
% Ankathete 
\draw[thick, green] (A) -- (B) node[midway, left] {$\sin\alpha$}; 
% Gegenkathete 
% Rechten Winkel markieren (Punkt A) 
\draw (0.816,0) -- (0.816,0.05) -- (0.866,0.05); 
\fill (0.84,0.025) circle (0.2pt); 
% Winkel alpha einzeichnen 
\draw[->] (0.2,0) arc (0:30:0.2); 
\node at (15:0.28) {$\alpha$};

\end{tikzpicture}
\end{document}
```
***
+ Funktionen 1:
```tikz
\usepackage{pgfplots} 
\begin{document} 
\begin{tikzpicture}[scale=1] 
\begin{axis}[ 
axis lines = middle, 
xlabel = $x$, 
ylabel = $y$, 
xtick = {0, pi/2, pi, 3*pi/2, 2*pi, 5*pi/2, 3*pi, 7*pi/2, 4*pi}, 
xticklabels = {$0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$, $\frac{5\pi}{2}$, $3\pi$, $\frac{7\pi}{2}$, $4\pi$}, 
ytick = {-1, 1}, 
ymin = -1.3, 
ymax = 1.3, 
domain = 0:4*pi, 
samples = 200, 
width = 14cm, 
height = 6cm, 
xlabel style={below right}, 
ylabel style={above left}, ] 
\addplot[green, thick] {sin(deg(x))}; 
\addplot[blue, thick] {cos(deg(x))};
\addplot[violet, thick] {tan(deg(x))}; 
\end{axis} 
\end{tikzpicture} 
\end{document}
```

***
### Taschenrechner
+ Wenn Verhältnis gegeben
	+ **$\sin( \frac{1}{2}$)** -> für den Winkel im TR arcsinus eingeben: **$\sin^{-1} (\frac{1}{2}) = 30 \degree$**
+ Wenn Winkel gegeben $\sin (30\degree) = \frac{1}{2}$
	+ Der Winkel im ersten Quadrant $I$
	+ Quadrant $II:180 \degree \cdot 30 \degree = 150 \degree$
+ **Beispiel sin(x) Quadrant $I$ und $II$**
	+ Gegeben: 0.515
		+ Quadrant $I :$ TR Eingabe $\alpha = \sin^{-1} (0.515) = 31 \degree$
		+ Quadrant $II: 180 \degree - \alpha \degree = 149 \degree$
		+ Quadrant $III: 180 \degree + \alpha = 211\degree$
		+ Quadrant $IV: 360 \degree - \alpha = 329\degree$
+ Beispiel cos(x)
	+ **Positiv (+)** ist der Kosinus im **1. und 4. Quadranten**.
	- **Negativ (-)** ist der Kosinus im **2. und 3. Quadranten**.
	+ Gegeben $\cos(-0.8)$ und Referenzwinkel $\cos(0.8)$
		+ $II: \cos^{-1}(-0.8) = 143.130$
		+ $III: 360 \degree - 143.130 \degree = 216.9 \degree$
		+ $I: \cos^{-1}(0.8) = 36.87 \degree$
		+ $IV: 360 \degree - 36.87 \degree = 323.13 \degree$
***
+ Funktionen 2:

```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[scale=1]
\begin{axis}[
axis lines = middle,
xlabel = $x$,
ylabel = $y$,
xtick = {0, pi/2, pi, 3*pi/2, 2*pi, 5*pi/2, 3*pi, 7*pi/2, 4*pi},
xticklabels = {$0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$, $\frac{5\pi}{2}$, $3\pi$, $\frac{7\pi}{2}$, $4\pi$},
ytick = {-1, 1},
ymin = -2.3,
ymax = 2.3,
domain = 0:4*pi,
samples = 200,
width = 14cm,
height = 6cm,
xlabel style={below right},
ylabel style={above left},
legend style={at={(1.02,0.5)}, anchor=west},
]
\addplot[green, thick] {2*sin(deg(x))};
\addlegendentry{$2\sin(x)$}
\addplot[blue, thick] {0.5*sin(deg(x))};
\addlegendentry{$\frac{1}{2}\sin(x)$}
\addplot[violet, thick] {sin(deg(x))};
\addlegendentry{$\sin(x)$}
\end{axis}
\end{tikzpicture}
\end{document}
```

+ Funktionen 3:
```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[scale=1]
\begin{axis}[
axis lines = middle,
xlabel = $x$,
ylabel = $y$,
xtick = {-3*pi/2, -pi, -pi/2,0, pi/2, pi, 3*pi/2, 2*pi, 5*pi/2, 3*pi, 7*pi/2, 4*pi},
xticklabels = {$-\frac{3\pi}{2}$, $-\pi$, $-\frac{\pi}{2}$, $0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$, $\frac{5\pi}{2}$, $3\pi$, $\frac{7\pi}{2}$, $4\pi$},
ytick = {-1, 1},
ymin = -2.3,
ymax = 2.3,
domain = -2*pi:4*pi,
samples = 200,
width = 14cm,
height = 6cm,
xlabel style={below right},
ylabel style={above left},
legend style={at={(1.02,0.5)}, anchor=west},
]
\addplot[red, thick] {sin(deg(x-pi/2))};
\addlegendentry{$\sin(x-\frac{\pi}{2})$}
\addplot[blue, thick] {sin(deg(x+pi/2))};
\addlegendentry{$\sin(x+\frac{\pi}{2})$}
\end{axis}
\end{tikzpicture}
\end{document}
```
+ Funktionen 4: 
```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[scale=1]
\begin{axis}[
axis lines = middle,
xlabel = $x$,
ylabel = $y$,
xtick = {-3*pi/2, -pi, -pi/2,0, pi/2, pi, 3*pi/2, 2*pi, 5*pi/2, 3*pi, 7*pi/2, 4*pi},
xticklabels = {$-\frac{3\pi}{2}$, $-\pi$, $-\frac{\pi}{2}$, $0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$, $\frac{5\pi}{2}$, $3\pi$, $\frac{7\pi}{2}$, $4\pi$},
ytick = {-2,-1,1,2},
ymin = -2.5,
ymax = 2.5,
domain = -2*pi:4*pi,
samples = 200,
width = 14cm,
height = 6cm,
xlabel style={below right},
ylabel style={above left},
legend style={at={(1.02,0.5)}, anchor=west},
]
\addplot[red, thick] {1.5*sin(deg(2*x+pi/2))};
\addlegendentry{$1.5\sin(2x+\frac{\pi}{2})$}
\end{axis}
\end{tikzpicture}
\end{document}
```
+ Funktionen 5:
```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[scale=1]
\begin{axis}[
axis lines = middle,
xlabel = $x$,
ylabel = $y$,
xtick = {-3*pi/2, -pi, -pi/2,0, pi/2, pi, 3*pi/2, 2*pi, 5*pi/2, 3*pi, 7*pi/2, 4*pi},
xticklabels = {$-\frac{3\pi}{2}$, $-\pi$, $-\frac{\pi}{2}$, $0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$, $\frac{5\pi}{2}$, $3\pi$, $\frac{7\pi}{2}$, $4\pi$},
ytick = {-2,-1,1,2},
ymin = -2.5,
ymax = 2.5,
domain = -2*pi:4*pi,
samples = 200,
width = 14cm,
height = 6cm,
xlabel style={below right},
ylabel style={above left},
legend style={at={(1.02,0.5)}, anchor=west},
]
\addplot[blue, thick] {sin(deg(x)};
\addlegendentry{$\sin(x)$}
\addplot[red, thick] {cos(deg(x)};
\addlegendentry{$\cos(x)$}
\end{axis}
\end{tikzpicture}
\end{document}
```
 