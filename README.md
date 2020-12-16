# FiniteAutomata

This repository is intended to contain code files for various properties of finite automata.
It is created for instructors who want to quickly provide/verify solutions. And for students who want to verify solutions. 

Version 1.0 contains code for following algorithm
  * NFA to DFA
  * NFA-null to NFA
  * Minimization of DFA
  * DFA to RE using State Elimination method
  
## Abbreviations
Following Abbreviations are used throughout this repository
* FA=Finite Automata
* NFA= Non-deterministic Finite Automata
* DFA= Deterministic Finite Automata
* NFA-null= Non-deterministic Finite Automata with null transitions
* RE= Regular Expression  

## Code
All the code files are in Jupyter Notebook Python 3

## Input
All codes take a transition table, in CSV file, as input. The following columns should be in the file

* state, this column contains name of file
* input_x column for each x in symbols,  a comma separated list of states that can be reached from state on symbol x
* isInitial, a binary column containing True if state is initial state and False otherwise.
* isFinal, a binary column containing True if state is final state and False otherwise.
For NFA-null following column is also required
* input_null column,  a comma separated list of states that can be reached from state of null input
### Input Example

An example CSV file for NFA-null given in figure is 

![](https://github.com/nNasir/FiniteAutomata/blob/master/NFAnull.JPG)

```
states,input_0,input_1,input_null,isInitial,isFinal
1,,,2,TRUE,FALSE
2,"2,3",,,FALSE,TRUE
3,,4,,FALSE,FALSE
4,,5,1,FALSE,FALSE
5,4,,,FALSE,FALSE
```
##Output
The output of each code will be printed in the notebook and is self-explanatory. Some of the working will also be printed to help understand the working of algorithm.


## Future Work.
Some more algorithms that should be added to this repository are

* Extended transition function of FA
* RE to FA

  

