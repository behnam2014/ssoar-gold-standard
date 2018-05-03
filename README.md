# SSOAR Gold Standard


This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers in German and come from the [SSOAR repository](http://www.ssoar.info/). We will constantly grow this corpus.

## Content
The latest update of files is available in [v3-2018-Mai](https://github.com/exciteproject/ssoar-gold-standard/tree/master/v3-2018-04-24). Other folders are an archive of former files.
* [v3-2018-Mai](v3-2018-Mai)
    *[1-pdfs](v3-2018-Mai/1-pdfs)
        contains pdf files
    *[2-layouts](v3-2018-Mai/2-layouts)
        contains extracted layouts from pdfs by [efext](https://github.com/exciteproject/refext)
    *[3-Layout_and_refs_merged_and_checked_by_Anno1](v3-2018-Mai/3-Layout_and_refs_merged_and_checked_by_Anno1)
        contains extracted annotated reference strings in layout. reference strings checked and edited by our Annotator Tools
    *[4-References_extracted_from_Layout](v3-2018-Mai/4-References_extracted_from_Layout)
        contains extracted reference strings from annotated layout files
    *[5-References_segmented_by_Anno2](v3-2018-Mai/5-References_segmented_by_Anno2)
        contains segmented reference strings which checked and edited by our Annotator Tools
    *[6-Layout_and_segmentated_ref_merged](v3-2018-Mai/6-Layout_and_segmentated_ref_merged)
        contains merge of layout and segmented reference strings

## Paper Selection

We randomly select our papers from the 33,954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
For easier referencing we introduce a second ID, the EXCITEID, which refers to the position of a SSOAR ID in the above list.
Files name are equal to SSOAR ID (For easier referencing).
For example, ``12826.pdf`` refers to SSOAR ID 12826.
By replacing SSOARID in [https://www.gesis.org/ssoar/home/](https://www.gesis.org/ssoar/home/), you can access each paper (metadata + pdf).

We excluded the following publications from our gold standard:

* Non-German and Non-English publications
* Publications that were in OCR format or scanned (images)
* Publications that do not contain a reference section
* Publications that have more than 50 and less than 3 references in their reference section

A list of excluded papers can be found [here](v3-2018-Mai).











