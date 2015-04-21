# PseudoSpectralPython
A short course in pseudospectral collocation methods for wave equations, with implementations in Python.


###### Content provided under a Creative Commons Attribution license, CC-BY 4.0; code under MIT License. (c)2015 [David I. Ketcheson](http://davidketcheson.info)

##### Version 0.1 - April 2015

Welcome to PseudoSpectralPython, a short course that will teach you how to solve wave equations using pseudospectral collocation methods.  This notebook zero is just some preliminary material.  If you want to dive in, just skip to [the first notebook](./PSPython_01-linear-PDEs.ipynb)!

###Table of contents:

- [Course scope](#course-scope)
- [Pre-requisites](#pre-requisites)
- [Additional resources](#additional-resources)
- [Errors, suggestions, etc.](#errors,-suggestions,-etc.)

## Course scope

Pseudospectral methods are one of the simplest and fastest ways to solve many nonlinear or variable-coefficient wave equations, including

- [Navier-Stokes](http://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_equations) (fluid flow; both compressible and incompressible)
- [Korteweg-de Vries](http://en.wikipedia.org/wiki/Korteweg%E2%80%93de_Vries_equation) (water waves)
- [Nonlinear Schrodinger](http://en.wikipedia.org/wiki/Nonlinear_Schr%C3%B6dinger_equation) (photonics)

and more.  Pseudospectral methods are best suited to simple geometries, and in this short course we'll only consider periodic Cartesian domains.  The benefit of this is that we can get our hands on interesting solutions of complicated wave equations with relatively little code and with only the computing power in your laptop.

As this course is fast-paced and hands-on, we will not spend much time on deriving physical models or mathematical justifications.  Such topics are better suited to a textbook format, and there are many good resources already available.

## Pre-requisites

### Python

The code for this course is written in Python, which is a programming language designed to promote code that is easy to read and write.  Python has become one of the most important languages in scientific computing.  It is high-level like MATLAB, but unlike MATLAB it is free and is intended as a general-purpose language.

You should know a little Python before starting the course.  In particular, you should be familiar with the packages [numpy](http://www.numpy.org/) and [matplotlib](http://matplotlib.org/).  If you aren't, a good place to start is [Lesson 0 of the HyperPython course](http://nbviewer.ipython.org/github/ketch/HyperPython/blob/master/Lesson_00_Python.ipynb).  If you're completely new to Python, or to programming in general, you may wish to go through one of the many great free online Python tutorials available on the web.

[IPython](http://www.ipython.org) is a collection of tools for interactive programming in Python.  Most importantly for us, IPython includes an interactive shell and a browser-based notebook, now known as the Jupyter notebook.  You will need at least version 3 of IPython in order to open the notebooks for this course.

### Mathematics

The course will make more sense if you have had a course in partial differential equations, including Fourier transforms.  Some basic complex analysis and theory of ordinary differential equations will also serve you well.  However, none of the lessons are intended to be mathematically rigorous, and it's certainly possible to work through them with a less complete background.

### Software

To run the code in this course, you'll need an installation of Python, numpy, matplotlib, and IPython (version >= 3.0).  The easiest way to get them all is to use [SageMathCloud](http://cloud.sagemath.org) -- just create a free account, start a new project, open a terminal, and type
    
    git clone git@github.com:ketch/PseudoSpectralPython.git
   
Open the first notebook there and you're off.

You can also use [Wakari](http://wakari.io), or install everything locally on your own machine.  For local installation, [Anaconda](https://store.continuum.io/cshop/anaconda/) is convenient, or you can just use pip.  All of these are free.

## Additional Resources

This course has benefitted from my own reading of several texts.  I strongly recommend any of the following for a much more thorough introduction to spectral methods:

- *Spectral methods in MATLAB*, by L. N. Trefethen.  Very accessible and includes MATLAB code demonstrating everything.  My favorite introduction.  Some of the codes in PseudoSpectralPython benefitted directly from codes in this book.
- *Chebyshev and Fourier Spectral Methods*, by John Boyd.  Very verbose and with lots of diagrams.  Especially relevant to this course are the following chapters: 4, 9, 10, 11, 12, 13, 14.
- *A Practical Guide to Pseudospectral Methods*, by Bengt Fornberg.  Much more concise than Boyd's text, and in a similar vein.

The three books above are similar to PseudoSpectralPython in that they are aimed at practitioners and de-emphasize purely theoretical aspects.  For a more purely mathematical treatment, I recommend *Spectral Methods for Time-Dependent Problems* by Hesthaven, Gottlieb, and Gottlieb.


## Errors, suggestions, etc.

If you notice anything that could be improved -- or if you want to contribute an example, exercise, or lesson to the course -- please [raise an issue](https://github.com/ketch/PseudoSpectralPython/issues), [send a pull request](https://github.com/ketch/PseudoSpectralPython/pulls), or simply [email me](mailto:dketch@gmail.com).