# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers which come from the **[SSOAR repository](http://www.ssoar.info/)**. 
This corpus will grow constantly.

## big picture of "gold standard process"
![gold standard process](https://github.com/exciteproject/ssoar-gold-standard/blob/master/guidelinefiles/goldstandard-process.PNG "gold standard process")

## Content

### How access to German papers:
There is six different folder in this repository.
* [1-German_papers_ref_section_at_end_of_paper_1](German_papers_ref_section_at_end_of_paper_1)
    * In this folder there is 105 papers in German language.
    * There is a reference section at end of these papers.
* [2-English_papers](2-English_papers)
    * In this folder there is 100 papers in English language.
    * There is a reference section at end of these papers.
* [3-German_papers_with_footnote](3-German_papers_with_footnote)
    * In this folder there is 20 papers in German language.
    * These papers have references in footnote.
* [4-References_extracted_from_Layout](4-References_extracted_from_Layout)
    * In this folder there is 117 papers in German language.
    * These papers are the second group of papers in German language which have a reference section at end of paper.
    * for these papers the layouts are extracted from pdf files but references are not checked manually.
* [5-References_segmented_by_Annotatortool2](5-References_segmented_by_Annotatortool2)
    * In this folder there is 12 papers in German language.
    * These papers have a reference section at end of paper plus some short citation as footnote.
* [guidelinefiles](guidelinefiles/)
   * There is one guideline files in this folder.

    
Each folder again contains several sub-folders:
1. Pdfs
    * This folder contains pdf files which randomly picked from [SSOAR publications](http://www.ssoar.info/)(for understanding how they are selected see Selection method).
2. Layouts
    * This folder contains extracted layout files from selected pdfs.
    * [CERMINE](https://github.com/CeON/CERMINE) is used for layout extraction
3. Layout with references checked manually by EXRef-Identifier Tool
    * This folder contains layout files which all references strings are annotated and checked manually.
    * [EXRef-Identifier](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1) is used for checking identified reference strings in layout files.
4. Extracted References from Layouts
    * This folder contains extracted reference strings from annotated layout files (the output of step 3).
    * [refext ](https://github.com/exciteproject/refext) is used for extracting reference strings from layout files.
5. Segmented References
    * this folder contains segmented reference strings
    * references are checked and edited manually by [EXRefmeta-Extractor Tool](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2)
6. Merged Layout and segmented references
    * this folder contains again layout files which are merged with segmented reference strings.

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
* selected papers contain a reference section at end of the paper or some citation as a footnote .
* Number of References are in the range of: (3 < Reference < 50) 
