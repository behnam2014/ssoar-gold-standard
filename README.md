## ssoar-gold-standard
This repository contains manually inspected datasets for evaluating the different steps during the citation information extraction process.


##ssoar-gold-standard/reference-extraction/
	1.ref-tags
		This folder contains Text of papers which are stored seprately. In this files refrence strings in refrence section are tagged by <ref></ref>.
		Then name of each files contains two parts (ExciteID-SSOARID.txt -e.g 109-12826.txt, ExciteID: 109 and SSOARID:12826)
		By using this Url (http://www.ssoar.info/ssoar/handle/document/SSOARID), you can easily access to each papers (meta data+ Pdf). You only needs to replace SSOARID part in the URl.
	
	2.ref-strings
		The refrence strings (only in refrence section) of a paper are extracted from <ref></ref> tags and saved in a file for a papers.

##ssoar-gold-standard/reference-segmentation/
The Extracted refrence strings from each papers fead to different tools and saved the result into the following subfolders:
	1. Anystyle-parser
		(https://github.com/inukshuk/anystyle-parser)
	2. Grobid
		(https://github.com/kermitt2/grobid)
	3. Cermine
		(https://github.com/CeON/CERMINE)

##
