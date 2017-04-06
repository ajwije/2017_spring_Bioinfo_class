.. module:: Mapping short reads

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

****************************************************************
Mapping short reads 
****************************************************************
If you are using genome as the reference for RNAseq reads, you will need to use a splice-aware aligner like Tophat2.
If you are using cDNA as the reference, you can use a general purpose aligner like Bowtie2. 

*You need to do only one of the procedures based on what your group have been assigned to.* 


Step 1: **Mapping with Tophat2**
------------------------------------------
1. Click on *App*.

|
2. In the finder window type "Tophat"

|

3. Select "Tophat2-PE".
 
	.. figure:: img/tophat_1.png



|

4. As indicated in the figure, Name your analysis as you want.

|

5. Select the output folder where your analysis is going to be.

|

6. Click on "Input data" 

	.. figure:: img/tophat_2.png
	
|

7. Click on the Green "+" sign. 
	

|
8. Navigate to the folder where your samples are located. Select only the **first read files**.
Click "OK".  **You can select all three of your first read files.**

	.. figure:: img/tophat_3.png
	
|
9. Scroll down and click on the "+" below "Fastq file(s) (Read 2 of paired end reads):"

|

10. Select "Reference Genome" and select the tomato genome sequence as input. 

	.. figure:: img/tophat_4.png
	
|
11. Make sure quality is Sanger and leave rest of the default values as they are. Launch the analysis. 

	.. figure:: img/tophat_5.png
	
|
|


Step 2: **Mapping with Bowtie2**
------------------------------------------

1. Click on *App*.

|
2. In the finder window type "Bowtie".

|

3. Select Bowtie app indicated in the figure. 
 
	.. figure:: img/bowtie_1.png
|

4. As indicated in the figure, Name your analysis as you want.

|

5. Select the output folder where your analysis is going to be.


	.. figure:: img/bowtie_2.png

|

6. Click on "Input" 


|
8. Navigate to the folder where your samples are located. Select first and second read files.
You can only input one sample at a time. 

|

9. You need to name your output file carefully. For e.g., if it is heat1 sample, name the output as heat1.sam. 

	.. figure:: img/bowtie_4.png
	
|


10. Select "Reference Index" and select the tomato cDNA sequence as input. 

	.. figure:: img/bowtie_3.png
	
|
11. Select options. Set "Minimum fragment length" as 100 and "Maximum fragment length" as 600. Launch the analysis. 

	.. figure:: img/bowtie_5.png
	