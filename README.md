# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers which come from the **[SSOAR repository](http://www.ssoar.info/)**. 
This corpus will grow constantly.

* and guideline files are available in [guidelinefiles](guidelinefiles/)


## big picture of "gold standard process"
![gold standard process](https://github.com/exciteproject/ssoar-gold-standard/blob/master/guidelinefiles/goldstandard-process.PNG "gold standard process")

## Content

At the moment there are 105 German and 100 English papers in this repository.
### How access to German papers:
There is five different folder in this repository.
* 1-[105 papers in German language which have a reference section at end of paper] (German_papers_ref_section_at_end_of_paper_1)
* 2-[100 papers in English language which have a reference section at end of paper] (2-English_papers)
* 3-[20 papers in German language which have references in footnote] (3-German_papers_with_footnote)
* 4-[117 papers in German language which have a reference section at end of paper] (4-References_extracted_from_Layout)
    * These papers are the second group of papers in German language which have a reference section at end of paper.
    * for these papers the layouts are extracted from pdf files but references are not checked manually.
* 5-[12 papers in German language which have a reference section at end of paper plus some short citation as footnote] (5-References_segmented_by_Annotatortool2)
    
* each folder again contains these  sub-folders
    1. pdfs
        * this folder contains pdf files which randomly picked from [SSOAR publications](http://www.ssoar.info/) (for understanding how they are selected see Selection method (### Selection method)).
    2. layouts
        * this folder contains extracted layout files from selected pdfs.
        * [CERMINE](https://github.com/CeON/CERMINE) is used for layout extraction
    3. Layout with references checked manually by EXRef-Identifier Tool
        * this folder contains layout files which all references strings are annotated and checked manually.
        * [EXRef-Identifier](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1) is used for checking identified reference strings in layout
    4. extracted References from Layouts
        * contains extracted reference strings from annotated layout files (the output of step 3).
        * [refext ](https://github.com/exciteproject/refext) is used for extracting reference strings from layout files.
    5. segmented References
        * this folder contains segmented reference strings
        * references are checked and edited manually by [EXRefmeta-Extractor Tool](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2)
    6. merged Layout and segmented references
        * this folder contains files that are a merge of layout and segmented reference strings.

        
### Selection method
We randomly select our papers from the 33,954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
### Files name
Files name are equal to SSOAR ID (For easier referencing).
> For example, ``12826.pdf`` refers to SSOAR ID 12826.
### How access to papers in SSOAR repository
By searching SSOARID (file name) in [https://www.gesis.org/ssoar/home/](https://www.gesis.org/ssoar/home/), you can access each paper(metadata and pdf).
### Selection criteria

* all selected papers are in German and English languages
* Publications that were in OCR or scanned (images) format or have watermark in background are excluded.
* all selected papers contain a reference section at end of paper or some citation as footnote .
* Number of References are in the range of: (3 < Reference < 50) 
