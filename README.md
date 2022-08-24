<img src="./images/Archer2_logo.png" width="355" height="100"
align="left"> <img src="./images/epcc_logo.jpg" align="right"
width="133" height="100">

<br /><br /><br /><br /><br />

# Make your Python code 10,000 times faster with parallel numpy!

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

<h2>Introduction</h2>

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

Full instructions are provided below - if there are any issues please
contact [d.henty@epcc.ed.ac.uk](mailto:d.henty@epcc.ed.ac.uk).

<h2>Python setup on your laptop</h2>

<h3>Python environment</h3>

To install Python3, Anaconda and Jupyter Notebooks follow the
[instructions on the Software Carpentries
website](https://swcarpentry.github.io/python-novice-inflammation/setup.html).

If you are a Windows user, note that during installation you should
make sure you check the box **Add Anaconda to my PATH environment
variable**.

Note that this installation can take a long time; for me it stalled
for quite a while at "Setting up the base environment" but did
complete eventually!

</h4>Testing</h4>

To test your numpy installation, download and unzip
[PythonHPCexamples.zip](https://github.com/davidhenty/PythonHPCprep/raw/master/PythonHPCexamples.zip)
and open `examples.ipynb` in a Jupyter notebook. The notebook also
includes a simple test which you can run after installing your MPI
installation below.

<h3>MPI environment</h3>

Once you have the Anaconda distribution, it is a relatively
straightforward matter to install mpi4py and an actual MPI
implementation (here we use MPICH) which is required to do the
work underneath.

From a local terminal type:
````
user@laptop> conda install -c conda-forge mpi4py
````

Windows users should launch an Anaconda Prompt terminal using `CMD.exe
Prompt` from Anaconda Navigator.

Note for users who already have MPI installed (e.g., for C/Fortran):
to prevent name clashes in your PATH it can be useful to use a conda
environment to install mpi4py and the associated MPI implementation -
see
[http://conda.pydata.org/docs/using/envs.html](http://conda.pydata.org/docs/using/envs.html). You
can switch to a different environment using "Kernel -> Change kernel"
from the Jupyter notebook.

</h4>Testing</h4>

Run the `mpihello.py` example as instructed in the notebook you
previously donwloaded to test Python and numpy.

<h3>ARCHER2 Account</h3>

You will also need an account on the [UK national supercomputer
ARCHER2](https://www.archer2.ac.uk/). As someone who expressed an
interest in this workshop when you registered you will have received
an email detailing how to apply for an account.

Please note:

  * Due to security resrictions we cannot accept ARCHER2 registrations
    from non-institutional accounts (e.g. gmail accounts are not
    accepted). All ".ac.uk" addresses are accepted, and we will also
    consider applications from recognised academic institutions and
    commercial companies.

  * Don't worry if you can't get an ARCHER2 account - all the
    exercises can be done on your laptop and it is only the final
    performance measurements that actually require access to
    ARCHER2. You are welcome to pair up with someone else for this
    session at the workshop.
  
---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]


