.. Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
   Hatchet Project Developers. See the top-level LICENSE file for details.

   SPDX-License-Identifier: MIT

.. hatchet documentation master file, created by
   sphinx-quickstart on Tue Jun 26 08:43:21 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

####
SPOT
####

SPOT is a web-based data analysis and visualization interface with novel
visualizations to explore large collections of performance profiles. Some
common use cases include:

* Performance comparison of nightly tests
* Look for performance regressions
* Performance tracking of developer changes
* Run an MPI scaling study
* Collect performance profiles from users
* Understand how users run and hit performance issues.

.. figure:: images/spot-landing-page.png

   SPOT landing page.

.. figure:: images/spot-landing-page2.png

   SPOT landing page's.

SPOT is available internally at LLNL or you can use the container recipe
available in a `GitHub repository <https://github.com/llnl/spot2_container>`_.

For Lawrence Livermore National Laboratory users, we recommend using the
internal SPOT deployment available at `<https://lc.llnl.gov/spot2/>`_.

.. toctree::
   :maxdepth: 1
   :caption: User Docs

   getting_started
   basic_tutorial
   llnl

If you encounter bugs while using the SPOT container, you can report them by
opening an issue on `GitHub <http://github.com/llnl/spot2_container/issues>`_.

If you are referencing hatchet in a publication, please cite the
following paper:

* David Boehme, Pascal Aschwanden, Olga Pearce, Kenneth Weiss, and Matthew
  LeGendre. 2021. Ubiquitous Performance Analysis. In High Performance
  Computing: 36th International Conference, ISC High Performance 2021, Virtual
  Event, June 24 – July 2, 2021, Proceedings. Springer-Verlag, Berlin,
  Heidelberg, 431–449. `<https://doi.org/10.1007/978-3-030-78713-4_23>`_

##################
Indices and tables
##################

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
