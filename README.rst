======================
passive-fm-utils
======================

Functions used with data from MIT Haystack Intercepted Signals for Ionospheric Science 
P. I. Frank Lind

.. contents::

data available from
http://atlas.haystack.mit.edu/isis/fermi/events/

Programs
========
These programs don't actually do any processing, just for user convenience of plotting.

``PlotSCR`` plots Scatter to Clutter ratio of an HDF5 file.

``FMbesselSidebands`` theoretical sideband relative amplitude

Getting the Data
================
You will need ``wget``. This is built-in to every Linux system, on Cgywin under Windows, and via HomeBrew or MacPorts on Mac.

Example Download Commands
-------------------------
::
  
  mkdir -p ~/data
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-03/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-13/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-05/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-04/rx40rx51/

