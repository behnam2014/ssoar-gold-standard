## ssoar-gold-standard
This repository contains manually inspected datasets for evaluating the different steps during the citation information extraction process.


## ssoar-gold-standard/reference-extraction

	1. ref-tags
		This folder contains text of randomly picked SSOAR papers. In these files, reference strings in reference section are tagged by <ref></ref>.
		Then name of each files contains two parts (ExciteID-SSOARID.txt - e.g 109-12826.txt, ExciteID: 109 and SSOARID:12826)
		By using this Url (http://www.ssoar.info/ssoar/handle/document/SSOARID), you can easily access to each paper (meta data+ Pdf). You only need to replace the SSOARID part in the URL.
	
	2. ref-strings
		The reference strings (only in reference section) of papers are extracted from <ref></ref> tags and saved in text files. Each text file contains references of a paper and each reference string is saved in a seprated line.

## ssoar-gold-standard/reference-segmentation
The Extracted refrence strings from each papers were feaded to different tools and the result also were saved into the following listed subfolders. 
Metadata (e.g authors, years , titles and etc.) of each refernce strings were extracted by these tools.
			
			1. Anystyle-parser (https://github.com/inukshuk/anystyle-parser)
			2. Grobid (https://github.com/kermitt2/grobid)
			3. Cermine(https://github.com/CeON/CERMINE)
			4. manually_checked
				We picked outputs of Cermine and then Manually correct the tags of metadata in each refrence string (we only focuse on three tags 1- authors name , 2- titles 3- years)
