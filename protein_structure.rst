.. module:: Protein Structure Analysis 

   :synopsis:
       
.. moduleauthor:: Asela Wijeratne<awijeratne@astate.edu>

.. index::

.. highlight:: rest

.. figure:: img/UnivLogo_Stack_2C_Dark.png
   :align: right



Secondary Structure Prediction
------------------------------------

1. We will use one of the differentially expressed in tomato pollen transcriptome under head stress. 

I have retrive the amino acid sequences for Solyc06g050510 from `SolGen website <https://solgenomics.net/feature/17844299/details>`_.

| 

MKRHIHYNAHPIDPHPFEAFWYGSWQAVERLRINMGTITTHVLVDGEVIEENIPVTNLRMRSRKATLSDCAC
FLRPGLEVCVLSIPYQGENSGDEKDVKPVWIDGKIRSIERKPHELTCTCKFHVSVYVTQGPPPILKKTLSKE
IKMLPIDQIAVLQKLEPKPCENKRYRWSSSEDCNSLQTFKLFIGKFSSDLTWLMTASVLKEATFDVRSIHNQ
IVYEIVDDDLVRKETNSNQHSYSVNFKLEGGVQTTTVIQFNRDIPDINSTSDLSESGPLVLYDLMGPRRSKR
RFVQPERYYGCDDDMAEFDVEMTRLVGGRRKVEYEELPLALSIQADHAYRTGEIEEISSSYKRELFGGNIRS
HEKRSSESSSGWRNALKSDVNKLADKKSVTADRQHQLAIVPLHPPSGTGLTVHEQVPLDVDVPEHLSAEIGE
IVSRYIHFNSSSTSHDRKASKMNFTKPEARRWGQVKISKLKFMGLDRRGGTLGSHKKYKRNTTKKDSIYDIR
SFKKGSVAANVYKELIRRCMANIDATLNKEQPPIIDQWKEFQSTKSSQRESGDHLAMNRDEEVSEIDMLWKE
MELALASCYLLDDSEDSHAQYASNVRIGAEIRGEVCRHDYRLNEEIGIICRLCGFVSTEIKDVPPPFMPSSN
HNSSKEQRTEEATDHKQDDDGLDTLSIPVSSRAPSSSGGGEGNVWALIPDLGNKLRVHQKRAFEFLWKNIAG
SIVPAEMQPESKERGGCVISHTPGAGKTLLIISFLVSYLKLFPGSRPLVLAPKTTLYTWYKEVLKWKIPVPV
YQIHGGQTFKGEVLREKVKLCPGLPRNQDVMHVLDCLEKMQMWLSQPSVLLMGYTSFLTLTREDSPYAHRKY
MAQVLRQCGLLILDEGHNPRSTKSRLRKGLMKVNTRLRILLSGTLFQNNFGEYFNTLTLARPTFVDEVLKEL
DPKYKNKNKGASRFSLENRARKMFIDKISTVIDSDIPKKRKEGLNILKKLTGGFIDVHDGGTSDNLPGLQCY
TLMMKSTTLQQEILVKLQNQRPIYKGFPLELELLITLGAIHPWLIRTTACSSQYFKEEELEALQKFKFDLKL
GSKVKFVMSLIPRCLLRREKVLIFCHNIAPINLFLEIFERFYGWRKGIEVLVLQGDIELFQRGRIMDLFEEP
GGPSKVMLASITTCAEGISLTAASRVILLDSEWNPSKSKQAIARAFRPGQDKVVYVYQLLATGTLEEEKYKR
TTWKEWVSSMIFSEDLVEDPSHWQAPKIEDELLREIVEEDRATLFHAIMKNEKASNMGSLQE


|

2. `Point your browser to <bioinf.cs.ucl.ac.uk/psipred/>`_.

|
3. Copy and paste the amino acid sequence in the box and label the sequence. 

	.. figure:: img/protein_struct_1.png
|

4. We will use the previous submitted results:

http://bioinf.cs.ucl.ac.uk/psipred/result/e3f48c8e-28ff-11e7-879a-00163e110593


Tertiary Structure Prediction
------------------------------------

1. Frist find a structure similar to above sequence in PBD. We will use DELTA BLAST to search PBD.

	.. figure:: img/protein_struct_2.png
	
2. Click on the first significant hit to access the PDB. In case, you don't have BLAST results, use the following link to access the previous results. 
`Link <https://www.ncbi.nlm.nih.gov/protein/62738897?report=genbank&log$=protalign&blast_rank=2&RID=FTN4ETFX014>`_

3. `RCSB <http://www.rcsb.org/pdb/home/home.do>`_ provides curated content of PDB and use PDB ID: 1Z3I to visualize the protein in RCSB. 


4. Perform a multiple sequence alignment to find conserved sequences. 
|

	:a:. Retrive sequence from databank

	.. figure:: img/protein_struct_3.png
|
	:b:. Selected sequences are in the following fasta file. 
	
	https://github.com/ajwije/2017_spring_Bioinfo_class/blob/master/rad54.fasta
	
	:c:. Use `Tcoffee server <http://tcoffee.crg.cat/apps/tcoffee/do:expresso>`_  and align the sequences using structural information:
		

5. You can download crystal structure information from PDB in Cn3 format.

	.. figure:: img/protein_struct_4.png
	
6. Download `Cn3D software <https://www.ncbi.nlm.nih.gov/Structure/CN3D/cn3dinstall.shtml#browser>`_ from NCBI and install it on your computer. 

7. Open above Cn3 file using the Cn3D software.

8. Go to sequence viewer

	.. figure:: img/protein_struct_5.png
	
9. Under view, select find pattern:

	.. figure:: img/protein_struct_6.png


10. Copy a conserved region from multiple sequence alignment in the search window and click OK:

	.. figure:: img/protein_struct_7.png
	
11. You will see conserved region displayed on the crystal structure.

	.. figure:: img/protein_struct_8.png

