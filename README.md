# FiniteAutomata

This repository is intended to contained code files for various properties of finite automata.
Its is created to for instructors who want to quickly provide/verify solutions. And for students who want to verify solutions. 

Version 1.0 contains code for following algorithm
  * NFA to FA
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
### Example

And Example CSV file for FA given in figure is 
![NFA null](NFAnull.png)

