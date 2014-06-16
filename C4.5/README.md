C4.5
====

* Developed by Quinlan, successor of [ID3](http://en.wikipedia.org/wiki/ID3_algorithm)
* Wikipedia article on [C4.5](http://en.wikipedia.org/wiki/C4.5_algorithm)

The decision tree is built based on information entropy and recursion. Supervised.
Related to Occam's Razor (given two correct solutions, choose the simple one).


    # each sample s_i consists of a p-dimensional vector
    # representing feautures and the class of the sample
    sample = [2, 3, 9, 29, 1]

    samples = []
    
In each step, the algorithm splits the sample such that the attribute
used for the split yields the highest *normalized information gain*.

What are the base cases?

* All samples belong to the same class: Create a leaf and choose class.
* None of the features provide any gain: Create node higher up using expected value of the class.
* Instance of previously unseen class? Create a node higher up using the expected value.

Example training data:

* [Iris flower](http://en.wikipedia.org/wiki/Iris_flower_data_set) (1936)
* [More classical data sets](http://en.wikipedia.org/wiki/Data_set#Classic_datasets)
* [Weather and play](http://www2.cs.uregina.ca/~dbd/cs831/notes/ml/dtrees/c4.5/c4.5_prob1.html)
* [Life sciences](http://www.grappa.univ-lille3.fr/~torre/Recherche/Experiments/Datasets/)
* [Classification data sets](http://sci2s.ugr.es/keel/category.php?cat=clas)
* [Learning evaluation sets](ftp://ftp.cs.toronto.edu/pub/neuron/delve/data/tarfiles/)
