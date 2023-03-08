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
   - **Springer**: https://www.springer.com/

- **What?**: We defined a query string to be executed on different digital resources to collect papers. To this end, the **query string** that we conceived is the following: 

**Search String**:

(Title:("model migration") OR Title:("model co-evolution")) AND (Fulltext:(MDE) OR Fulltext:(Model Driven Engineering))

Note that we reported one of the strings executed on one of the digital libraries, the others are equivalent but with different syntax and operators.

For each paper collected, its title and abstract were extracted.
The selection criteria used for this study are organized in inclusion criteria (I):
- **I1**: Studies subject to peer review (e.g., papers published in conference proceedings or in journals are considered, whereas white papers or technical reports are excluded);
- **I2**: Studies that propose a tool-supported approach;
- **I3**: Studies that clearly mention or propose migration patterns, i.e., evolution of the metamodel and corresponding migration strategy of the model;

whereas the

exclusion criteria (E) of our study are reported in the following:
- **E1**: Papers that are not written in English;
- **E2**: Short papers, tutorial slides or technical reports;
- **E3**: Book chapters;
- **E4**: Studies or tools working on artifacts that are not modeling artifacts, e.g., code adaptation. 
- **E5**: Studies not reporting clear examples of the application of the migration pattern.

- **When?**: We considered papers that have been published in the period 2005-2022

The extraction process generated 194 papers and we applied the filtering criteria to get 68 papers. You can find the initial papers and final studies at the following [excel file](slr.xlsx)



## References
1. H. Zhang, M. A. Babar, and P. Tell. Identifying relevant studies in software engineering. Information and Software Technology, 53(6):625–637, 2011.
