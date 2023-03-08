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

- **Which?** Automatic and manual searches were performed for relevant papers from conferences and journals.
- **Where?** The defined search strategy has been applied to digital libraries available online, in which we selected the following four to run the automated search to guarantee a certain level of quality of relevant papers: \textit{IEEE Xplore}\footnote{\url{https://ieeexplore.ieee.org/Xplore/home.jsp}},
   \textit{Scopus}\footnote{\url{https://bit.ly/3m4T74d}},
    \textit{Association for Computing Machinery (ACM)}\footnote{\url{https://www.acm.org/}},
     \textit{dblp computer science bibliography}\footnote{\url{https://dblp.uni-trier.de/}}, and \textit{Springer}\footnote{\url{https://www.springer.com/}}.

-**What?** We defined a query string to be executed on different digital resources to collect papers. To this end, the \textit{query string} that we conceived is the following\footnote{We reported one of the strings executed on one of the digital libraries, the others are equivalent but with different syntax and operators.}:


\textbf{Search String:} \texttt{(Title:("model migration") OR Title:("model co-evolution")) AND (Fulltext:(MDE) OR Fulltext:(Model Driven Engineering))}

    For each paper collected, its title and abstract were extracted.
    The selection criteria used for this study are organized in inclusion criteria (I):
\begin{itemize}
    \item[I1] Studies subject to peer review (e.g., papers published in conference proceedings or in journals are considered, whereas white papers or technical reports are excluded);
    \item[I2] Studies that propose a tool-supported approach;
    \item[I3] Studies that clearly mention or propose migration patterns, i.e., evolution of the metamodel and corresponding migration strategy of the model;
    \end{itemize}
    whereas the
exclusion criteria (E) of our study are reported in the following:
    \begin{itemize}
    \item[E1] Papers that are not written in English;
    \item[E2] Short papers, tutorial slides or technical reports;
    \item[E3] Book chapters;
    \item[E4] Studies or tools working on artifacts that are not modeling artifacts, e.g., code adaptation. 
\item[E5] Studies not reporting clear examples of the application of the migration pattern.
\end{itemize}
    \item[] \emph{When?} We considered papers that have been published in the period 2005--2022
\end{itemize}

The extraction process generated 194 papers and we applied the filtering criteria to get 69 papers

## Pubblication trends (RQ1)
To answer RQs, we conducted a lightweight literature review to identify the publication trends of this 15-year-long collaboration over time.
We collected the data through the web search engine [Google Scholar](https://scholar.google.com) using the following search string: 

_rubus AND component AND model_

We did a full-text search. The RCM was formally defined in 2008 by Häanninen et al. [1], but the first hints on RCM date back to 2003. 
For this reason, we carried out our search from 2003 to date (December 15, 2022). 

The initial search gave [265 results](google-scholar.csv). Then, we removed impurities and duplicates; eventually, we applied the following inclusion and exclusion criteria:
- **I1**: Studies written in English
- **I2**: Studies exploiting the Rubus Component Model 
- **E1**: Studies with full-text not available
- **E2**: Studies in the form of tutorial papers, editorials, reports, etc., since they do not carry the type of information that we seek.

At the end of the process, we obtained a set of [171 primary studies](final-studies.xlsx).

## References
1. Hänninen, K., Mäki-Turja, J., Nolin, M., Lindberg, M., Lundbäck, J., Lundbäck, K.: The rubus component model for resource onstrained real-time systems. In: IEEE Third International Symposium on Industrial Embedded Systems, SIES 2008, Montpellier / La Grande Motte, France, June 11-13, 2008, p. 177–183. IEEE (2008). https://doi.org/10.1109/SIES.2008.4577697
