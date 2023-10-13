# Supporting Reusable Model Migration with Edelta
- Lorenzo Bettini (Università degli studi Firenze, Firenze, Italy)
- Amleto Di Salle (Università Europea di Roma, Roma, Italy)
- Ludovico Iovino (Gran Sasso Science Institute, L'Aquila, Italy)
- Alfonso Pierantonio (Università degli studi dell'Aquila, L'Aquila, Italy)

## Abstract
In Model-Driven Engineering, metamodels define the vocabulary of concepts and relations that designers use to define a wide range of artifacts, including models, transformations, and editors. Therefore, whenever a metamodel undergoes modifications, the depending artifacts may no longer be valid, and consistency needs to be repaired through coupled evolution techniques. While several approaches have been proposed over the last decades, they are artifact- and domain-specific and do not facilitate the reuse of migration strategies. Indeed, migration strategies are often hard-coded for a given project in a specific domain. In this paper, we propose the novel concept of migration patterns to leverage reuse across different domains and projects. The approach extends the existing Edelta framework and has been evaluated by considering several case studies identified in a systematic literature review. 

## Research questions (RQs)
- RQ1: _What migration patterns are supported by the existing co-evolution approaches?_
- RQ2: _Are there migration patterns shared among multiple domains?_

The search strategy has been defined by answering the following four W-questions [1] -**Which?**, **Where?**, **What?**, and **When?**.

- **Which?**: Automatic and manual searches were performed for relevant papers from conferences and journals.
- **Where?**: The defined search strategy has been applied to digital libraries available online, in which we selected the following four to run the automated search to guarantee a certain level of quality of relevant papers:
   - **IEEE Xplore**: https://ieeexplore.ieee.org/Xplore/home.jsp,
   - **Scopus**: https://bit.ly/3m4T74d,
   - **Association for Computing Machinery (ACM)**: https://www.acm.org/
   - **dblp computer science bibliography**: https://dblp.uni-trier.de/
   - **Springer Link**: https://link.springer.com/

- **What?**: We defined a query string to be executed on different digital resources to collect papers. To this end, the **query string** that we conceived is the following: 

**Search String**:

(Title:("model migration") OR Title:("model co-evolution") OR Title:("model adaptation")) AND (Fulltext:(MDE) OR Fulltext:(Model Driven Engineering))

Note that we reported one of the strings executed on one of the digital libraries, the others are equivalent but with different syntax and operators.

Springer Link’s search engine does not allow a combined full-text or title search. Therefore, we limit the search to article titles, i.e.,  "model migration", "model co-evolution", and "model adaptation". As for Scopus, it does not permit full-text searching. Therefore, we limit the search to titles, keywords, and abstracts for "MDE" and "model driven engineering" keywords.

## Selection Process
Figure shows the process of searching and selecting relevant studies from the defined five databases. In the initial search, 215 studies have been identified. Then, the following selection process steps are executed to obtain the relevant studies.
![slr-search-selection-process](https://github.com/amletodisalle/JSS_edelta-migration-SLR/assets/25907051/fbcec487-064d-469f-b330-f224cf13efe5)

**Impurity removal:** In this step, we excluded non-research papers like books, reports, theses, and articles that were unavailable or not published in a journal or presented at a conference. After executing the impurity removal step, we obtained 203 studies, including 21  for the ACM, 1 for the DBLP, and 78 for the Springer databases. 

**Merge and duplicate removal:** We combined papers from the five sources into a single corpus and removed duplicates, resulting in 169 studies.

**Application of selection criteria 1st round:** During the first phase of study selection, the second and third authors examined the titles and abstracts of the studies and identified potential studies based on the following selection criteria. The authors included studies if they could not judge them by only reading the titles and abstracts. The selection criteria are organized in inclusion criteria (I):
I1 Studies subject to peer review;
I2 Studies that propose a tool-supported approach;
I3 Studies that clearly mention or propose migration patterns, i.e., evolution of the metamodel and corresponding migration strategy of the model;
whereas the exclusion criteria (E) of our study are reported in the following:
E1 Papers that are not written in English;
E2 Short papers, tutorial slides, or technical reports;
E3 Studies or tools working on artifacts that are not modeling artifacts, e.g., code adaptation. 
E4 Studies not reporting clear examples of the application of the migration pattern that do not permit the formalization of a clear migration pattern.
After the first round, 49 studies have been identified.

**Application of selection criteria 2nd round:** The second and third authors independently read the full papers coming from the first round. They made the final decision on whether a study should be selected or not. If a study was considered controversial, all the authors discussed it and agreed on whether it should be included. At the end of the second round, 14 studies have been selected.

**Snowballing:** We complemented the selection process using the snowballing technique[[2]](#2). In particular, we only conducted the backward snowballing activity where the third author read the references of the studies extracted in the first round of study selection. In the snowballing activity, we extracted 5 studies.

At the end of the searching and selecting process, 19 studies have been identified.

You can find the initial papers and all identified papers together with the final studies at the following [excel file](slr.xlsx)

## References
1. H. Zhang, M. A. Babar, and P. Tell. Identifying relevant studies in software engineering. Information and Software Technology, 53(6):625–637, 2011.
2. Guidelines for snowballing in systematic literature studies and a replication in software engineering. In M. J. Shepperd, T. Hall, and I. Myrtveit, editors, 18th International Conference on Evaluation and Assessment in Software Engineering, EASE ’14, London, England, United Kingdom, May 13-14, 2014, pages 38:1– 38:10. ACM, 2014. doi: 10.1145/2601248.2601268. URL https://doi.org/10.1145/2601248.2601268
