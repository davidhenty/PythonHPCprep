<img src="./images/Archer2_logo.png" width="355" height="100"
align="left"> <img src="./images/epcc_logo.jpg" align="right"
width="133" height="100">

<br /><br /><br /><br /><br />

# Make your Python code 10,000 times faster with parallel numpy!

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

<h3>Introduction</h3>

This page details the setup steps you need to take in advance of the
RSECon22 workshop [Make your Python code 10,000 times faster with
parallel
numpy!](https://virtual.oxfordabstracts.com/#/event/3101/submission/103)
on Wednesday 7th September 2022, 09:00 - 12:30 BST.

Participants must bring a laptop with a Mac, Linux, or Windows
operating system (not a tablet, Chromebook, etc.) that they have
administrative privileges on.

In advance of the course, you need to:

  * set up Python, Anaconda, Jupyter notebooks and mpi4py on your laptop;
  * apply for a login account on ARCHER2, the UK National HPC service.

Full instructions are proved below.

<h3>Python setup on your laptop</h3>

<h4>Pre-requisites</h3>

To install Python3, Anaconda and Jupyter Notebooks follow the
[instructions on the Software Carpentries
website](https://swcarpentry.github.io/python-novice-inflammation/setup.html).

We will not be using the same material as the Software Carpentries
course, but to test your installation you can follow the instructions
to "Obtain lesson materials", open `swc-python/Untitled.ipynb` in a
Jupyter notebook and execute the following commands (to execute a command in a notebook you need to type Shift + Enter, not just Enter):
````
import numpy as np
a = np.array( [-1, 0, 1] )
print(a)
````
You should see the output:
````
[-1  0  1]
````


The course assumes a basic understanding of Python programming. You
will also need to be able to run a Jupyter notebook on your own laptop
-- follow the installation instructions at
[https://jupyter.org/install](https://jupyter.org/install).

You will also need an account on the [UK national supercomputer
ARCHER2](https://www.archer2.ac.uk/); full details of how to apply
will be supplied in advance.


---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]


