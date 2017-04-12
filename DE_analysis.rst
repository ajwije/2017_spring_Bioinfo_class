.. module:: Differential gene expression analysis 

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

****************************************************************
Differential gene expression analysis
****************************************************************

Link for  Bowtie mapped counts http://de.cyverse.org/dl/d/E9B4C299-D6CB-4656-A4F6-FF67240AEA49/170407_bowtie_counts.txt


Target file for bowtie mapped reads: http://de.cyverse.org/dl/d/BECB62C3-A369-4084-9BC9-2BFD9E6E9600/bowtie_target.txt




DESeq tutorial:
-------------------

`Tutorial link <https://pods.iplantcollaborative.org/wiki/display/DEapps/DESeq>`_


Steps to perform DEseq analysis
------------------------------------
1. From Apps select "DEseq (Multifactorial Comparison)

	.. figure:: img/DEseq_1.png

|
2. Name your analysis and select a folder where your results need to be saved. 

	.. figure:: img/DEseq_2.png
	
|

3. Select the correct target file and the count file. 

	.. figure:: img/DEseq_3.png
	
|
4. Give a name to the project. Reference biological condition should be "control" samples. Variable of 
interest is "group" (Column header of the third column of the target file). 

	.. figure:: img/DEseq_4.png

|
5. Set the significant threshold to 0.05 and launch the analysis. 

	.. figure:: img/DEseq_5.png
