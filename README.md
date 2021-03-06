# ncplot
RAF netCDF file timeseries plotting tool.

ncplot is an interactive plotting tool for workstations running X11/R5, Motif 1.2. ncplot allows the user to view time-series data stored in netCDF files that conform to the NCAR-RAF/nimbus conventions. Both Low-rate and Mixed-rate files are supported, as well as files where the data have been reduced below 1 sps (sample per second), e.g., files run through ncav.

A few of its features are:

    Plots up to 8 datasets per graph.
    Can draw from up to 4 netCDF files on the same plot.
    1 to 4 time-series strip charts.
    1 to 4 XY plots.
    XYZ plot.
    ASCII window.
    Spectra, Co-spectra, Quadrature, Coherence, and Phase.
    Allows user-defined titles, labels, scaling, and major & minor tic marks.
    Annotations.
    Publication quality [Encapsulated] [color] PostScript printouts.
    Optional realtime/on-board mode. 

ncplot is NOT for contouring, image or vector data.

ncplot was written at the Research Aviation Facility of The National Center for Atmospheric Research to view and analyze our aircraft data (and NOAA's GIV). The NCAR-RAF/nimbus conventions were designed to store multi-rate data, i.e., variable A may be stored at 5sps and variable B at 25sps. ncplot will plot variables of differing rates (and from different files) next to each other. Every effort has been made to make it "what you see is what you get" between the screen and printouts.

## Documentation

https://www.eol.ucar.edu/raf/Software/ncplot.html  
https://www.eol.ucar.edu/raf/Software/netCDF.html describes netCDF conventions used.  
https://github.com/ncar/aircraft_oap/wiki/MacOS-Build-Environment for building on MacOS.

## Build

ncplot can be built on any Unix platform, including MacOS.  Motif GUI toolkit is the limiting factor.

```
git clone https://github.com/ncar/ncplot
cd ncplot
```
    
If you are on MacOS, follow MacOS Environment instructions above and edit the Makefile and uncomment the MacOS section.

```
make
```

    
