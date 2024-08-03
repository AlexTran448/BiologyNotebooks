# BiologyNotebooks
Various google colab notebooks investing protein predictions, alignment, evolutionary model simulations.. ect.

## Protein prediction
This notebook checks if it is feasible to estimate the protein concentration using mRNA concentration

mRNA and protein concentrations are weakly correlated.

Some mRNA has a greater influence on protein concentration, such as those present in the ribosome.
This is due to the ribosome being the site of protein sythesis.

notebook includes diagrams using linear regression to identify lines of best fit

## Needleman_wrunch
Uses blosum50 scoring matrix to check the alignment between 2 different protein sequences.
Alignment is done with own implementation of needleman wrunch and smith waterman algorithms.
Notebook includes diagrams created using matplotlib and scipy to visually show the alignment matrix used.
Includes arrows which shows if a indel (gap) or subsitution is present.
This is done so manually checking for faults is easier for the user (myself). 

Notebook also includes the veterbi algorithm, which is used to predict if the state enterio bacteriophage is AT or CG.
Contains implementations standard veterbi to find the most likely states at each step and the soft output veterbi algorithm to get probabilities.
This algorithm tends to struggle predicting when the states shift rapidly.

## Fisher_Wright
This notebook makes population simulations on how the population of mutants change over time.
Begins by comparing a finite population to an infinite population (shows increasing the finite population increases the similarity to the infinite population).
Uses the Markov models to get the likelyhood of different percentages of mutant populations over time.
Compares the markov model and multiple runs of the fisher wright models.
Implements and shows the difference between markov and fisher wright models.
