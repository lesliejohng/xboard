Building winBoard with Visual Studio 2013/ Visual C++ 2013 resulted in a number of errors:-
Error	264	error C2054: expected '(' to follow 'inline'	c:\users\leslie\chess\xboard\parser.c	91	1	winboard
Error	265	error C2085: 'Match' : not in formal parameter list	c:\users\leslie\chess\xboard\parser.c	92	1	winboard
Error	266	error C2143: syntax error : missing ';' before '{'	c:\users\leslie\chess\xboard\parser.c	92	1	winboard
Error	267	error C2054: expected '(' to follow 'inline'	c:\users\leslie\chess\xboard\parser.c	103	1	winboard
Error	268	error C2085: 'Word' : not in formal parameter list	c:\users\leslie\chess\xboard\parser.c	104	1	winboard
Error	269	error C2143: syntax error : missing ';' before '{'	c:\users\leslie\chess\xboard\parser.c	104	1	winboard

The Branch LJGBuild was set up to correct these.
Visual C++ did not accept the inline command used for two functions in parser.c. These commands were commented out. Whether this was the correct solution will need to wait until testing of the program.
On subsequent builds further errors were identified as detailed in Git logs.
