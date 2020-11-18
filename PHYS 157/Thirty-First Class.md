# Thirty-First Class
Nov 18, 2019
* Exponential decay
  * When amplitutde/energy decreases by fixed fraction each period
  * $A=A_0e^{-\frac{-t}{t_0}}$
* Damped Oscillations
  * $x(t)=A_0e^{-\frac{t}{t_0}}\cos(\omega t+\phi)$
* Forces that lead to damping are velocity dependent and opposite direction to velocity
  * e.g. friction or drag forces in air or fluids
* Example: drag forces from air/fluids
  * When $v$ is small, $F=-bv$
  * When $v$ is large, $|F|\propto v^2$
    * When $v$ is large fluids are very hard to model, so we only think about small $v$
  * $F_0=-bv$
  * $F_{net}=-kx-bv$
  * Equations of motion
    * $\frac{dx}{dt}=v$
    * $\frac{dv}{dt}=-\frac{k}{m}x-\frac{b}{m}v$
  * Solution:
    * $x(t)=A_0e^{-\frac{t}{t_0}}\cos(\omega t+\phi)$
    * $t_0=\frac{2m}{b}$
    * $\omega=\sqrt{\frac{k}{m}-\frac{b^2}{4m^2}}$
    * Valid for $b<2\sqrt{km}$
  * When $b=2\sqrt{km}$, it's critical damping and it's pure decay with no iscillations
  * When $b>2\sqrt{km}$, it's overdamped
    * Also exponential decay, but slower to reach equilibrium than critical damping
  * For small $b$, $\omega\approx\omega_{b=0}=\sqrt\frac{k}{m}$
* Forced oscillations
  * We can add in an oscillating force by hand: 
    * $F=F_0\cos(\omega_0 t)$
    * $\omega_0$ is the driving frequency: we can choose this
    * Object will end up oscillating at driving frequency, but amplitude largest if $\omega_D$ matches $\omega_0=\sqrt\frac{k}{m}$
    * This is resonance
    * $A_{max}=\frac{F_0}{\omega_0 b}$