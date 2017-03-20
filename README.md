# SSOAR Gold Standard


This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. All datasets consist of research papers in German and come from the [SSOAR repository](http://www.ssoar.info/).

## Content

* [reference-extraction](reference-extraction)
	* [ref-tags](reference-extraction/ref-tags)

	    Currently contains 85 randomly picked German SSOAR publications with annotated reference strings (see [Paper Selection](#paper-selection)).
	* [ref-strings](reference-extraction/ref-strings)

		The reference strings (only in reference section) of papers are extracted from <ref></ref> tags and saved in text files. Each text file contains references of a paper and each reference string is saved in a separated line.

* [reference-segmentation](reference-segmentation)
	* [cermine/xml](reference-segmentation/cermine/xml)

## Paper Selection

We randomly select our papers from the 33954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
The random order of SSOAR publications that we used can be found at [random-ssoar-ids.csv](corpus/de/random-ssoar-ids.csv).
For easier referencing we introduce a second ID, the EXCITEID, which refers to the position of a SSOAR ID in the above list.
For example, ``109-12826.pdf`` refers to SSOAR ID 12826 which appears in line 109 in [corpus/de/random-ssoar-ids.csv](corpus/de/random-ssoar-ids.csv).
By replacing SSOARID in [http://www.ssoar.info/ssoar/handle/document/SSOARID](http://www.ssoar.info/ssoar/handle/document/SSOARID), you can access each paper (metadata + pdf).

We excluded the following publications from our gold standard:

* Non-German publications
* Publications that were scanned
* Publications that do not contain a reference section

A list of excluded papers can be found at ...











