msm_we
------

* Authors: John Russo, Sagar Kania, Jeremy Copperman, Daniel Zuckerman
* Free software: MIT license

Background
----------
This is a package for doing history-augmented MSM (haMSM) analysis on weighted ensemble trajectories.

Weighted ensemble data produced from simulations with recycling boundary conditions are naturally in a directional
ensemble. This means that a history label can be assigned to every trajectory, and an haMSM can be constructed.

Features
--------

* Compute a history-augmented Markov state model from WESTPA weighted ensemble data
* Estimate steady-state distributions
* Estimate flux profiles
* Estimate committors
* WESTPA plugins to automate haMSM construction
* WESTPA plugin to automate bin+allocation optimization


Known Issues
------------

- Sometimes, on Python3.7 (and maybe below) the subprocess calls will fail. This may manifest as a silent failure,
  followed by hanging (which is very fun to debug!) To fix this, upgrade to Python 3.8+.

- If running with `$OMP_NUM_THREADS > 1`, Ray parallelism may occasionally silently hang during clustering / fluxmatrix calculations


Credits
-------

This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.

.. Cookiecutter: https://github.com/audreyr/cookiecutter
.. `audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
