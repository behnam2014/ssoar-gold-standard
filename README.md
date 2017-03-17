## ssoar-gold-standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. All datasets consist of research papers in German and come from the SSOAR repository http://www.ssoar.info/.


## ssoar-gold-standard/reference-extraction

	1. ref-tags
		This folder contains text of randomly picked SSOAR papers. In these files, reference strings in reference sections are tagged by <ref></ref>.
		The name of each files contains two parts (ExciteID-SSOARID.txt - e.g 109-12826.txt, ExciteID: 109 and SSOARID:12826)
		By using this url (http://www.ssoar.info/ssoar/handle/document/SSOARID), you can easily access each paper (meta data+ pdf). You only need to replace the SSOARID part in the URL.
	
	2. ref-strings
		The reference strings (only in reference section) of papers are extracted from <ref></ref> tags and saved in text files. Each text file contains references of a paper and each reference string is saved in a separated line.

## ssoar-gold-standard/reference-segmentation
The extracted reference strings from each paper were fed to different tools and the result also were saved into the following listed subfolders. 
Metadata (e.g authors, years, titles and etc.) of each reference string were extracted by these tools.
			
			1. Anystyle-parser (https://github.com/inukshuk/anystyle-parser)
			2. Grobid (https://github.com/kermitt2/grobid)
			3. Cermine (https://github.com/CeON/CERMINE)
			4. manually_checked
				We picked outputs of Cermine and then manually correct the tags of metadata in each refrence string (we only focuse on three tags 1- authors name , 2- titles 3- years)
