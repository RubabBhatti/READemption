Visualization of RNA-seq data
==============================

This guide explains how to visualize RNA-seq data files in integrated genome browser (IGB). 

Installing IGB
--------------

1. Install IGB for your system from IGB official website: https://www.bioviz.org/ .
2. Follow the installation requirements for Linux, Windows and macOS.
3. Launch IGB.

For linux, run the following command in terminal after installation to open IGB:
::

    $ chmod +x IGB-linux-amd64-<version>.sh
    $ ./IGB-linux-amd64-<version>.sh


Preparing data for visualization
--------------------------------

After running the READemption analysis, you"ll get wiggles files in coverage folder. 
These wiggle files will be used for visualization. 

1. Go to the coverage folder first.
2. Navigate ".wig" or ".wig.gz" files of your sample.
3. Unzip the .wig.gz files (optional) by running the following command:
         $ Gunzip *.wig.gz

Load the data in IGB
--------------------

1. Open IGB.
2. Load reference genome file (".fa", ".fna", ".fasta") and annotation file (".gff3") by clicking on
 "File" → "Open file" on the top left corner, and then click on "Load sequence" on top right corner next to zoom option .
3. Load the coverage ".wig" files. 
4. Zoom in and zoom out into the regions of your interest.

NOTE : After running READemption_analysis you will get two folders of coverage named as
 "READemption_analysis/output/salmonella_coverage-tnoar_mil_normalized/" and "READemption_analysis/output/salmonella_coverage-tnoar_min_normalized/", 
  you can use either file but for IGB visualization  "READemption_analysis/output/salmonella_coverage-tnoar_mil_normalized/"
  is recommended for clear display of normalised expressions. 


Additional Tips
---------------

1. You can change the color of the strands of reference genome, gff3 or wiggles file data by 
locating the track in IGB main window where there is a table like view named as "Data management view"
, Click on the color appearing in the boc below "FG".

2. IGB only support file formats like ".fasta", ".gff3", ".bigwig", ".bam", ".bed", ".wig", ".vcf". Make 
sure you load the right file format.

3. Verify your files are compatible with IGB's version.

