Dependency to Lambda-calculus Conversion Rules
==============================================
Overview
--------
The files in this repository contain rules for conversion of syntactic dependency trees (in the "[Stanford dependencies style](http://nlp.stanford.edu/software/dependencies_manual.pdf
)" to lambda-calculus logical forms representing the semantics of a sentence or question.

These rules are described in more detail in the paper:  
Siva Reddy, Oscar T&auml;ckstr&ouml;m, Michael Collins, Tom Kwiatkowski, Dipanjan Das, Mark Steedman, Mirella Lapata (2016). *Transforming Dependency Structures to Logical Forms for Semantic Parsing*. Transactions of the Association for Computational Linguistics, vol 4.

Note that this repository does not include any software required to apply these rules.

Content
-------
The rules consists of the following files:

* [dependency-transformation-rule.proto](../master/dependency-transformation-rule.proto):  
   Protocol buffer format in which the rules are specified.

* [transformation-rules.pb.txt](../master/transformation-rules.pb.txt):  
   Transformation rules that modify the dependency-tree (e.g., by adding BIND operations) and relabeling dependencies to simplify lambda expression assignment.

* [assignment-rules.pb.txt](../master/assignment-rules.pb.txt):  
  Lambda-calculus assignment rules, which assign lambda-calculus expressions to each leaf node in the s-expressions.

License
-------
This work is licensed by Google Inc. under a Creative Commons Attribution 4.0 International License.  
![alt text](https://licensebuttons.net/l/by/4.0/88x31.png "CC-BY")
