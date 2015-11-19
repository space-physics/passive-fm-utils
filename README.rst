======================
passive-fm-utils
======================

Functions used with data from `MIT Haystack Intercepted Signals for Ionospheric Science <http://www.haystack.mit.edu/atm/science/space/isis/index.html>`_

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
You will need ``wget``. This is built-in to every Linux system, on Cygwin under Windows, and via HomeBrew or MacPorts on Mac.

Example Download Commands
-------------------------
::
  
  mkdir -p ~/data
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-03/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-13/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-05/rx40rx51/
  
  wget --quota=10000m -r -np -nc -nH --cut-dirs=3 --random-wait --wait 0.5 --reject index.html* -e robots=off -P ~/data/ http://atlas.haystack.mit.edu/isis/fermi/events/2010-08-04/rx40rx51/


References
==========

.. [1] Lind F., et al, “Intercepted Signals for Ionospheric Science”, Radio Science, vol. 48, pp. 248-264, June 2013. doi:10.1002/rds.20034, 2013
.. [2] Sahr J. and Lind F., “The Manastash Ridge Radar: A passive bistatic radar for upper atmospheric radio science”, Radio Science, vol. 32, no. 6, pp. 2345-2358, Nov. 1997. doi: 10.1029/97RS02454
.. [3] Sahr J. “Ionospheric Measurements”, Chap. 7 in, Advances in Bistatic Radar, SciTech Pub., 2007.
.. [4] Meyer M., “Passive VHF Radar Interferometer Implementation, Observations, and Analysis”, M.S. thesis, Elect. Eng. Dept., Univ. of Washington, Seattle, WA, 2003. URL: www.if.ufrj.br/~marroqui/DRACON/tese/mgm-thesis.pdf
.. [5] Lathi B. and Ding Z., Modern Digital and Analog Communication Systems. 4th Ed. Oxford Univ. Press, 2009.
.. [6] Lyons R., Understanding Digital Signal Processing. 3rd Ed., Prentice Hall, 2010.
.. [7] Carson, J., "Notes on the Theory of Modulation," Proc. IRE , vol.10, no.1, pp.57,64, Feb. 1922. doi: 10.1109/JRPROC.1922.219793
.. [8] Tsao, T., et al, "Ambiguity function for a bistatic radar," Aerospace and Electronic Systems, IEEE Trans., vol.33, no.3, pp.1041-1051, July 1997. doi: 10.1109/7.599331
.. [9] Howland, P., "Target tracking using television-based bistatic radar," Radar, Sonar and Navigation, IEEE Proc. , vol.146, no.3, pp.166-174, Jun 1999. doi: 10.1049/ip-rsn:19990322
.. [10] Thidé, B., “Simulated Scattering of Large Amplitude Waves in the Ionosphere: Experimental Results”, Physica Scripta, vol.T30, pp. 170-180, 1990. doi:10.1088/0031-8949/1990/T30/023
.. [11] Strømme, A., “Ionospheric and Magnetospheric studies with incoherent scatter radars”, EISCAT/SRI Int., EISCAT School, Qingdao China, 31 Oct 2006. URL: https://www.eiscat.se/groups/Documentation/CourseMaterials/2006Qingdao/Ionospere_China_Anja.pdf Retrieved 2 Dec 2013.
