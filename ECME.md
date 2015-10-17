Title:	ECME
CSS:	http://home.eng.iastate.edu/~ald/ald_files/article.css
xhtml header:	
</script> 

	


Sparse Signal Reconstruction via ECME Hard Thresholding
=======================================================

Kun Qiu and [Aleksandar Dogandžić](http://home.eng.iastate.edu/~ald/index.html)

### Reference:

*IEEE Trans. Signal Processing*, vol.60, pp. 4551-4569, Sep. 2012.
[BibTeX](ECMERef.bib)

### Abstract

We propose a probabilistic model for sparse signal reconstruction and
develop several novel algorithms for computing the maximum likelihood
(ML) parameter estimates under this model. The measurements follow an
underdetermined linear model where the regression-coefficient vector is
the sum of an unknown deterministic sparse signal component and a
zero-mean white Gaussian component with an unknown variance. Our
reconstruction schemes are based on an *expectation-conditional
maximization either (ECME) iteration* that aims at maximizing the
likelihood function with respect to the unknown parameters for a given
signal sparsity level. Compared with the existing iterative hard
thresholding (IHT) method, the ECME algorithm contains an additional
multiplicative term and guarantees monotonic convergence for a wide
range of sensing (regression) matrices. We propose a *double
overrelaxation (DORE)* thresholding scheme for accelerating the ECME
iteration. We prove that, under certain mild conditions, the ECME and
DORE iterations converge to local maxima of the likelihood function. The
ECME and DORE iterations can be implemented exactly in small-scale
applications and for the important class of large-scale sensing
operators with orthonormal rows used e.g. partial fast Fourier transform
(FFT). If the signal sparsity level is *unknown*, we introduce an
*unconstrained sparsity selection (USS)* criterion and a tuning-free
*automatic double overrelaxation (ADORE)* thresholding method that
employs USS to estimate the sparsity level. We compare the proposed and
existing sparse signal reconstruction methods via one-dimensional
simulation and two-dimensional image reconstruction experiments using
simulated and real X-ray CT data.

### Index Terms

Expectation-conditional maximization either (ECME) algorithm, iterative
hard thresholding, sparse signal recon- struction, unconstrained
sparsity selection, successive overrelaxation.

### Full paper download:

[![pdfIcon](pdficon.gif)](ECME.pdf) 
(6.2MB)

### Matlab code download:

(1.7MB) Here is the code for reproducing the results reported in this
paper. Please read the enclosed “Readme” file as well. If you use this
code in your research and publications, please refer to the above paper.

[![zipIcon](zipicon.png)](ECME.tar.gz) 
(6.2MB)
