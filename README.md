Multiplatform CTF implementation and use in the FreeBSD kernel debugger
-----------------------------------------------------------------------

The goal of the thesis is to provide an open-source implementation of
the Compact C Type Format (CTF) in the form of a C99 library with an
appropriate free documentation of both the format itself and the
corresponding API. A strong emphasis is being placed on the
multiplatform availability of the library - BSD, illumos and Linux
worlds included.

Functionality and correctness of the library will be verified by unit
testing of its core components with sufficient code coverage.  Part of
the CTF tool-chain is also a set of command-line utilities such as
one-way conversion from DWARF to CTF, merging two CTF datasets in one
(while creating a parent-child relationship), printing of the CTF data
and computing statistics.

An ultimate demonstration of the capabilities of the implementation is a
feature addition to the FreeBSD kernel debugger DDB - pretty printing
for the data structures used in the currently loaded kernel image. A
vital point is the comparison to other approaches that would aim to
solve this problem.

Furthermore, the thesis should discuss and argue about future
possibilities of the technology, its use in compilers, system-wide
availability as debugging data even in production environments, the
potential use for core dumps examination or enrichment of the format by
adding the support for C++ classes.

### Literature
#### The C Programming Language
* Authors: Brian W. Kernighan, Dennis M. Ritchie
* Edition: 2nd
* ISBN-13: 007-6092003106

#### The Art of UNIX Programming
* Author: Eric S. Raymond
* Edition: 1st
* ISBN-13: 007-6092025368

#### The Design and Implementation of the FreeBSD Operating System
* Authors: Marshall K. McKusick, George V. Neville-Neil, Robert N. M. Watson  
* Edition: 2nd
* ISBN-13: 978-0321968975

#### Solaris Internals
* Authors: Richard McDougall, Jim Mauro
* Edition: 2nd
* ISBN-13: 978-0131482098

#### D-Trace: Dynamic Tracing in Oracle Solaris, Mac OS X and FreeBSD
* Authors: Brendan Gregg, Jim Mauro
* Edition: 1st
* ISBN-13: 978-0132091510

