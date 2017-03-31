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
------------------------------------------
1. Click on *App*.

|
2. In the finder window type "trim-galore"

|

3. Select "trim-galore-0.4.1".
 
	.. figure:: img/trim_1.png



|

Step 2: **Selecting output folder**
----------------------------------------------------------------

As indicated in the figure:
1. Name your analysis as you want

|

2. Select the output folder where your analysis is going to be

|

3. Click on "Paired end Input fastq files" 

	.. figure:: img/trim_2.png
	

|

Step 3: **Selecting input files**
----------------------------------------------------------------
1. Click on the Green "+" sign. 
	
	.. figure:: img/trim_3.png
|
2. Navigate to the folder where your samples are located. Select only the **first read files**.
Click "OK".  

	.. figure:: img/trim_4.png
	
|

3. You should all your first read files selected like this.

	.. figure:: img/trim_5.png
|

4. Scroll down and click on the "+" below "Fastq file(s) (Read 2 of paired end reads):"

	.. figure:: img/trim_6.png
|
	
5. Select the read two files as above. You will see them in the box as in the figure below.

	.. figure:: img/trim_7.png
	
|

6. Scroll down and check box beside "Paired (Select this option for paired-end files)" to 
indicate these are paired end reads. 

**very important** 

	.. figure:: img/trim_8.png

|

7. Click on "Parameters" as indicated in the above figure. 

|

8. Set the parameters as indicated in the figure:

|

a. Use Fred 20 as quality trimming cut off (this is the default).

|

b. Copy and paste the following adapter sequence for in the box below "Adapter sequence to be trimmed:"

|

		AATGATACGGCGA

|

c. Copy and paste the following adapter sequence for in the box below "Adapter2"

|

		CAAGCAGAAGACGG

|

d. Set the stringency to 6. 

	.. figure:: img/trim_9.png

|

e. Scroll down and set the length as 40. Any sequence become shorter than this length during the trimming will be discarded.
|
f. Launch the analysis. 

	.. figure:: img/trim_10.png
	

	
	
	
