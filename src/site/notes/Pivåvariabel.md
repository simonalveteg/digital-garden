---
{"dg-publish":true,"permalink":"/pivavariabel/","tags":["digitalteknik, systemochtransformer"]}
---


The pivot or pivot element is the element of a matrix which is selected by an algorithm (e.g [[Gaussian Elimination\|Gaussian Elimination]]) to do certain calculations.

If during the process a pivot element is zero, then we change rows. If this is not possible because all elements below it are also zero then the system is singular (i.e, the linear system is not uniquely solvable)

A pivot cannot be 0. A small pivot can introduce large numerical errors. Multipliers should be less than 1 in magnitude. **[[Partial Pivoting\|Partial pivoting]]** chooses largest magnitude in column as pivot. This is possible because rows may be interchanged => no [[Swamping\|Swamping]].