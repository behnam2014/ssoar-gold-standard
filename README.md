# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers which come from the **[SSOAR repository](http://www.ssoar.info/)**. 
This corpus will grow constantly.

## big picture of "gold standard process"
![gold standard process](https://github.com/exciteproject/ssoar-gold-standard/blob/master/6-Guidelinefiles/goldstandard-process.PNG "gold standard process")

## Content
* Number of all papers in repository: 354
* Number of German papers in repository: 254
* Number of English papers in repository: 100
* Number of processed papers up until now: 225

### How access to papers:
**There are six different folders in this repository.**
* [1-German_papers_with_reference_section_at_end_of_paper_first_group](1-German_papers_with_reference_section_at_end_of_paper_first_group)
    * In this folder there are 105 papers in German language.
    * At the end of each paper there is a reference section.
    * This is the first group of selected papers for checking.
* [2-English_papers_with_reference_section_at_end_of_paper](2-English_papers_with_reference_section_at_end_of_paper)
    * In this folder there are 100 papers in English language.
    * At the end of each paper there is a reference section.
* [3-German_papers_with_footnote](3-German_papers_with_footnote)
    * In this folder there are 20 papers in German language.
    * These papers have some references as a footnote.
* [4-German_papers_with_reference_section_at_end_of_paper_second_group](4-German_papers_with_reference_section_at_end_of_paper_second_group)
    * In this folder there are 117 papers in German language.
    * These papers are the second group of papers in German language which selected for processing.
    * At the end of each paper there is a reference section.
    * For these papers the layouts are extracted from pdf files but references are not checked manually.
* [5-German_papers_with_reference_section_at_end_of_paper_plus_short_citation_footnote](5-German_papers_with_reference_section_at_end_of_paper_plus_short_citation_footnote)
    * In this folder there are 12 papers in German language.
    * There is a reference section at the end of each paper plus some short citation as footnote.
    * For these papers the layouts are extracted from pdf files but references are not checked manually.
* [6-Guidelinefiles](6-Guidelinefiles/)
   * All guideline files will be located in this folder.

    
**Each folder contains several sub-folders:**
1. **Pdfs**
    * This folder contains pdf files which are randomly picked from [SSOAR publications](http://www.ssoar.info/)(for understanding how they are selected see **Selection method**).
2. **Layouts**
    * This folder contains extracted layout files from selected pdfs.
    * [CERMINE](https://github.com/CeON/CERMINE) is used for Generating layout CSV files from given PDFs.
3. **Layout with identified references**
    * This folder contains layout files plus identified references and all the reference strings are annotated and checked manually.
    * [EXRef-Identifier](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1) is used for checking identified reference strings in layout files.
4. **Extracted References from Layouts**
    * This folder contains extracted reference strings from annotated layout files (the output of step 3).
    * [refext ](https://github.com/exciteproject/refext) is used for extracting reference strings from layout files.
5. **Segmented References**
    * This folder contains segmented reference strings.
    * references are checked and edited manually by [EXRefmeta-Extractor Tool](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2)
6. Merged Layout and segmented references
    * This folder contains layout files(from step 3) which are merged with segmented reference strings(from step 5).

### Selection method
We randomly select our papers from the 33,954 available publications in [SSOAR repository](http://www.ssoar.info/).
### Files name
Files name are equal to SSOAR ID (For easier referencing).
> For example, ``12826.pdf`` refers to SSOAR ID 12826.
### How access to papers in SSOAR repository
By searching SSOARID (file name) in [SSOAR repository](http://www.ssoar.info/), you can access each paper(metadata and pdf).

### Selection criteria
* selected papers are in German or English languages. (other languages are excluded)
* selected papers are not in OCR or scanned (images) format or do not have a watermark in the background.
* selected papers contain a reference section at end of the paper or some short citation as a footnote .
* Number of References are in the range of: (3 < Reference < 50) 
