# mackskill-matlab
Nonparametric Two-way ANOVA Used For Block Designs with Unequal Numbers of Multiple Observations

The Mack-Skillings statistical test is a nonparametric two-way ANOVA used for unbalanced incomplete block designs, when the number of observations in each treatment/block pair is one or greater. The test is equivalent to the Friedman test when the observations are balanced. 

Syntax: 
[p stats] = mackskill(response, treatments, blocks) 
[p stats] = mackskill(M, reps) 

Example: 
load popcorn 
friedman(popcorn,3) 
mackskill(popcorn,3) 
popcorn(5) = NaN; 
mackskill(popcorn,3) 

Mack, G. A., & Skillings, J. H. (1980). A Friedman-Type Rank Test for Main Effects in a 2-Factor Anova. Journal of the American Statistical Association, 75(372), 947-951.
Hollander, M., & Wolfe, D. A. (1999). Nonparametric statistical methods (2nd ed.). New York: Wiley.

