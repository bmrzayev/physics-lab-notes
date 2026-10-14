# Inclined Plane: Motion with Constant Acceleration

Short, formula-focused notes for the undergraduate physics lab on a cart sliding down a (nearly) frictionless incline, timed with two photogates.

## Goals
- Study straight-line motion with constant acceleration on an incline
- Measure the cart's acceleration and compare it with the theoretical value $g\sin\theta$
- Check that the acceleration does not depend on mass
- Get $a$ from the slope of an $x$–$t^2$ graph

## 1. Theory

**Newton's second law:** $\sum \vec F = m\vec a$

**Weight components on an incline of angle $\theta$:**
- Parallel to the surface: $F_\parallel = mg\sin\theta$
- Perpendicular to the surface: $F_\perp = mg\cos\theta$, balanced by the normal force $N = mg\cos\theta$

**Frictionless incline:** the only net force along the slope is $mg\sin\theta$, so

$$mg\sin\theta = ma \;\Rightarrow\; a_{\text{expected}} = g\sin\theta \quad (g = 9.80\ \text{m/s}^2)$$

The mass cancels, so $a$ is independent of mass and always smaller than $g$.

**Constant-acceleration kinematics:**

| Quantity | Formula |
|---|---|
| Velocity | $v = v_0 + at$ |
| Average velocity | $v_{av} = \dfrac{v_0 + v}{2}$ |
| Position | $x = x_0 + v_0 t + \tfrac{1}{2}at^2$ |

**Released from rest** ($x_0 = 0$, $v_0 = 0$): $x = \tfrac12 a t^2$, so

$$a_{\text{experimental}} = \frac{2x}{t^2}$$

## 2. Setup
- Track tilted to $\theta = 10^\circ$, two photogates a distance $x$ apart
- The timer starts when the cart's flag blocks gate 1 and stops when it blocks gate 2
- Release the cart from rest with the flag just before gate 1, so $v_0 \approx 0$
- Repeat for $x = 0.2,\ 0.4,\ 0.6,\ 0.8,\ 1.0$ m

## 3. Procedure
1. Level the track, mount the photogates, and connect them to the timer.
2. Raise one end to $\theta = 10^\circ$.
3. Place the cart with the flag just behind gate 1 (gate 1 unblocked).
4. Start data collection, release the cart, and record $t$ (time between the two blocks).
5. Compute $a = 2x/t^2$ and compare with $g\sin\theta$.
6. Repeat for each gate separation.

## 4. Analysis

**Percent error:**

$$\%\ \text{error} = \frac{|a_{\text{exp}} - a_{\text{expected}}|}{a_{\text{expected}}}\times 100$$

**$x$–$t^2$ graph:** plot $x$ (y-axis) against $t^2$ (x-axis). The points should lie on a straight line through the origin, and

$$\text{slope} = \frac{a}{2} \;\Rightarrow\; a = 2\times\text{slope}$$

A straight line through the origin means the acceleration is constant.

## 5. Worked example ($\theta = 10^\circ$)

$a_{\text{expected}} = 9.80 \sin 10^\circ \approx 1.70\ \text{m/s}^2$

Expected slope of the $x$–$t^2$ graph: $a/2 \approx 0.85\ \text{m/s}^2$

| $x$ (m) | Expected $t = \sqrt{2x/a}$ (s) | Expected $t^2$ (s²) |
|---|---|---|
| 0.2 | 0.485 | 0.235 |
| 0.4 | 0.686 | 0.470 |
| 0.6 | 0.840 | 0.705 |
| 0.8 | 0.970 | 0.940 |
| 1.0 | 1.084 | 1.175 |

## 6. Questions and answers
1. **How does the experimental $a$ compare with $g\sin\theta$?** Calculate the percent error. Small differences come from residual friction, angle and distance measurement, and flag/timing error.
2. **What happens if the cart's mass is doubled?** Nothing, in the ideal case: mass cancels in $a = g\sin\theta$.
3. **Weight components?** Parallel: $mg\sin\theta$. Perpendicular: $mg\cos\theta$.
4. **Free-body diagram:** forces are the weight $mg$ (straight down) and the normal force $N$ (perpendicular to the track). Along the slope, $mg\sin\theta = ma$, so $a = g\sin\theta$.
5. **Does $a$ depend on the ramp angle?** Yes. A larger $\theta$ gives a larger $\sin\theta$ and a larger $a$, so the cart covers more distance per second.

## 7. Sources of error
Friction, angle measurement, gate spacing, flag width, imperfect release from rest.

---
*Notes written for teaching and study purposes. Based on a university inclined-plane lab manual; all text here is my own wording.*
