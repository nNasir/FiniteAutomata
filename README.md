# FiniteAutomata

This repository is intended to contained code files for various properties of finite automata.
Its is created to for instructors who want to quickly provide/verify solutions. And for students who want to verify solutions. 

Version 1.0 contains code for following algorithm
  * NFA to DFA
  * NFA-null to NFA
  * Minimization of DFA
  * DFA to RE using State Elimination method
  
## Abreviations
Following Abbreviations are used throughout this repositort
* FA=Finite Automata
* NFA= Nondeterminisitic Finite Automata
* DFA= Deterministic Finite Automata
* NFA-null= Nondeterminisitic Finite Automata with null transitions
* RE= Regular Expression  

## Input
All thse code file take a transition table in CSV file as input. The following columns should be in the file

* state, this colum contains name of file
* input_x column for each x in symbols,  a comma seperate list of states that can be reached from state on symbol x
* isInitial, a binary column containing True if state is initial state and False other wise.
* isFinal, a binary column containing True if state is final state and False other wise.
For NFA-null following column is also required
* input_null column,  a comma seperate list of states that can be reached from state of null input
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
The output of each code will be printed in the notebook and is self explanatory. Some of the working will also be printed to help understand the working of algorithm.


## Future Work.
Some more algorithms that should be added to this repository are

* Extended transition function of FA
* RE to FA

  

