## Variational Bayesian Neural Network (VBNN) for Critical Temperature (Tc) Predictive Model

This folder contains the Python implementation of the VBNN model presented in the submitted manuscript "Critical Temperature Prediction for a Superconductor: A Variational Bayesian Neural Network Approach".

===================================================

I. Installation:

This code depends on GPy package[2] and climin package [3].

Note: We used GPy version 1.8.5 with several new files and functions added to support the new model. The following installation requires modifications to GPy package so if you are working on an existing installation of GPy and do not want to make changes to that installation, please consider creating a new Virtual Environment for the following installation. For details on creating Virtual Environment, please refer to: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments .

I.1. Install GPy

We strongly recommend using the anaconda python distribution (https://www.anaconda.com/download/) for easy installation of GPy. We use Anaconda 3 on Windows and Ubuntu systems.
To install GPy, download its source code from its Github repository: https://github.com/SheffieldML/GPy, and follow the installation instruction in Section "Getting started: installing with pip" from that link.
We used GPy version 1.8.5 with several new files and functions added. For these changes to take effect, copy the included GPy folder to overwrite the installation folder of GPy.
Note: The intallation folders of the installed packages are located in the site-packages folder, which you can find out by running: python -c "import site; print(site.getsitepackages())". For example, in my Windows system with Anaconda3, it is located at: C:\Users\usr\Anaconda3\Lib\site-packages.

I.2. Install climin

Download its source code from its Github repository: https://github.com/BRML/climin. Follow the installation instruction from the above link, or follow the following steps:

From command line, change to the downloaded folder
Run: pip install climin
Note: To make climin package to work in Python 3, go to the installation folder of climin (located in the site-packages folder), change line 86 in file climin/util.py (function draw_mini_slices()) to: idxs = list(range(len(slices)))

I.3. For Windows systems, install 'numpy-1.13+mkl' from this page: https://www.lfd.uci.edu/~gohlke/pythonlibs/

===================================================

II. Test script

An example test script is given in the file 'test_hgp.py'. It can be run with: python test_hgp.py

=====================================================

References

[1] J. Shi, J. Chen, J. Zhu, S. Sun, Y. Luo, Y. Gu, and Y. Zhou, “ZhuSuan:A library for Bayesian deep learning,” arXiv preprint arXiv:1709.05870, 2017.

[2] J.  Drugowitsch,  “Variational  bayesian  inference  for  linear  and  logisticregression,”arXiv preprint arXiv:1310.5438, 2013

[3] D. P. Kingma and M. Welling, “Auto-encoding variational bayes,” arXivpreprint arXiv:1312.6114, 2013

