.. YA LATIF

OCEANLYZ
========

OCEANLYZ, Ocean Wave Analyzing Toolbox, is a toolbox for analyzing the wave time series data collected by sensors in open body of water such as ocean, sea, and lake or in a laboratory.

This toolbox contains functions that each one is suitable for a particular purpose. Both spectral and zero-crossing methods are offered for wave analysis. This toolbox can calculate wave properties such as zero-moment wave height, significant wave height, mean wave height, peak wave period and mean period. This toolbox can correct and account for the pressure attention (pressure loss) in the water column for data collected by a pressure sensor. This toolbox can separate wind sea and swell energies and reports their properties.

:Name: OCEANLYZ
:Description: Ocean Wave Analyzing Toolbox
:Version: 2.0
:Requirements: MATLAB, or GNU Octave, or Python (3 or later)
:Developer: Arash Karimpour (http://www.arashkarimpour.com)
:Documentation: https://oceanlyz.readthedocs.io
:Tutorial Video: `YouTube Playlist <https://www.youtube.com/playlist?list=PLcrFHi9M_GZRTCshcgujlK7y5ZPim6afM>`_
:Source Code: https://github.com/akarimp/oceanlyz
:Report Issues: https://github.com/akarimp/Oceanlyz/issues


Installation (MATLAB Version)
-----------------------------

To use MATLAB version of OCEANLYZ toolbox:

* Install MATLAB or GNU Octave
* Download OCEANLYZ:

    * Version 2.0 (GitHub): https://github.com/akarimp/oceanlyz/releases/download/2.0/oceanlyz_2_0.zip
    * Version 1.5 (CNET): https://download.cnet.com/Oceanlyz/3000-2054_4-75833686.html
    * Version 1.5 (GitHub): https://github.com/akarimp/oceanlyz/releases/download/1.5/oceanlyz_1_5.zip
    * Version 1.4 (GitHub): https://github.com/akarimp/oceanlyz/releases/download/1.5/oceanlyz_1_4.zip

* Unzip OCEANLYZ in any location you choose such as “C:\\”


Installation (Python Version)
-----------------------------

To use Python version of OCEANLYZ toolbox:

* Install Python
* Install OCEANLYZ

**1) Install Python**

First, we need to install Python programming language.

* Method 1:
    Install pure Python from https://www.python.org and then use the **pip** command to install required packages
* Method 2 (Recommended):
    Install Anaconda Python distribution from https://www.anaconda.com and then use the **conda** command to install required packages

**2) Install OCEANLYZ**

After Python is installed, we need to install OCEANLYZ package.

To install OCEANLYZ via pip (https://pypi.org/project/oceanlyz):

.. code:: python

    pip install oceanlyz

To install OCEANLYZ via Anaconda cloud (https://anaconda.org/akarimp/oceanlyz):

.. code:: python

    conda install -c akarimp oceanlyz


Operating System
----------------

This code can be run on Windows, Mac, and Linux. However, make sure any given path is compatible with a running operating system. In particular, “\\” is used in Windows path, while “/” is used in Mac or Linux path. For example, if a path is “C:\\” on Windows machine, it would be “C:/” on Mac or Linux.


Required Programing Language
----------------------------

This toolbox can be run by using MATLAB (https://www.mathworks.com), GNU Octave (https://www.gnu.org/software/octave), or Python (https://www.python.org). 


Required Package for MATLAB
---------------------------

MATLAB users need to install MATLAB Signal Processing Toolbox for running the Oceanlyz spectral analysis. It gives Oceanlyz access to MATLAB Welch's power spectral density calculation. However, MATLAB Signal Processing Toolbox it is not required for zero-crossing analysis. 


Required Package for GNU Octave
-------------------------------

GNU Octave users need to install/load GNU Octave Signal Package for running the Oceanlyz spectral analysis. It gives Oceanlyz access to GNU Octave Welch's power spectral density calculation. However, GNU Octave Signal Package it is not required for zero-crossing analysis.

GNU Octave Signal Package can be loaded inside GNU Octave by using a following command in a command window (This should be done every time GNU Octave is opened):


.. code:: octave
    
    >> pkg load signal


If GNU Octave Signal Package is not already installed, it should be first installed from Octave Forge (octave.sourceforge.io), and then get loaded by using the following commands in a command window:

.. code:: octave

    >> pkg install -forge signal
    >> pkg load signal


Required Package for Python
---------------------------

Following packages are required:

* NumPy (https://numpy.org)
* SciPy (https://www.scipy.org)
* Matplotlib (https://matplotlib.org)


Quick Start (MATLAB Version)
----------------------------

* Open MATLAB or GNU Octave
* Change a current folder (current directory) to a folder that contains OCEANLYZ toolbox, for example “C:\\oceanlyz”, in MATLAB or GNU Octave.
* Open a file named “oceanlyzinput.m” in MATLAB or GNU Octave editor and modify it based on the properties of the collected dataset and required analysis.
* Run a file named “RunOceanlyz.m” in MATLAB or GNU Octave to start calculations.


Quick Start (Python Version)
----------------------------

* Open Python
* Import OCEANLYZ package by using "import oceanlyz" 
* Create OCEANLYZ object such as “ocn=oceanlyz.oceanlyz()” in Python and set/modify its properties based on the dataset and required analysis.
* Run a method as “ocn.runoceanlyz()” in Python to start calculations.


Recommended Book
----------------

* | **Ocean Wave Data Analysis**
  | Introduction to Time Series Analysis, Signal Processing, and Wave Prediction.
  | Order at Amazon: https://www.amazon.com/dp/0692109978
  |
* | **Principles of Data Science with Python**
  | Introduction to Scientific Computing, Data Analysis, and Data Visualization.
  | Order at Amazon: https://www.amazon.com/dp/1735241008
  |
* | **Fundamentals of Data Science with MATLAB**
  | Introduction to Scientific Computing, Data Analysis, and Data Visualization.
  | Order at Amazon: https://www.amazon.com/dp/1735241016

Citation
--------

Cite this toolbox as:

Karimpour, A., & Chen, Q. (2017). Wind Wave Analysis in Depth Limited Water Using OCEANLYZ, a MATLAB toolbox. Computers & Geosciences.

Link: https://www.sciencedirect.com/science/article/pii/S0098300417306489

License Agreement and Disclaimer
--------------------------------

OCEANLYZ: Ocean Wave Analyzing Toolbox

Copyright (c) 2022 Arash Karimpour

All rights reserved

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
