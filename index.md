### METH2SEQ
Program semantic properties such as class names, method names, and variable names and types play an important role in software development and maintenance. They provide the cornerstone of abstraction for developers to communicate with each other for various purposes (e.g., code review and program comprehension). Existing program semantic property prediction approaches often represent code as lexical tokens or syntactical AST (abstract syntax tree) paths, failing to bridge the gap between code syntax and code semantics hindering their effectiveness in predicting program properties. Initial attempts have been made to represent code as execution traces for capturing code semantics, but suffer scaliabiltiy in collecting execution traces.

In this paper, we propose a hybrid code representation learning approach, named METH2SEQ, to encode a method as a sequence of distributed vector. METH2SEQ represents a method as 1) a bag of paths on the program dependence graph, 2) a sequence of typed intermediate representation statements and 3) a sentence of natural language comment, to scalably capture code semantics. The learned sequence of vectors of a method can be fed to a decoder model to predict program properties. Our evaluation results on the difficult task of method name prediction with a dataset of 280.5K methods in 67 Java projects have demonstrated that METH2SEQ outperforms the two state-of-the-art code representation learning approaches in F1-score by 92.6% and 36.6%, while also outperforming two state-of-the-art method name prediction approaches in F1-score by 85.6% and 178.1%.

### CODE
You can download the source code of Meth2Vec and DeepName from [here](meth2seq.zip)

### DATASET
Due to the large volume of our dataset (aroud 25 GB), please contact *rachmanino@yahoo.com* for further use.
