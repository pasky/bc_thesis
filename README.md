Multiplatform CTF implementation and use in UNIX-like operating systems
-----------------------------------------------------------------------

Compact C Type Format (CTF) is a light-weight alternative to DWARF for
storing metadata on symbols and types in ELF binary files.  CTF has seen
some usage in UNIXes like Solaris and the BSDs, but the lack of a highly
permissive license, poor documentation and private unstable API prevent
it from a wider adaptation.

The goal of this thesis is to provide a 2-clause BSD licenced implementation of
the CTF in the form of a multi-platform C library
and properly document both the CRF and the corresponding new API.
The library should also be accompanied by some command-line tools such as
one-way conversion from DWARF to CTF, merging two CTF data sets in one,
printing of the CTF data, or computing statistics.

Besides the work on a core CTF library, the thesis should also show some
applications, with comparison to other possible approaches:

  * An extension to the FreeBSD kernel debugger DDB, pretty printing
    for the data structures used in the currently loaded kernel image.

  * Type-aware KVM Library that builds on top of the BSD standard
    kernel virtual memory library to provide a type-safe interface to read data
    from a live kernel or a core dump (possibly originating from a different
    processor architecture).

The thesis will also investigate and discuss at least one other
direction of extending the existing technology - e.g. its use in compilers, system-wide
availability as debugging data even in production environments or enrichment of
the format by adding support for C++ classes.

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

