# Measurements, Errors and Graphs

Concise notes for a General Physics I lab: using a ruler, vernier caliper, micrometer and graduated cylinder, handling measurement errors, plotting graphs, and finding density.

## 1. Units
SI base quantities used in mechanics: length (m), mass (kg), time (s). Others: current (A), temperature (K), amount of substance (mol), luminous intensity (cd).

| Prefix | Symbol | Power of ten |
|---|---|---|
| femto | f | $10^{-15}$ |
| pico | p | $10^{-12}$ |
| nano | n | $10^{-9}$ |
| micro | μ | $10^{-6}$ |
| milli | m | $10^{-3}$ |
| centi | c | $10^{-2}$ |
| kilo | k | $10^{3}$ |
| mega | M | $10^{6}$ |
| giga | G | $10^{9}$ |
| tera | T | $10^{12}$ |

- **Direct measurement:** read from an instrument (e.g. length with a ruler).
- **Indirect measurement:** calculated from direct ones (e.g. $V = \tfrac43\pi r^3$ from a measured radius).

## 2. Errors
- **Systematic error:** fixed offset from the instrument (e.g. zero error). Correct it by adding or subtracting the offset.
- **Random error:** unpredictable variation. Reduce it by repeating measurements and averaging.
- **Instrument error:** the smallest division the device can read. Result is written $x \pm \Delta x$.
- **Accuracy:** closeness to the true value (affected by systematic error).
- **Precision:** reproducibility (affected by random error).

## 3. Significant figures
1. The leftmost nonzero digit is the most significant.
2. Without a decimal point, the rightmost nonzero digit is the least significant.
3. With a decimal point, the rightmost digit counts, even if it is zero.
4. Everything between counts.

Examples (all 4 s.f.): 6739, 456900, 0.008589, 0.01000, 10.60, 1.057.

**Rounding:** last digit < 5 → drop it; ≥ 5 → drop it and add 1 to the previous digit.
**Multiply/divide:** keep as many s.f. as the least precise number. Example: $3.519 \times 2.3 = 8.0937 \approx 8.1$.
**Add/subtract:** keep as many decimal places as the least precise term. Example: $0.073 + 13.7 + 156 = 169.773 \approx 170$.
**Scientific notation:** one nonzero digit before the decimal point, times a power of 10 (e.g. $4.569\times10^{5}$).

## 4. Errors in calculated results

| Operation | Result | Maximum error |
|---|---|---|
| $x \pm y$ | $(x \pm y)$ | $\Delta x + \Delta y$ |
| $x \cdot y$ | $xy$ | $x\Delta y + y\Delta x$ |
| $x / y$ | $x/y$ | $\dfrac{y\Delta x + x\Delta y}{y^2}$ |

For products and quotients, relative errors add: $\dfrac{\Delta z}{z} = \dfrac{\Delta x}{x} + \dfrac{\Delta y}{y}$.

## 5. Statistics of repeated measurements
- Mean: $\bar x = \dfrac{1}{N}\sum x_i$
- Deviation: $d_i = x_i - \bar x$
- Average deviation: $\text{A.D.} = \dfrac{1}{N}\sum |d_i|$
- Standard deviation: $\sigma = \sqrt{\dfrac{\sum (x_i-\bar x)^2}{N-1}}$
- Absolute error: $\Delta x$ (same units as $x$)
- Fractional error: $\Delta x / x$ (no units)
- Percentage error: $\dfrac{\Delta x}{x}\times 100$

Write the error with the same number of decimal places as the measurement.

## 6. Instruments

**Ruler** (1 mm divisions): error $\pm 1$ mm per reading. For a length found from two end positions, the error is $\pm 2$ mm. Avoid parallax by looking perpendicular to the scale.

**Vernier caliper**
- Parts: main scale, vernier scale, fixed and sliding jaws, locking screw, depth gauge.
- Uses: outside (external) size, inside diameter, depth.
- Check for zero error first. Clean the jaws and the object.
- Reading = main scale value just left of the vernier zero + (aligned vernier line × resolution).
- Example with 0.01 mm resolution: $20\ \text{mm} + 54\times0.01\ \text{mm} = 20.54\ \text{mm}$.

**Micrometer** (0.5 mm pitch screw, 50 thimble divisions)
- Reading = sleeve (mm) + half-mm mark (0.5) + thimble divisions × 0.01 mm.
- Example: $12\ \text{mm} + 0.5 + 16\times0.01 = 12.66 \pm 0.01$ mm.
- Always close with the ratchet stop (until it clicks) for constant force, and check the zero error.

