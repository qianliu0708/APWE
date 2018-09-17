# APWE
Code for APWE method, introduced in paper "Leveraging Pattern Associations for Word Embedding Models" (DASFAA'17).
-------------------------------------------------------------------------------------------------------------------

Installation: type make

To run this code, type:

    ./word2vec -train corpus.txt -output result.txt -cbow 1 -size 300  -negative 25 -hs 1 -sample 1e-4 -threads 20 -binary 0 -pattern pattern_test1.txt -pro 20


Here,

-train is the training corpus

-output is the output word embedding file

-pattern is the file of patterns, example file is in code/pattern_test1.txt 

-pro is parameter which controls the combination of contextual information and pattern information (defined as alpha/beta in the paper)

Usually, the other hyper-parameters such as the learning rate do not need to be tuned for different training sets. 
