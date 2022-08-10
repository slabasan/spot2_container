.. Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
   Hatchet Project Developers. See the top-level LICENSE file for details.

   SPDX-License-Identifier: MIT

*****************************
Using Hatchet on LLNL Systems
*****************************


Hatchet installations are available on both Intel and IBM systems at Lawrence
Livermore National Laboratory.

To use one of these global installations, please add the following to your
Python script or Jupyter notebook. This code allows you to use hatchet and its
dependencies.

.. code-block:: python

  import sys
  import platform

  machine = platform.uname().machine

  input_deploy_dir_str = "/usr/gapps/spot/live"
  sys.path.append(input_deploy_dir_str + "/hatchet-venv/" + machine + "/lib/python3.7/site-packages"),
  sys.path.append(input_deploy_dir_str + "/hatchet/" + machine)

  import hatchet