**Graduated cylinder**
- Read the bottom of the meniscus at eye level.
- Water displacement: $V_{\text{object}} = V_2 - V_1$ (final minus initial volume).
- The object must be fully submerged and must not exceed the cylinder's maximum volume.
- If the smallest division is large, half a division can be used as the uncertainty.

**Balances**
- Equal-arm balance: uncertainty equals the smallest mass in the set (10 mg).
- Digital balance: zero (tare) before use, wait for a stable reading.
- Conversions: 1 oz = 28.350 g, 1 dwt = 1.555 g, 1 ct = 0.2 g.

## 7. Volumes and density

| Shape | Volume |
|---|---|
| Rectangular solid | $V = W\,L\,h$ |
| Cube | $V = a^3$ |
| Sphere | $V = \tfrac43\pi r^3$ |
| Cylinder | $V = \pi r^2 L$ |
| Cone | $V = \tfrac13\pi r^2 h$ |
| Cylinder with holes | $V = \pi R^2H - \pi r_1^2h_1 - \pi r_2^2h_2$ |

For round objects, measure the diameter and halve it.

**Density:** $d = \dfrac{m}{V}$ in g/cm³ (CGS) or kg/m³ (SI). $1\ \text{g/cm}^3 = 1000\ \text{kg/m}^3$.

## 8. Graphs
A good graph has: title, labelled axes with units, sensible scale, clear data points, error bars, a best-fit line and a worst-fit line, and the slope and intercept shown.

- Independent variable on the x-axis, dependent on the y-axis.
- Straight line: $y = mx + b$, slope $m = \dfrac{\Delta y}{\Delta x}$ (use two points on the line, not data points).
- Error in slope: $\Delta m = |m - m'|$; error in intercept: $\Delta b = |b - b'|$ ($m', b'$ from the worst line, which must cross the best line).

**Straightening non-linear relations**

| Relation | Plot | Slope |
|---|---|---|
| $y = k/x$ | $y$ vs $1/x$ | $k$ |
| $y = kx^2$ | $y$ vs $x^2$ | $k$ |
| $y = k/x^2$ | $y$ vs $1/x^2$ | $k$ |
| $y = k e^{cx}$ | $\ln y$ vs $x$ | $c$ (intercept $\ln k$) |
| $y = kx^c$ | $\log y$ vs $\log x$ | $c$ (intercept $\log k$) |

**Density from a graph:** plot mass (y) against volume (x) for objects made of the same material. The slope is the density, with error $\Delta m = |m - m'|$.

## 9. Practice exercises

**Task 1.** How many significant figures does 0.01000 have?
**Answer:** 4 (the leading zeros are not significant, the trailing zeros after the decimal point are).

**Task 2.** The ends of an object read 20.0 cm and 21.6 cm on a ruler with ±1 mm per reading. Give the length with its error.
**Answer:** $L = 1.6 \pm 0.2$ cm (= $16 \pm 2$ mm).

**Task 3.** A micrometer sleeve reads 12.5 mm and the thimble line 16 coincides with the datum line. What is the reading?
**Answer:** $12.5 + 16\times0.01 = 12.66 \pm 0.01$ mm.

**Task 4.** On a caliper the vernier zero lies between 20 and 21 mm and the 54th line aligns (resolution 0.01 mm). What is the reading?
**Answer:** $20 + 54\times0.01 = 20.54$ mm.

**Task 5.** A cube has $a = 2.00 \pm 0.01$ cm. Find $V \pm \Delta V$.
**Answer:** $V = 8.00$ cm³. Relative error $= 3\times0.01/2.00 = 1.5\%$, so $\Delta V = 0.12$ cm³. $V = 8.00 \pm 0.12$ cm³.

**Task 6.** A sample has $m = 54.0 \pm 0.1$ g and $V = 20.0 \pm 0.5$ cm³. Find the density with its error.
**Answer:** $d = 2.70$ g/cm³. Relative error $= 0.1/54.0 + 0.5/20.0 \approx 0.027$, so $\Delta d \approx 0.07$. $d = 2.70 \pm 0.07$ g/cm³.

**Task 7.** The initial water level is $100 \pm 5$ mL and the final level is $118 \pm 5$ mL. Find the object's volume.
**Answer:** $V = 18 \pm 10$ mL (errors add).

**Task 8.** For $y = k/x^2$, what should you plot to get a straight line?
**Answer:** $y$ versus $1/x^2$; the slope is $k$.

**Task 9.** Five readings: 12.1, 12.3, 12.2, 12.4, 12.0. Find the mean, average deviation and standard deviation.
**Answer:** Mean $= 12.2$. Deviations: −0.1, +0.1, 0, +0.2, −0.2, so A.D. $= 0.12$. $\sigma = \sqrt{0.10/4} \approx 0.16$.

---
*Study notes written in my own words, based on a university General Physics I lab manual.*
