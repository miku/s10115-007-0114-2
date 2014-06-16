README
======

Code for top 10 data mining algorithms identified by the IEEE
International Conference on Data Mining (ICDM) in December 2006.

* C4.5
* k-means
* SVM
* Apriori
* EM
* PageRank
* AdaBoost
* kNN
* Naive Bayes
* CART

Cover classification, clustering, statistical learning, association analysis, link mining.

Candidate list: http://www.cs.uvm.edu/~icdm/algorithms/CandidateList.shtml

C4.5
====

Basic formulation: Given a set of cases with fixed attributes each belonging to one class, work out the class of a new case, based on its attribtues.

Is a descendent of ID3 and ILS. Ruleset or decision tree form.

Desicion tree
-------------

First construct a decision tree via divide and conquer:

* If all elements in S belong to the same class or S is small, the tree
  is a leaf, labeled with the most frequent class

* Otherwise, choose a test based on a single attribute with two or more
  outcomes. This test is the root of the tree and it partitions S into
  subsets S_1, S_2, ... according to the number of outcomes. Apply this
  procedure recursively in this set.

