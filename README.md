# Graph Matching package: `graphm`

## About this repository

My intent with this repo is to update a bit the tool `graphm` which was initially proposed here: <https://projects.cbio.mines-paristech.fr/graphm/>.
It has not been for a decade and the code does not compile on my laptop, so I took the initiative to distribute the few fixes I made to have a working project.
At the beginning, I fixed a compilation error and then, a segmentation fault. The segmentation fault was solved by addressing a compilation warning, so I addressed all the compilation warnings.
For now, my intent is to make the code work without refactoring it. If some people are interested in refactoring and updating this code, you can contact me so we can organize something.

Feel free to contribute to this repo to fix additional bugs. Please also consider completing the requirements below.

## Implemented algorithms

* Umeyama algorithm. [S.Umeyama: An eigendecomposition approach to weighted graph matching problems](https://ieeexplore.ieee.org/abstract/document/6778)
* Linear programming approach. [H.A. Almohamad and S.O. Duffuaa: Linear Programming Approach for the Weighted Graph Matching Problem](http://doi.ieeecomputersociety.org/10.1109/34.211474https://ieeexplore.ieee.org/abstract/document/211474)
* Rank algorithm. [R.Singh and J.Xu and B.Berger: Pairwise Global Alignment of Protein Interaction Networks By Matching Neighborhood Topology](https://link.springer.com/chapter/10.1007/978-3-540-71681-5_2)
* QCV (Quadratic convex relaxation) algorithm. [M.Zaslavskiy and F.Bach and J-P.Vert A path following algorithm for the graph matching problem](https://ieeexplore.ieee.org/abstract/document/4641936)
* PATH (A path following) algorithm. [M.Zaslavskiy and F.Bach and J-P.Vert A path following algorithm for the graph matching problem](https://ieeexplore.ieee.org/abstract/document/4641936)

## Install

Requirements:

* g++
* make
* GSL package

```bash
sudo apt install make build-essential libgsl-dev g++
```

Install script:

```bash
./graphm_install
```

Once install is done, you should have the binary `./bin/graphm`.
