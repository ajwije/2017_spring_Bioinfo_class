.. module:: Adapter and quality trimming using trim-galore

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

****************************************************************
Adapter and quality trimming using trim-galore
****************************************************************

We are going to use Trim-galore to trim adapters, and poor quality bases. This tool has several advantages. It allows selection
multiple files. You can also select both forward and reverse reads. If you want to read more about Trim-galore, 
please visit their `website <http://www.bioinformatics.babraham.ac.uk/projects/trim_galore/>`_.
Also, Trim-galore is a wrapper for `Cutadapt <http://cutadapt.readthedocs.io/en/stable/guide.html#three-prime-adapters>`_ , 
which is the actual tool that performs the trimming.



*Please follow the tutorial carefully.*

Step 1: **Launching Trim-galore**
-----------------------------------------

1. In the finder window type "trim-galore"

|

3. Select "Trim Galore".
 
	.. figure:: img/trim_galore_1.jpg



|

Step 2: **Selecting input files**
----------------------------------------------------------------

As indicated in the figure:
1. Is this library paired- or single-end? "Paired-end" 

|

2. Adapter sequence to be trimmed: "Select Illumina universal" 

	.. figure:: img/trim_galore_2.jpg
	

|

Step 3: **Advance settings**
----------------------------------------------------------------
1. From "Trim Galore! advanced settings" select "Full parameter list"

	.. figure:: img/trim_galore_3.jpg
	
2. Set "Overlap with adapter sequence required to trim a sequence" to 6.

	.. figure:: img/trim_galore_4.jpg

3. Run the analysis. 


	
	