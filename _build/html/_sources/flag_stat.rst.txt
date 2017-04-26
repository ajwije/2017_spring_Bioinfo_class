.. module:: Counting mapped reads 

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

****************************************************************
Counting mapped reads
****************************************************************


To get the number of reads mapped to a reference sequences (in this case, predicted tomato cDNA sequences), we can use Samtools. Bowtie2 
output is in sam format and first, we need to convert the output files into sorted bam files.


1. Type Samtools in app finding window. 


.. figure:: img/samtools_1.png


2. Select "SAM to sorted BAM" 

.. figure:: img/samtools_2.png


3. Select Bowtie2 output files (SAM format). 

.. figure:: img/samtools_3.png

4. Above will create sorted bam file. You will need to use this as the input for the Samtools Flagstat, which
will count the number of mapped reads. 

.. figure:: img/samtools_4.png


|

.. figure:: img/samtools_5.png


I have used the following bash command to count mapped reads in case you are interested in it doing programmatically. 

.. code-block:: bash


	# navigate to where your sam files are and execute the following commands. 

	for i in *.sam

	do 
	#extract the file name without extension and print it to the screen 


	echo ${i%.sam}

	#covert sam to sorted bam 
	samtools view -bS $i | samtools sort - -o ${i%.sam}_sorted.bam

	#getting flagstat and write it an output file for each bam file. 
	samtools flagstat ${fname%.sam}_sorted.bam >> flagstat.txt

	done

