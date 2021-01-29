# Introduction

This repo is part of the Master's [course] about performance evaluation at [Ensimag]. 

It is a practical training to simulate different variations of the [ALOHA] system and perform statistical analysis on their performance.

# Session 1

## Requirements

  - [Python3] 
  - [SimPy] discrete-event simulation library
  - [Matplotlib] or any other 2D plotting library

## Installation

Install python 3.6:

```sh
$ sudo apt-get update
$ sudo apt-get install python3.6
```

Check if installation succeeded, the following command should display your python version:
```sh
$ python3.6 --version
```
Install python packet management system PIP:

```sh
$ sudo apt-get install python3-pip
```

Install the libraries:

```sh
$ sudo pip3 install -U simpy matplotlib numpy
```

## Homework

- Write a SimPy program that simulates a Poisson packet arrival process with intensity \lambda = 15 packets per second
- What is the observed average packet rate ? 
- What is the 95% confidence interval ?

   
# Session 2

- The "two routers" problem with and without collision are presented in the slides named "exercice2.pdf"
- The homework is due by the 23/11/18 before midnight.

## Homework

* Complete the implementation of the queue simulation module
* Using the module, implement the two routers problem **without collision**. Then, for \lambda_1=\lambda_2= 7.5 packets per second, simulate and compute the following (in the stationary regime):
    * The average packet rate at the output of both routers. What can you conclude about the sum of two independent Poisson processes ?
    * The average latency. What is the **99%** confidence interval ?
* Using the API, implement the two routers problem **with collision**. Then, for \lambda_1=\lambda_2= 7.5 packets per second, simulate and compute the following (in the stationary regime):
    * The average latency. What is the 99% confidence interval ?
    * The average packet drop ratio for each router What is the 99% confidence interval ? 

## FAQ

- Generators are important in SimPy, I suggest you check this [page] for a quick tutorial. 

   [Ensimag]: <https://ensimag.grenoble-inp.fr/>
   [course]: <https://ensimag.grenoble-inp.fr/fr/formation/performance-evaluation>
   [Python3]: <https://www.python.org/>
   [SimPy]: <https://simpy.readthedocs.io/en/latest/contents.html>
   [Matplotlib]: <https://matplotlib.org/>
   [ALOHA]: <https://en.wikipedia.org/wiki/ALOHAnet>
   [page]:https://www.programiz.com/python-programming/generator
   
   
