.. module:: In_class activities Week 7
   :synopsis: Phylogenetics   
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right

***********************************
Steps of building a tree (Part II)
************************************

Make multiple sequence alignment for Globin gene family
----------------------------------------------------------
:Step 1: Download globin.fasta from Blackboard and perform a MSA using MUSCLE (follow the steps we discussed last week).

:Step 2: Examine the alignment to make sure it is correct and no additional editing is needed. 

:Step 3: Export the alignment as a fasta format file on your Desktop. Name it as globin_align
|
|
|
Find the best substitution model 
----------------------------------------
:Step 1: Calculate the distance using different substitution models
	:a: Select **Distance** and then **Compute Pairwise distance**
	:b: Calculate distance using the following methods
		:i: No. of Differences 
		:ii: p-distances 
		:iii: Poisson model 
|
|

.. figure:: img/mega_13.png
|
|

:Step 2: Use the same alignment file and build three NJ trees using different substitution models:

	:a: No. of Differences 
	
	:b: p-distances 
	
	:c: Poisson model 
|
|


.. figure:: img/mega_12.png

|
|
:Step 3: `Best model based on ProtTest <http://darwin.uvigo.es/cgi-bin/queueSystem.pl?cgi_pid=9928>`_

Building Phylogenetic trees
----------------------------------------

:Step 1: Click on **Phylogeny**
|
.. figure:: img/mega_10.png

|
:Step 2: Make Neighbor-Joining tree with **Bootstrap 500 replicates**

	:A: What relationships can you see in the tree?

	:B: What can you say about the statistical support for each relationship?

	:C: What should be the out-group? 

|
|


.. figure:: img/mega_11.png

|
|

	

:Step 3: Save the tree as a pdf file by clicking on **Image** button

|
|

:Step 4: Build a tree using Parsimony method with **50 Bootstrap** replicates (500 will be very slow).

	:A: What relationships can you see in the tree?

	:B: What can you say about the statistical support for each relationship?

	:C: Do you see the same relationships that you saw with NJ tree?
|
|

:Step 5: Bayesian inference of phylogeny

`Follow this link to MrBayes online server <http://www.phylogeny.fr/one_task.cgi?task_type=mrbayes>`_

	:A: Use the same alignment file 
	:B: In MrBayes select Poisson amino acid model with equal rates of substitution.
    :C: Select prior parameters (e.g. equal, fixed frequencies for the states; equal probability for all topologies; unconstrained branch lengths).
    :D: Run 1,000,000 trials for Monte Carlo Markov Chain estimation of the posterior distribution.
    :E: Obtain phylogram
    :F: Export tree files 
    :G: View in MEGA software
    
|
|
.. figure:: img/mega_15.png    

    
    

    
|
|
.. figure:: img/mega_14.png


















