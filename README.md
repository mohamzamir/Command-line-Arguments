# Command Line Arguments

## Project Overview

This project is a command-line tool that allows users to search for and replace text in a file. It provides several optional features, including the ability to limit the search and replace function to specific lines, as well as support for wildcard searching. The tool requires the input file and output file paths, along with the search and replace texts as arguments.

The syntax for running the tool is as follows:

```bash
 $ text_tool -s <search_text> -r <replace_text> [-w] [-l start_line,end_line] <input_file> <output_file>
 ```
 
 ## Arguments
 
**-s <search_text>:** The text to search for in the input file. This option is required.
**-r <replace_text>:** The text that will replace the search text in the output file. This option is required.
**-w:** Enable wildcard searching of words. This option is optional.
**-l <start_line,end_line>:** The range of lines of the input file to process. The range is inclusive. Lines outside this range are simply copied from the input file to the output file unmodified. If end_line is greater than the number of lines in the file, the tool will read to the end of the file. Note that line numbers start at 1, not 0. This option is optional.
**<input_file>:** Pathname of the input file. This argument is required.
**<output_file>:** Pathname of the output file. This argument is required.
