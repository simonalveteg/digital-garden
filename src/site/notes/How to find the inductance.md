---
{"dg-publish":true,"permalink":"/how-to-find-the-inductance/","tags":["elektromagnetiskfältteori"]}
---

If we have only one [[Spole\|coil]], we are after the [[Self-Inductance\|Self-Inductance]]. If we have two [[Spole\|coils]] or more we are after the [[Mutual Inductance\|Mutual Inductance]].

## 1. Choose a [[Coordinate Systems\|coordinate system]]
Choose the [[Coordinate Systems\|coordinate system]] that makes it as easy as possible to calculate the [[Magnetic Field\|magnetic field]] for one of the circuits.

If you're dealing with a [[Magnetic Dipole\|Magnetic Dipole]] you need to set the [[Coordinate Systems\|coordinate system]] so that the circuit loop goes around the z-axis in other to use the formula in the formula sheet.

## 2. Assume current
Assume the current in one of the circuits. When calculating the [[Mutual Inductance\|Mutual Inductance]] $L_{12}=L_{21}$ one of the calculations is usually a lot easier than the other. $L_{12}$ is how circuit 1 affects circuit 2, and therefore you want to use the current $I_{1}$ and [[Magnetic Field\|magnetic field]] $B_{1}$ and the surface $S_{2}$.

## 3. Find the [[Magnetic Field\|magnetic field]]
Either with [[Biot-Savart Law\|Biot-Savart Law]] or [[Ampere's Circuital Law\|amperes law]] and [[Vector Magnetic Potential\|Vector Magnetic Potential]].

## 4. Find the [[Magnetic Flux Linkage\|magnetic flux linkage]]
Which is $\Lambda=N\Phi$, and
$$
\Phi_{11}=\int_{S_{1}} \vec{B}_1  \, d\vec{s}_1
$$
$$
\Phi_{12}=\int_{S_{2}} \vec{B}_1  \, d\vec{s}_2
$$
## 5. Find inductances
$$
L_{11}=\frac{\Lambda_{11}}{I_1}
$$
$$
 L_{12}=\frac{\Lambda_{12}}{I_1}
$$
# If distance is much greater than the size of the circuit
When the distance between $C_{1}$ and $C_{2}$ is much greater than the size of $C_{2}$, the [[Magnetic Flux\|magnetic flux]] through $C_{2}$ can be calculated as just the [[Magnetic Field\|magnetic flux density]] in the center of the loop multiplied by the surface area. The [[Magnetic Field\|magnetic flux density]] can be seen as practically the same over the entire surface.