.. Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
   Hatchet Project Developers. See the top-level LICENSE file for details.

   SPDX-License-Identifier: MIT

***************
Getting Started
***************

SPOT's Workflow
===============

First, point the SPOT webpage at a directory containing ``*.cali`` files.

.. image:: images/directory_input.png

Second, select “interesting” sets of runs to analyze, that is slice and dice
the data to make interesting comparisons.  Third, run common analyses with
SPOT, such as graphing a history of performance changes or viewing performance
context trees. Fourth, run more advanced, deep-dive analysis with `Hatchet
<https://github.com/llnl/hatchet>`_.

Data Collected
==============

Each application run has two types of data:

Metadata
--------
* Name/value data about job, such as user, host, FOM, input parameters, etc
* Displayed as histograms

.. image:: images/metadata-histogram.png

Metadata can be filtered by selecting regions of the histograms. Filtering in
one histogram updates the range of all other histograms. As an example,
filtering ``Launchdate`` to ``Feb 19-Feb 26`` will update the ``Users``
histogram to only show users who ran between those dates. While filtered,
comparisons and Jupyter notebooks will operate on the filtered data.

.. image:: images/metadata-histogram-filtered.png

Metadata is also configurable by either showing/hiding metadata or creating
composite metadata.

.. image:: images/metadata-selected.png

.. image:: images/metadata-composite.png

Performance Data
----------------
* Can be different metrics, including Avg Time/Rank, Max Time/Rank, bandwidth,
  etc
* Displayed as a flame graph or timeseries

.. image:: images/perfdata-flamegraph.png

.. image:: images/perfdata-timeseries.png

Performance data can be visualized per-run or compared across runs. A single
run is contained in each row of the Table View:

.. image:: images/single-run.png

By clicking the clock icon on the right, a flame graph is generated showing
performance against code:

.. image:: images/single-run-flamegraph.png

And by clicking the graph icon on the right, a timeseries is generated showing
performance against time:

.. image:: images/single-run-timeseries.png

When visualizing performance data across runs, the display is as follows:

#. Metadata value on x-axis
#. Aggregation (min/max/avg…) if multiple runs at same point.
#. Metric to graph on y-axis.
#. Grouping metadata.  Each unique value is a graph.
#. Stacked performance graph.  Click to drill-down.
#. Flame graph for runs currently under cursor.
#. Metadata for runs currently under cursor.


.. image:: images/perfdata-across-runs.png
