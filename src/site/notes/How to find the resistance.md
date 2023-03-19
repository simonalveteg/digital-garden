---
{"dg-publish":true,"permalink":"/how-to-find-the-resistance/","tags":["elektromagnetiskfältteori"]}
---

How do we calculate the [[Resistans\|resistance]] between two conducting plates? 

From [[Ohm's Law\|Ohm's Law]] we know that 
$$
R=\frac{V}{I}
$$
and we can express both $V$ and $I$ in terms of the [[Electric Field\|electric field]].
$$
V=-\int \vec{E}\cdot d\vec{l} 
$$
$$
I=\iint \vec{J}\cdot d\vec{s}=\iint \sigma\vec{E}\cdot d\vec{s}
$$
Since symmetry can't be used to simplify a line-integral we can't start there. Instead we get an expression of the [[Electric Field\|electric field]] from the current, and plug that into the line-integral of the [[Potential\|potential]]. 

Step by step:

## 1. Set charges and find symmetries
Choose one of the [[Conductor\|conductors]] to be $+Q$ and the other $-Q$.

In this course we can often use symmetry to simplify calculations of integrals. For [[Resistans\|resistance]] calculations symmetry of the [[Electric Field\|electric field]] is immensely helpful. In the case of a cylinder with positive charge on the inner [[Conductor\|conductor]] and negative on the outer we would have
$$
\vec{E}=E(r)\vec{a}_r
$$
since the [[Electric Field\|electric field]] is in the radial direction from the positive to the negative [[Conductor\|conductor]]. 

## 2. Derive an expression for the [[Electric Field\|electric field]]
Using 
$$
I=\iint \vec{J}\cdot d\vec{s}=\iint \sigma\vec{E}\cdot d\vec{s}
$$
Note that the direction of the surface is the same as the direction of $\vec{E}$. If we have symmetry we can move the [[Electric Field\|electric field]] out of the integral, which leaves just $ds$ in the surface integral. $d\vec{s}$ is expressed as the same direction as the current (other directions won't contribute to the integral). Look at the formla sheet to find what to replace $d\vec{s}$ with, depending on which [[Coordinate Systems\|coordinate system]] we are using. If the current flows in the radial direction we want to find $ds_r$ and so on.

In other words,
$$I=\sigma E(r)S \Rightarrow E(R)=\frac{I}{\sigma S}$$

## 3. Perform the line integral
Plug the derived expression of $E(r)$ into the line integral
$$
V=-\int \vec{E}\cdot d\vec{l} 
$$
which gives us the [[Potential\|potential]]. Remember that it's the negative line integral from the negative charge to the positive charge. 

## 4. Get the [[Resistans\|resistance]]
Now we just use [[Ohm's Law\|Ohm's Law]] to get the [[Resistans\|resistance]]!
$$
R=\frac{V}{I}
$$

Quick note about [[Series or parallell connections\|Series or parallell connections]].


# Vince's Version - geometry
In general, calculation of [[Resistans\|resistance]] can be based on the simple concept $R=\frac{l}{\sigma S}$, by recognizing that the [[Conductor\|conductor]] in question can be broken down into small parts, each having an elemental [[Resistans\|resistance]] $dR$ (in which $l,\sigma,S$ are all constants). $l$ is the length of the [[Ohmic Materials\|ohmic material]] with [[Conductivity\|conductivity]] $\sigma$ and cross section area $S$.

1. Choose the appropriate [[Coordinate Systems\|coordinate system]]
2. Identify which of the parameters $l,\sigma,S$ is not constant between the terminals and write it as a function of position along the [[Conductor\|conductor]] (if not already given to you)
3. Identify $dR$ for series or $dG$ (elemental conductance) for parallell connection
4. Calculate [[Resistans\|resistance]] $R$ by integrating $dR$ (or conductance $G$ by integrating $dG$, $R=1/G$)
