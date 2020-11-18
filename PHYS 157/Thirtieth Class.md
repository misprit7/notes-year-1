# Thirtieth Class
Nov 15, 2019
* Energy in simple harmonic motion
  * Kinetic energy
    * $K.E.=\frac{1}{2}Mv^2$
  * Potential energy relative to equilibrium
    * $P.E.=\frac{1}{2}k(\Delta x)^2$
    * Derivation: 
      * Let point B be at equilibrium displacement with $V_{max}$, and let $C$ be most stretched out point in SHM (simple harmonic motion)
      * Energy at B relative to mass at equilibrium: $\frac{1}{2}Mv^2_{max}$
      * Total energy at $C$ is the same (conservation of energy), so energy at $C$ is $\frac{1}{2}Mv^2_{max}$
      * Rewriting in terms of $k$ and $A$, we get: 
      * $v_{max}=A\omega=A\sqrt{\frac{k}{m}}$
      * $\frac{1}{2}Mv^2_{max}=\frac{1}{2}MA^2\frac{k}{m}=\frac{1}{2}kA^2$
* Total energy is conserved
  * $\frac{1}{2}Mv^2+\frac{1}{2}kx^2=E=const.$
* Key fact about oscillating systems: energy is proportional to amplitude squared
  * $E_{total}\propto A^2$
* In real oscillators, energy is lost
  * Lost to things like friction, air/fluid drag or heating of the system
  * Amplitude decreases with time
* Common stipulation: Amplitude decreases by approximately the same fraction each full oscillation
  * e.g. 
    * $t=0\to A=A_0$
    * $t=T\to A=A_0\cdot r$
    * $t=2T\to A=A_0\cdot r^2$
    * General $T\to A=A_0\cdot r^{t/T}$
  * We can rewrite this as exponential decay: 
    * $A=A_0e^{-t/t_0}$
    * $t_0=-\frac{T}{\ln{r}}$
    * This work since $e^{-t/t_0}=r^{t/T}$