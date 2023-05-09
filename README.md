# A Review of Sensitivity Methods for Differential Equations 

This respository contains all the text, code and figures used for the review paper about sentitivity methods for differential equations. This topic received different names in different communities, but the core problem is very simple and important. Given a system of differential equations 
```math
\frac{du}{dt} = f(u, \theta, t),
```
with $u \in \mathbb R^n$ the unknow solution and $\theta \in \mathbb R^p$ a vector of parameters, how do we compute the gradient of a loss function 
```math
\mathcal L (\theta) = L ( u(\cdot, \theta) )
```
with respect to the parameters $\theta$ of the dynamical model? 

There are different methods that try to solve this problem, and we had roughly classify them in the following scheeme. 

<p align="center">
	<img src="tex/figures/scheme-methods.png" width="50%">
</p>  
<p align="center">	
	<i>Schematic classification of different methods to compute gradients of functions involving solutions of differential equations.</i>
</p>

The goal of this review is to revisit all this methods and compare them. 

## Code 

We provide code for the different simulations and examples we excibit in the project. Most of this code is provided in the Julia programming language, given that many of the libraries to perform sensitivity analysis are supported there, plus the Julia solver for differential equations are currently the state of the art in scientific computing. 

## How to use? 

This repository is organized in a way that contains most of the important elements of modern scientific workflow. We had included the following elements in this repository:
- `tex`: This is the folder where all the latex text belongs and what we use to compile `main.pdf`. 
- `code`: Folder with both Jupyter notebooks and Julia scripts. 
- `Makefile`: make file that automatizes all the commands that can be executed within this repository. 

### Makefile

Make is an old but very useful technology that allows automation of computing processes. From the directory where you have this respository you can enter `make help` from a terminal to display the different functionalities currently supported in our `Makefile`. We currently support the following operations:
- `make tex`: Compiles the `main.tex` latex file inside the folder `tex` with its respective bibliografy, deletes auxiliaries files in the process and them move the generated pdf file to the home directory. 

## Open Science from Scratch: contribute to the project! 

This review started with some of the authors willing to understand this tools in a comprehensive way and gathering references from fields like statistics, applied mathematics and computer science. Unhappy with the lack of a general compendium of the different methods that exists to address this problem, we had decided to make a single document where all the methods can coexists under common ground and can be compareded under their different scopes and domains of applications. 

We are driving by learning and undersranding and the original authors of this report decided to manage this as an open science project from the beginning. What does this entitles? Anyone interested in participating and contrubuting is welcome to join. We beleive that science will benefit for more open collaborations happening under the basis of people trying to understand a topic. 

<!-- :::note Contribute

Some **content** with _Markdown_ `syntax`.

:::
 -->
 
### Contribute 

We encourage contributors to participate in this project! If you are interested in contributing, there are many ways in which you can help build this:
- Open `Issues` in this repository to report bugs, 

<!-- ## Reference

If you find this article useful, you can cite it as follows 
```

``` -->
