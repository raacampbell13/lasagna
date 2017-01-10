# Lasagna - Python Volume Visualiser for 3-D data. #


![cover image](http://raacampbell.github.io/lasagna/images/mainWindow.jpg "Main Window")

## Concept ##
Lasagna is a lightweight platform for visualising for 3D volume data. Lasagna features
a flexible plugin system, allowing it to be easily extended using Python and PyQt. 
Visualisation is peformed via three linked 2D views. Lasagna was written to explore 
registration accuracy of 3D data, guide registration, and overlay point data onto images. 
It was also written to help explore the Allen Reference Atlas. Lasagna is under heavy 
development but is maturing rapidly. For more information see 
the [website](http://raacampbell.github.io/lasagna).


## Installation ##
Lasagna runs on Python 3, PyQt5, and uses PyQtGraph for the plotting and requires the following modules:


* PyLibTiff
* pynrrd
* numpy
* pyqtgraph >0.10.0
* yaml [and pyyaml]
* Scipy [optional - ARA explorer]
* Scikit-Image [optional - ARA explorer]
* PyQt5
* SIP
* tifffile [optional for importing LSM files]
* vtk [optional, for faster import of MHD files but doesn't work in Python 3]


On Linux you should be able to install everything but `tifffile` and `vtk` by running:

```
pip3 install -r requirements.txt --user --upgrade
```

This command installs the dependencies in your home folder and if any are already installed in the system path it looks for newer versions and installs those. 
It does not install `vtk`, which currently seems not to be supported by Python 3. 
For other platforms, please see [here](http://raacampbell.github.io/lasagna/installation.html)



After the first run, Lasagna creates a preferenes file in the ```.lasagna``` hidden directory in your home directory. 
You may need to edit this file to make Lasagna aware of its built in-plugins. i.e. edit the pluginPaths preference. 
This step isn't user-friendly, sorry.

## Usage

See the [website](http://raacampbell.github.io/lasagna).

## Current status ##
Even the master branch is currently unstable (although should always be usable). 
