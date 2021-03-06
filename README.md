kgrid
=====

Generates a suitably converged **k**-point grid for solid-state
quantum chemical calculations.

Current status
--------------

* Reads FHI-aims geometry.in file from working directory or specified file
* A **k**-point density is selected to satisfy a given length cutoff, as
  described by Moreno & Soler (1992)[1]
* This **k**-point grid is expressed as a number of samples in each
  lattice vector and passed to standard output
* Defaults to working directory and 10Å (generally well-converged for
  semiconducting or insulating materials)
* Optional arguments are implemented with conventional GNU/POSIX
  syntax, including -h help option

Short-term goals
----------------

* Robust type-checking and error-handling
* Support for VASP (delegated to Lee Burton)

Long-term goals
---------------

* Generate suitable input files directly
    * May involve integrating this script into a larger, more general program

Disclaimer
----------

This program is not affiliated with FHI-aims. This program is made available under the GNU General Public License; you are free to modify and use the code, but do so at your own risk.

References
----------

[1] Moreno, J., & Soler, J. (1992). Optimal meshes for integrals in real- and reciprocal-space unit cells. *Physical Review B*, 45(24), 13891–13898. [doi:10.1103/PhysRevB.45.13891](http://dx.doi.org/10.1103/PhysRevB.45.13891)
