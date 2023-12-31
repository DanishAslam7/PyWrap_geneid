# PyWrap_geneid
A python wrapper for the gene prediction program geneid.
# Requirements
To use PyWrap_geneid, an installed or built geneid with any version, preferably, geneid_v1.4.4.Jan_13_2011 is required. Using Ubuntu, geneid can be installed as follows.

Visit https://genome.crg.es/software/geneid/ and download a tar.gz file of desired version.

Unzip the file.
Type:
~~~
tar -zxvf geneid(version).tar.gz
~~~

More information can be found on the geneid GitHub page (https://github.com/guigolab/geneid).

# File Listing
The geneid distribution contains the following files and directories:

*bin/ compiled binaries
*CVS/ Entries, Repository, Root
*docs/ documentation: a short handbook.
*include/ geneid.h: The geneid header file.
*objects/ object files after compiling the source code.
*param/ Parameter files for several species.
*samples/ Test sequences.
*src/ source code of geneid program.
*GNULicense This software is registered under GNU license.
*Makefile This file is required to build geneid binary file.
*README This file.

# Compiling geneid
Move into the geneid directory.

Type:
~~~
make
~~~

This will generate the geneid executable file within the bin/ subdirectory.

Type:
~~~
geneid -h
~~~
to test the binary file has been correctly created.

To run PyWrap_geneid properly it is necessary that the geneid compilation is successful.

# Permissions
Ensure Execution Permission

Type:
~~~
chmod +x /path/to/geneid
~~~
For PyWrap_geneid Python version 3.6 or higher is required.

# Installation
PyWrap_geneid can be installed from PyPi as follows.
~~~
pip install pywrapgeneid
~~~

# Usage
PyWrap_geneid supports prediction of acceptor sites, exons, genes etc. The general sequence file format is fasta format but gff format can also be used for the same.

## Prediction
To run a prediction geneid can be executed on the input file as usual or the input file can be split

~~~
import pywrapgeneid
~~~

Download example.py to run the job using the module.
