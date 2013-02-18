geotiff-iosp
============

GeoTIFF IOSP for NetCDF-Java

GEOTIFF-IOSP is a plugin for the Unidata [THREDDS Data Server](http://www.unidata.ucar.edu/projects/THREDDS/tech/TDS.html)(TDS) that allows the TDS to access GeoTIFF file content directly, without translation first into another format like NetCDF.  This allows GeoTIFF file content to be accessed via OPeNDAP, WCS, WMS, NcISO and other TDS services. 

###Installation

  * Download the [geotiff-iosp jar file](https://docs.google.com/file/d/0BzAHlPEEP_ujRnZYQXhlZmdjYWM/edit?usp=sharing), or if you want to use build the latest from source, clone the respository using git: 

      `git clone https://github.com/tkunicki-usgs/geotiff-iosp.git`
    
  and use Maven, NetBeans or similar to build.

  * Place the jar file in the `<tomcat>/thredds/WEB-INF/lib` directory and reload THREDDS.
 
###Usage

  * You can now use GeoTIFF files just as you would NetCDF files -- you can aggregate them or add metadata using NcML, or just add   `<include wildcard="*.tif"/>` to your DatasetScan to pick them up.  
  
  * Here is an example: http://geoport-dev.whoi.edu/thredds/dodsC/usgs/data1/rsignell/catalog.html?dataset=usgs/data1/rsignell/sample.tif
