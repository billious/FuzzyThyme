_FuzzyThyme_ is a minimal perl library to enable grepping of timestamps that are within a margin close to those found on disk.

*Reason / Impetus*

Stock _grep_ and _fzf_ will assist finding timestamps if you're seeking one that shares a subset of characters, eg. if you have 
three  files with respectively containing the text 1:23:44, 1:23:39, and 1:23:42, you could find the first (:45) and last (:42) with _grep_ itself
using 'grep -r 1:23:4 .', but you wouldn't see 1:23:39, because the file with 39 seconds isn't textually a match.  FuzzyThyme
provides functions that enable bandpass matching/filtering centered around 1:23:40 
