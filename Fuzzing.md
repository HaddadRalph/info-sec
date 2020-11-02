# Fuzzing

## What is Fuzzing

Fuzzing is an automated testing technique implemented by entering random or semi-random data as an input to record the behavior of the software in check. This is done to identify vulnerabilities that may arise during the testing phase such as bugs and implementation faults.

In addition to finding bugs, Fuzzing can be used to extract messages thrown by the app as a result of a user-input that attackers can exploit to their advantage. Examples of the messages outputed are error handling messages or messages containing a description of the vulnerablity "Incorrect Username" instead of "Incorrect Credentials".

## Fuzzer

A fuzzer is a program which injects automatically semi-random data into a program/stack and detect bugs. The data-generation part is made of generators, and vulnerability identification relies on debugging tools. Generators usually use combinations of static fuzzing vectors (known-to-be-dangerous values), or totally random data. New generation fuzzers use genetic algorithms to link injected data and observed impact.
