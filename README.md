pjawk
=====

An awk-like program to process JSON input using Perl syntax (thus, Perl+JSON+awk == pjawk).  This works best with input where each line is a single JSON string.  However, it can also be used with inputs where the entire input is a single JSON object with multiple lines (e.g. the JSON returned by most Amazon EC2 clients).

Like `awk`, the primary argument is a small program designating what to do with the input.  However, the syntax for this is Perl, with only a small number of helper macros (all of which are optional).  Most functionality is provided by predefined functions available to your programlet.

For full details, see command line help:

	pjawk --help
