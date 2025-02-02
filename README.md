# SIGCSE2021-dataset

This repositary contains the dataset used in the paper **Towards a Human-AI hybrid system for categorising programming problems**, published in SIGCSE 2021 conference. We scraped 5213 programming problem statements, merged and unified the labels from the [URI Online Judge](urionlinejudge.com.br) and [A2 Online Judge](a2oj.com/about). In both systems, the problem categories were annotated either by the problem creators, or by expert users, who had already solved the problem.

Some issues occurred from the start, as the problems were categorised differently in the two systems. Whilst URI used 8 computer science (macro-)subjects, A2 used finer-grained segregation, with a total of 152 categories. The reason for so many categories was that the maintainers manually labelled the problems with a plethora of specific categories, such as minimum spanning tree, depth-first search, flood fill, which could easily be classified into a more general category, such as graph. Such extremely detailed categorisation led also to extreme sparsity, with some classes with 1-2 problem instances only. To be more precise, 75 of the A2 categories contain less than 10 problems, rendering the data hard for  machine learning. The well-known book entitle "Competitive Programming 3" only recommends a limited number of categories -- the ones used by URI as macro-categories. Thus, we map the categories of A2 over the macro-categories of URI.

If you use our dabase or code for a scientific publication, we would appreciate citations to the following paper:

**APA**

Pereira, F. D., Pires, Francisco, Fonseca, S. C., Oliveira, E. H., Carvalho, L. S, Oliveira, D. B & Cristea, A. I. 2020. Towards a Human-AI hybrid system for categorising programming problems. In Proceedings of the 52st ACM Technical Symposium on Computer Science Education (SIGCSE '21).  Association for Computing Machiner. DOI:https://doi.org/10.1145/3408877.3432422.

**Bibtex**

@inproceedings{pereira2021sigcse,
author={Pereira, Filipe Dwan and Pires, Francisco and Fonseca, Samuel C and Oliveira, Elaine HT and Carvalho, Leandro SG and Oliveira, David BF and Alexandra I},
title = {Towards a Human-AI hybrid system for categorising programming problems},
year = {2021},
isbn = {97814503806212103},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3408877.3432422},
doi = {10.1145/3408877.3432422},
numpages = {7},
series = {SIGCSE '21}
}
