# CSV_MS-SQL

Tool to convert CSV data files into MS SQL statements that
can be used to populate SQL tables. Each line of text in
the file is read, parsed and converted to SQL and output
to stdout (which can be piped).

A table to populate is given by the -t/--table option or
by the basename of the input file (if not standard input).

Fields are either given by the -f/--fields option (comma
separated) or determinted from the first row of data.

--------------------------------------------------------

Eventually I would like it to sanitize the data it reads 
from the CSV before writing the SQL inport statments.
For now a simpe find and replace all in your favorite 
spreadsheet editor does the trick.
