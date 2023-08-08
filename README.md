# CTCD-Implementation-and-Methodological-Considerations
Data simulation CTCD in R, simulated data analyses in R, STATA and SPSS.

These scripts are part of the supplementary material of the paper The Co-Twin-Control_design: Implementation and Methodological Considerations, doi:10.1017/thg.2023.35

First, a data simulation was conducted using R to demonstrate the application of the Co-Twin-Control-Design (CTCD) for assessing causality and confounding. Three datasets were generated: one for a population sample, one for a dizygotic (DZ) twin sample, and one for a monozygotic (MZ) twin sample, where the desired samples can be specified by the user. 

Normally distributed continuous variables were generated for both the exposure (x) and the outcome (y) variables by exact data simulation. Subsequently, binary variables (dx and dy) were derived from the continuous variables. All continuous values above zero were assigned a value of one, indicating a positive outcome (‘case’), while the remaining values were assigned a value of zero (‘control’). 

The data simulation implements different scenario's:
Scenario A: No source of confounding.
Scenario B: Solely genetic confounding.
Scenario C: Solely shared environmental confounding
Scenario D: Both genetic and shared environmental confounding.
The simulation scenarios can be customized to incorporate different strengths of association and genetic and non-genetic variance components of x and y based on specific simulation requirements. 

In the current simulation, the variance components for x and y were chosen based on an ACE model (i.e., in this model the variation in a phenotype is due to additive genetic effects (A), the common environment (C), and the unique, random, environment (E)) with a relatively small contribution of C. The simulated exposure variable was based on traits such as victimization, with variance components of a2 = .45, c2 = 0.22, and e2 = 0.33, while the simulated outcome variable represented a trait such as depression, with variance components of a2 = 0.40, c2 = 0.10, and e2 = 0.50.  
