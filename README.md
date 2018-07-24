# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers which come from the **[SSOAR repository](http://www.ssoar.info/)**. 
This corpus will grow constantly.

## About Versioning
The latest update of files is available in [v2-2018-Mai](https://github.com/exciteproject/ssoar-gold-standard/tree/master/v2-2018-Mai). 
Other folders are an archive of former versions.

*[v1-2017-Jun](v1-2017-Jun/) [Readme file](v1-2017-Jun/)
*[v2-2018-Mai](v2-2018-Feb/) Last Update
*guideline files (guidelinefiles/)

** the following note is related to the last version.

## big picture of "gold standard process"
![gold standard process](https://github.com/exciteproject/ssoar-gold-standard/blob/master/guidelinefiles/goldstandard-process.PNG "gold standard process")

## Content

At the moment there are 105 German and 100 English papers in this repository.
### How access to German papers:
* [v2-2018-Mai/1-German_papers](v2-2018-Mai/1-German_papers)
    1. [pdfs](v2-2018-Mai/1-German_papers/1-pdfs)
        * contains selected pdf files.
    2. [layouts](v2-2018-Mai/1-German_papers/2-layouts)
        * contains extracted layout files from selected pdfs.
        * **[refext](https://github.com/exciteproject/refext)** is used for layout extraction
    3. [Layout_and_refs_merged_and_checked_by_Anno1](v2-2018-Mai/1-German_papers/3-Layout_and_refs_merged_and_checked_by_Anno1)
        * contains layout files with annotated reference strings.
        * These reference strings are checked and edited by our [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1)
    4. [References_extracted_from_Layout](v2-2018-Mai/1-German_papers/4-References_extracted_from_Layout)
        * contains extracted reference strings from annotated layout files (the output of step 3).
    5. [References_segmented_by_Anno2](v2-2018-Mai/1-German_papers/5-References_segmented_by_Anno2).
        * contains segmented reference strings 
        * These reference strings are checked and edited by [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2).
    6. [Layout_and_segmentated_ref_merged](v2-2018-Mai/1-German_papers/6-Layout_and_segmentated_ref_merged)
        * contains a merge of layout and segmented reference strings.

### How access to English papers
* [v2-2018-Mai/2-English_papers](v2-2018-Mai/2-English_papers)
    1. [pdfs](v2-2018-Mai/2-English_papers/1-pdfs)
        * contains selected pdf files.
    2. [layouts](v2-2018-Mai/2-English_papers/2-layouts)
        * contains extracted layout files from selected pdfs.
        * **[refext](https://github.com/exciteproject/refext)** is used for layout extraction
    3. [Layout_and_refs_merged_and_checked_by_Anno1](v2-2018-Mai/2-English_papers/3-Layout_and_refs_merged_and_checked_by_Anno1)
        * contains layout files with annotated reference strings.
        * These reference strings are checked and edited by our [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1)
    4. [References_extracted_from_Layout](v2-2018-Mai/2-English_papers/4-References_extracted_from_Layout)
        * contains extracted reference strings from annotated layout files (the output of step 3).
    5. [References_segmented_by_Anno2](v2-2018-Mai/2-English_papers/5-References_segmented_by_Anno2).
        * contains segmented reference strings 
        * These reference strings are checked and edited by [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2).
    6. [Layout_and_segmentated_ref_merged](v2-2018-Mai/2-English_papers/6-Layout_and_segmentated_ref_merged)
        * contains a merge of layout and segmented reference strings.
        
### Selection method
We randomly select our papers from the 33,954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
### Files name
Files name are equal to SSOAR ID (For easier referencing).
> For example, ``12826.pdf`` refers to SSOAR ID 12826.
### How access to papers in SSOAR repository
By searching SSOARID (file name) in [https://www.gesis.org/ssoar/home/](https://www.gesis.org/ssoar/home/), you can access each paper(metadata and pdf).
### Selection criteria
We excluded the following publications from our gold standard:

* Non-German and Non-English publications
* Publications that were in OCR or scanned (images) format or have watermark in background.
* Publications that do not contain a reference section.
* Publications that have more than 50 or less than 3 references in their reference section.
