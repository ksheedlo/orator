orator
======

Analyzing patterns in natural language for poetry, art and rhetoric

This is a side project from some time ago that I'm revisiting.
It was originally written in C, but I'm rewriting it in Python because
the original version was rather unsophisticated and building out the 
complexity I need in C would just be painful. What it does is takes in
a body of text and computes a Markov model where each state is a word
and each branch is each possible next word, weighted by the number of 
times it occurs. I've run the original on the Gettysburg Address and 
various classics. Results are hilarious, if a bit incoherent. I'm in 
the process of modifying it to handle word chains of arbitrary length,
or at least up to four. This should hopefully clean the voice up a bit
and make it sound a bit more human. 