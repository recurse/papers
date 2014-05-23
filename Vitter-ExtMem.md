# External Memory Algorithms and Data Structures: Dealing with Massive Data

Jeffrey Scott Vitter

This paper is an updated version of the article in ACM Computing Surveys, Vol. 33, No. 2, June 2001

## Abstract

Data sets in large applications are often too massive to fit completely inside the computer’s internal
memory. The resulting input/output communication (or I/O) between fast internal memory and
slower external memory (such as disks) can be a major performance bottleneck. In this article
we survey the state of the art in the design and analysis of external memory (or EM ) algorithms
and data structures , where the goal is to exploit locality in order to reduce the I/O costs. We
consider a variety of EM paradigms for solving batched and online problems efficiently in external
memory.

For the batched problem of sorting and related problems like permuting and fast Fourier trans-
form, the key paradigms include distribution and merging. The paradigm of disk striping offers
an elegant way to use multiple disks in parallel. For sorting, however, disk striping can be nonop-
timal with respect to I/O, so to gain further improvements we discuss distribution and merging
techniques for using the disks independently. We also consider useful techniques for batched EM
problems involving matrices (such as matrix multiplication and transposition), geometric data
(such as finding intersections and constructing convex hulls) and graphs (such as list ranking,
connected components, topological sorting, and shortest paths). In the online domain, canonical
EM applications include dictionary lookup and range searching. The two important classes of in-
dexed data structures are based upon extendible hashing and B-trees. The paradigms of filtering
and bootstrapping provide a convenient means in online data structures to make effective use of
the data accessed from disk. We also reexamine some of the above EM problems in slightly dif-
ferent settings, such as when the data items are moving, when the data items are variable-length
(e.g., text strings), or when the allocated amount of internal memory can change dynamically.
Programming tools and environments are available for simplifying the EM programming task.
During the course of the survey, we report on some experiments in the domain of spatial databases
using the TPIE system (Transparent Parallel I/O programming Environment). The newly devel-
oped EM algorithms and data structures that incorporate the paradigms we discuss are signifi-
cantly faster than methods currently used in practice.

## Copyright

Permission to make digital or hard copies of part or all of this work for personal or classroom use is
granted without fee provided that copies are not made or distributed for profit or direct commercial
advantage and that copies show this notice on the first page or initial screen of a display along
with the full citation. 

## Comments

An extensive survey paper covering a broad spectrum of algorithms and datastructures for external memory.
Also covers modifications to algorithmic complexity that result from violating the O(1) random-access 
assumption for memory, so results also apply to modern memory hierarchies as well as traditional memory/disk
configurations.

## URLS

2007 Revised Paper: http://crono.dei.unipd.it/~lds/MATERIALE/Vit.IO_survey.pdf
2001 Original Paper: http://dl.acm.org/authorize?11441
2008 Book: http://www.ittc.ku.edu/~jsv/Papers/Vit.IO_book.pdf 
