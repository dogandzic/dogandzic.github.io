Title:	MPEM
CSS:	http://home.eng.iastate.edu/~ald/ald_files/article.css
xhtml header:	
</script> 

	


A Max-Product EM Algorithm for Reconstructing Markov-tree Sparse Signals from Compressive Samples
=======================================================

Zhao Song and [Aleksandar Dogandžić](http://home.eng.iastate.edu/~ald/index.html)

### Reference:

*IEEE Trans. Signal Processing*, vol. 61, 2013, vol. 61, no. 23, pp. 5917–5931, 2013.
[BibTeX](MPEMRef.bib)

### Abstract

We propose a Bayesian expectation-maximization (EM) algorithm for reconstructing Markov-tree sparse signals via belief propagation. The measurements follow an underdetermined linear model where the regression-coefficient vector is the sum of an unknown approximately sparse signal and a zero-mean white Gaussian noise with an unknown variance. The signal is composed of large- and small-magnitude components identified by binary state variables whose probabilistic dependence structure is described by a Markov tree. Gaussian priors are assigned to the signal coefficients given their state variables and the Jeffreys’ noninformative prior is assigned to the noise variance. Our signal reconstruction scheme is based on an em iteration that aims at maximizing the posterior distribution of the signal and its state variables given the noise variance. We construct the missing data for the em iteration so that the complete-data posterior distribution corresponds to a hidden Markov tree (HMT) probabilistic graphical model that contains no loops and implement its maximization (M) step via a max-product algorithm. This EM algorithm estimates
the vector of state variables *as well as* solves iteratively a linear system of equations to obtain the corresponding signal estimate. We select the noise variance so that the corresponding estimated signal and state variables obtained upon convergence of the EM iteration have the largest marginal posterior distribution. We compare the proposed and existing state-of-the-art reconstruction methods via signal and image reconstruction experiments.

### Index Terms

 Belief propagation, compressed sensing,
expectation-maximization algorithms, hidden Markov models,
 signal reconstruction.


### Full paper download:

[![pdfIcon](pdficon.gif)](MPEM.pdf) 
(5.9 MB)

### Matlab code download:

Here is the code for reproducing the results reported in this
paper. Please read the enclosed “Readme” file as well. If you use this
code in your research and publications, please refer to the above paper.

[![zipIcon](zipicon.png)](MPEM_V1.0.zip) 
(1.1 MB)
