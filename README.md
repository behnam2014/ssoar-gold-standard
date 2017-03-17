## ssoar-gold-standard
This repository contains manually inspected datasets for evaluating the different steps during the citation information extraction process.


## ssoar-gold-standard/reference-extraction
1.ref-tags
		This folder contains Text of papers which are stored separately. In this files reference strings in reference section are tagged by <ref></ref>.
		Then name of each files contains two parts (ExciteID-SSOARID.txt -e.g 109-12826.txt, ExciteID: 109 and SSOARID:12826)
		By using this Url (http://www.ssoar.info/ssoar/handle/document/SSOARID), you can easily access to each paper (meta data+ Pdf). You only need to replace the SSOARID part in the URL.
	
2.ref-strings
		The reference strings (only in reference section) of a paper are extracted from <ref></ref> tags and saved in a text file.

## ssoar-gold-standard/reference-segmentation
The Extracted refrence strings from each papers fead to different tools and saved the result into the following listed subfolders. 
Metadata (e.g authors, years , titles and etc.) of each refernce strings are extracted by this tools.
			* Anystyle-parser (https://github.com/inukshuk/anystyle-parser)
			* Grobid (https://github.com/kermitt2/grobid)
			* Cermine(https://github.com/CeON/CERMINE)
			* manually_checked
				We picked outputs of Cermine and then Manually correct the tags of metadata in each refrence string (we only focuse on three tags 1- authors name , 2- titles 3- years)
