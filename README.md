## Variational Bayesian Neural Network (VBNN) for Critical Temperature (Tc) Predictive Model

This folder contains the Python implementation of the VBNN model presented in the submitted manuscript "Critical Temperature Prediction for a Superconductor: A Variational Bayesian Neural Network Approach".

===================================================

I. Installation:

This code depends on ZhuSuan package[1], variational  Bayesian  inference [2], Stochastic GradientVariational Bayes (SGVB) [3].

Note: We used Tensorflow version 1.14 with several new files and functions added to support the new model. The following packages are required additionaly to run the code. For details on installing Tensorflow,  and neccessary package , please refer to:

TensorFlow: https://www.tensorflow.org/install

ZhuSuan Bayesian Deep Learning: https://zhusuan.readthedocs.io/en/latest/

tensorflow>=1.13.0
Sphinx>=1.7.1
sphinx_rtd_theme
sphinxcontrib-bibtex>=0.3.6
coverage
pep8
matplotlib
mock
scipy
progressbar2
numpy>=1.14.0
six

II. Superconducting Material Database (SuperCon) from this page: https://supercon.nims.go.jp/index_en.html

===================================================

II. Test Result

A test result script is given in the file 'VBNN_HTc.ipynb'. It can be viewed by the link: https://github.com/ltdung/VBNN_HighTc/blob/master/VBNN_HTc.ipynb. In cases of, you find difficulty to view the file, please use: https://nbviewer.jupyter.org/

=====================================================

References

[1] J. Shi, J. Chen, J. Zhu, S. Sun, Y. Luo, Y. Gu, and Y. Zhou, “ZhuSuan:A library for Bayesian deep learning,” arXiv preprint arXiv:1709.05870, 2017.

[2] J.  Drugowitsch,  “Variational  bayesian  inference  for  linear  and  logistic regression,” arXiv preprint arXiv:1310.5438, 2013

[3] D. P. Kingma and M. Welling, “Auto-encoding variational bayes,” arXivpreprint arXiv:1312.6114, 2013

