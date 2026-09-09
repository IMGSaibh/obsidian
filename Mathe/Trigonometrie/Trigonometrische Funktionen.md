***
Im rechtwinkligen Dreieck
+ $\color{green}sin(x) = \frac{Gegenkathete}{Hypothenuse}$
+ $\color{blue}\cos(x) = \frac{Ankathete}{Hypotenuse}$
+ $\tan(x) = \frac{Gegenkathete}{Ankathete}$
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
% Punkt auf dem Kreis (cos(30°), sin(30°)) 
% Dreiecksseiten zeichnen 
\draw[thick, red] (O) -- (B) node[midway, above left] {$r=1$}; 
% Hypotenuse 
\draw[thick, blue] (O) -- (A) node[midway, below] {$\cos\alpha$}; 
% Ankathete 
\draw[thick, green] (A) -- (B) node[midway, right] {$\sin\alpha$}; 
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


