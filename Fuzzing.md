# Fuzzing

## What is Fuzzing

Fuzzing is an automated Black Box software testing technique implemented by entering random or semi-random data as an input to record the behavior of the software in check. This is done to identify vulnerabilities that may arise during the testing phase such as bugs and implementation faults.

Fuzz testing was developed at the University of Wisconsin Madison in 1989 by Professor Barton Miller and students. Their [work](http://www.cs.wisc.edu/~bart/fuzz/) is mainly oriented towards command-line and UI fuzzing, and shows that modern ooperating systems are vulnerable to even simple fuzzing.

## The need of Fuzzing

The purpose of fuzzing relies on the assumption that there are bugs within every program, which are waiting to be discovered. Therefore, a systematic approach should find them sooner or later. Fuzzing can add another point of view to classical software testing techniques (hand code review, debugging) because of it’s non-human approach. It doesn’t replace them, but is a reasonable complement, thanks to the limited work needed to put the procedure in place.

Example on the matter, Fuzzing can be used to extract messages thrown by the app as a result of a user-input that attackers can exploit to their advantage. Examples of the messages outputed are error handling messages or messages containing a description of the vulnerablity "Incorrect Username" instead of "Incorrect Credentials".

## Fuzzer

A fuzzer is a program which injects automatically semi-random data into a program/stack and detect bugs. The data-generation part is made of generators, and vulnerability identification relies on debugging tools. Generators usually use combinations of static fuzzing vectors known values, or totally random data. New generation fuzzers use genetic algorithms to link injected data and observed impact.
