# Avado
File manipulation in SSIS

Have set codepage to 65001 for error output

Seems to be a conditional text qualifier - ", presumably for when the value contains a comma? Have used throughout

Set text column to 255 rather than default 50; basic MO is to load everything and evaluate once loaded

Using signed integers - course mappings has a -1, assume this is possibility for universities, too

Unix time: I have assumed UTC and added the value as seconds to 01-01-1970



What do you want to do if the email is invalid? I have just wiped it for now

Multiple University IDs for a given text value; I have arbitrarily selected the first

Excluding universities - are you excluding learners at that university too (presume yes)?

I presume Title is "mr, Mrs" etc but not supplied in the data, hVE USED EMPTY STRING


PROBLEMS:
TODO: convert to 24 hour clock
TODO: Check input files exists and are accessible. NB: Unix file systems show thE file before it's been fully written so check can get a file lock
TODO: Check output file doesn't exist
TODO: Improve error handling - more user-friendly, add run datetime
TODO: add event handlers for basic logging, error handling, and for when the package fails



