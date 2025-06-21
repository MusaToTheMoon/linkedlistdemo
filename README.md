### HOW TO RUN
To run, first clean: ./clean.sh

Then, run infer: infer run --purity -- javac LinkedListDemo.java

### Current results

--purity correctly classifies 6 functions as pure, and all are TPs. It also has 0 FNs, meaning it doesn't miss any pure function.
--impurity correctly classifies 7 functions as impure, and 6 of these are TPs. The remaining one seems to be an error, as Infer seems to be classifying a function twice. Also, --impurity has 0 FNs, too, meaning it doesn't miss any impure functions.
