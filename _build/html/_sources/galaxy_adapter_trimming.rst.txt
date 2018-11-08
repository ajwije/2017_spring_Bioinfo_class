.. module:: Adapter and quality trimming using trim-galore

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

****************************************************************
Adapter and quality trimming using Cutadapt
****************************************************************

We are going to use Trim-galore to trim adapters, and poor quality bases. This tool has several advantages. It allows selection
multiple files. You can also select both forward and reverse reads. If you want to read more about Trim-galore, 
please visit their `website <http://www.bioinformatics.babraham.ac.uk/projects/trim_galore/>`_.
Also, Trim-galore is a wrapper for `Cutadapt <http://cutadapt.readthedocs.io/en/stable/guide.html#three-prime-adapters>`_ , 
which is the actual tool that performs the trimming.



*Please follow the tutorial carefully.*

Step 1: **Launching Cutadapt and performing the analysis**
------------------------------------------
1. Type Trim-galore in the search box on top left hand corner. 

|
2. Select paired-end and select the two paired-end files are shown below. Use Illumina universal adapter to trim. 
 
	.. figure:: img/cutadapt_1.png
	
3. Click on the advance settings. Set the parameters as indicated in blue arrows. 

	.. figure:: img/cutadapt_2.png


|


	.. figure:: img/cutadapt_3.png

|

	.. figure:: img/cutadapt_4.png

|

	.. figure:: img/cuadapt_5.png
	
	
4. Launch the analysis. 


