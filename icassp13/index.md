
Title:	MAC Beam Hardening Correction
CSS:	article.css
BibTeX:	
Biblio Style:	IEEEtran

xhtml header:	<script 
type="text/x-mathjax-config">MathJax.Hub.Config({TeX: { equationNumbers: { 
    autoNumber: "AMS" } }}); MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [ ['$','$'], ['\\(','\\)'] ]
  }
});
</script> 
<script type="text/x-mathjax-config">
  MathJax.Hub.Config({ TeX: { extensions: ["color.js"] }});
</script>
<script type="text/javascript"
  src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
	
# Beam Hardening Correction via Mass Attenuation Discretization

[Renliang Gu](http://co3125-07.ece.iastate.edu/renliang/) and
[Aleksandar Dogandžić](http://home.eng.iastate.edu/~ald/index.html)

### Reference:
*Proc. IEEE Int. Conf. Acoust., Speech, Signal Process.*, Vancouver,
Canada, May 2013, to appear.  [BibTeX](MAC.bib)

### Abstract

We develop a beam-hardening correction method for polychromatic
X-ray CT reconstruction based on *mass attenuation
coefficient discretization*. We assume that the inspected object
consists of an unknown single material and that the incident
X-ray spectrum is unknown. In this case, the standard
photon-energy discretization of the Beer's law measurement equation
leads to an excessive number of unknown parameters and scaling
ambiguity. To obtain a parsimonious measurement model
parametrization, we first rewrite the measurement equation in terms
of integral expressions of the mass attenuation rather than photon
energy. The resulting integrals can be discretized easily thanks to
the fact that the range of mass attenuations is bounded and, in
practice, fairly narrow. We then develop a constrained least-squares
optimization approach for reconstructing the underlying object from
log-scale measurements, where we impose the nonnegativity constraint
to both the signal and the X-ray spectrum density
estimates. We demonstrate the performance of the proposed method via
a numerical example where we compare it with the standard FBP, which 
ignores the polychromatic nature of the measurements.

### Index Terms

Beam hardening, computed tomography, signal reconstruction, X-ray 
tomography.

<!---
### Main Idea
~~~
{}{img_left}{lebesgue.jpg}{lebesgue}{200px}{}{}
*Assumption:*
- Both incident spectrum {{$\iota(\varepsilon)$}} and mass attenuation
  function {{$\mu(\varepsilon)$}} of the object are *unknown*.

*Objective:*
- Estimate the density map {{$\alpha(x,y)$}}.

Based on the fact that mass attenuation {{$\mu(\\\\varepsilon)$}} and incident spectrum density {{$\iota(\\\\varepsilon)$}} are both functions of {{$\\\\varepsilon$}}, our *idea* is to:
- write the model as integrals of {{$\mu$}} rather than {{$\\varepsilon$}};
- estimate {{$\iota(\varepsilon(\mu)) |\varepsilon'(\mu)|$}} rather than {{$\iota(\varepsilon)$}} and {{$\mu(\varepsilon)$}}.
~~~

~~~
{}
For invertible {{$\mu(\\\\varepsilon)$}}, define its inverse as {{$\\\\varepsilon(\mu)$}} and  
~~~

~~~
{}{raw}
\[
    \mathcal{I}^{\mathrm{in}} = \int \iota(\varepsilon(\mu)) |\varepsilon'(\mu)| d\mu, \qquad
    \mathcal{I}^{\mathrm{out}} = \int \iota(\varepsilon(\mu)) |\varepsilon'(\mu)|
    \exp\Bigl[ -\mu \int_\ell \alpha(x,y)  d\ell\Bigr] d\mu
\]
~~~
-->

### Full paper download:
[![pdfIcon](pdficon.gif)](icassp13.pdf) 
(1.2MB)

### Poster for download:
[![pdfIcon](pdficon.gif)](posterICASSP.pdf) 
(2.5MB)

<!---
### Matlab code download:

(1.7MB) Here is the code for reproducing the results reported in this
paper. Please read the enclosed “Readme” file as well. If you use this
code in your research and publications, please refer to the above paper.

[![zipIcon](zipicon.png)](icassp13.tar.gz) 
(6.2MB)
-->

