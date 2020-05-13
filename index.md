## DeepName


Names play an important role in software development and maintenance. Poor names might hinder code comprehension, increase maintenance cost, or even lead to software bugs. Method names are of particular importance because methods provide the cornerstone of abstraction for developers to communicate with each other for various purposes. Existing method naming approaches often represent code as lexical tokens or syntactical AST (abstract syntax tree) paths, failing to bridge the gap between code syntax and semantics. Initial attempts have been made to represent code as execution traces for capturing code semantics, but suffer scaliabiltiy in collecting traces. In this paper, we propose DeepName, which uses our novel neural network model, Meth2Vec, to encode a method as a continuous distributed vector, and then feeds the encoded vector to an encoder-decoder model to suggest the method name. Meth2Vec represents a method as 1) a bag of paths on the program dependence graph, and 2) a sequence of translated intermediate representation statements, to scalably capture code semantics. Our evaluation results on a dataset of 156.3K methods in 56 Java projects have demonstrated that DeepName outperforms the two state-of-the-art approaches in F1-score by 36.9% and 10.0% if we split the dataset according to projects and by 30.7% and 17.6% if we split the dataset according to methods. The paper about this work has been submitted to ICSE 2020.



### Source Code

You can download the source code of Drex [here](code.zip)

### Dataset

Due to the large volume of our dataset, please contact *17839227248@163.com* for further use.
