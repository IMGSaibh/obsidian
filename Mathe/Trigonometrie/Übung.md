***
### Übung 1
+ Es ist ein Mix aus Rad und Winkel gegeben $$\begin{align}\text{Gegeben:}\quad \sin( \frac{x}{2} - \frac{\pi}{3} ) &= -0.25  \end{align} $$
+ **Schritt 1:** Alles in Winkel umwandeln:
	+ $\text{Rad}: \theta=\frac{x}{2} - \frac{\pi}{3} \to \theta=\frac{x}{2} - 60 \degree$
	+ $Winkel: \implies TR:  \ \alpha = \sin^{-1}(-0.25) = -14.5 \degree$
+ **Schritt 2:** berechnen von $\theta$:
$$
\begin{aligned}
\text{Quadrant I (+):} \quad \theta_1 &= \alpha = 14.48^\circ \\
\text{Quadrant II (+):} \quad \theta_2 &= 180^\circ - \alpha = 165.52^\circ \\
\color{green}\text{Quadrant III (-):} \quad \theta_3 &=\color{green}{ 180^\circ + \alpha = 194.48^\circ} \quad \\
\color{green}\text{Quadrant IV (-):} \quad \theta_4 &= \color{green}{360^\circ - \alpha = 345.52^\circ \quad}
\end{aligned}
$$

+ Weil der Wert $-0.25$ gegeben war, sind ist nur der $\color{green}III$ und $\color{green}IV$ eine echte Lösung 
+ **Schritt 3:** berechnen von $x$
	+ Umstellen: $\theta = \frac{x}{2} - 60 \degree \implies x = 2 \cdot (\theta + 60\degree)$
$$
\begin{align}
x_1 &= 2 \cdot (14.48^\degree + 60^\degree) &&= \mathbf{148.96^\degree} \\
x_2 &= 2 \cdot (165.52^\degree + 60^\degree) &&= \mathbf{451.04^\degree} \pmod{360^\degree} \equiv \mathbf{91.04^\degree} \\
x_3 &= \color{green}{2 \cdot (194.48^\degree + 60^\degree)} &&= \color{green}{\mathbf{508.96^\degree} \pmod{360^\degree} \equiv \mathbf{148.96^\degree}} \\
x_4 &= \color{green}{2 \cdot (345.52^\degree + 60^\degree)} &&= \color{green}{\mathbf{811.04^\degree} \pmod{360^\degree} \equiv \mathbf{91.04^\degree}}
\end{align}
$$
***
### Übung 2
$$\begin{align}\text{Gegeben:}\quad \cos(x) + \cos(2x) = 0 \\   \end{align} $$
+ $\cos(2x)$ so umschreiben, dass nur noch normales $x$ darin vorkommt. Sonst kann Gleichung nicht aufgelöst werden. Nutze Doppelwinkelformeln (Identität)
+ **Für das Kosinus-Doppelwinkel-Theorem gibt es drei Varianten:**
	+ $\cos(2x) = \cos^2(x) - \sin^2(x)$
	+ $\cos(2x) = 1 - 2\sin^2(x)$
	+ $\cos(2x) = 2\cos^2(x) - 1$
+ Wir nutzen die Struktur die exakt wie eine normale quadratische Gleichung aussieht $2u^2+u-1=0$
$$
\begin{align*}
\text{Nutze Identität:} \quad \cos(2x) &= 2\cos^2(x) - 1 \\
\\
\cos(x) + \left(2\cos^2(x) - 1\right) &= 0 \\
2\cos^2(x) + \cos(x) - 1 &= 0 \\
\\
\text{Substitution:} \quad u &= \cos(x) \\
2u^2 + u - 1 &= 0 \\
\\
\text{p-q-Formel:} \quad u_{1,2} &= \frac{-1 \pm \sqrt{1^2 - 4 \cdot 2 \cdot (-1)}}{2 \cdot 2} \\
u_{1,2} &= \frac{-1 \pm \sqrt{9}}{4} = \frac{-1 \pm 3}{4} \\
\\
\implies u_1 = \frac{2}{4} = \frac{1}{2} \quad &\text{und} \quad u_2 = -\frac{4}{4} = -1
\end{align*}
$$
+ $u$ wieder zurück substituieren $u=\cos(x)$
$$
\begin{align*}
\text{Für das Intervall } [0^\circ; 360^\circ]: \\
\textbf{Fall 1:} \quad \cos(x) &= \frac{1}{2} \\
x_1 &= 60^\circ \quad \text{Qudarant I}\\
x_2 &= 300^\circ \quad \text{Qudarant VI}\\
\textbf{Fall 2:} \quad \cos(x) &= -1 \\
x_3 &= 180^\circ \quad \text{nur ein Winkel an position -1 auf dem Einheitskreis}
\end{align*}
$$

***
### Übung 3
$$
\begin{align*}
\cos^{3}x - 2 \cdot \cos x \cdot\sin^2x=0 \\
\cos x (\cos^2x - 2 \cdot \sin^2x)=0 \\
\cos^2x = 1 - \sin^2x \\
\cos x \cdot (1-\sin^2x - 2 \cdot \sin^2x) =0 \\
\cos x \cdot (1-3 \cdot \sin^2x)=0
\end{align*}
$$
