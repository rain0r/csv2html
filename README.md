csv2html
========

This software converts CSV table files into HTML tables using the old school `HTMLgen` Python 2.x module or the more modern `html` module found at https://pypi.python.org/pypi/html. By default it takes the first row the CSV file as the header of the HTML table. Note that for compatibility with LibreOffice Calc's current defaults csv2html uses `;` as the field delimiter unless you say otherwise; you may have to specify `-d ,` for files generated by Microsoft Excel and others.

Usage
-----
    usage: csv2html.py [-h] [-o output] [-t TITLE] [-d DELIM] [-s N] [-r] [-k]
                       input

    Converts CSV tables into HTML tables

    positional arguments:
      input                 input file

    optional arguments:
      -h, --help            show this help message and exit
      -o output, --output output
                            output file
      -t TITLE, --title TITLE
                            document & table title
      -d DELIM, --delimiter DELIM
                            field delimiter for CSV
      -s N, --start N       skip the first N-1 rows, start with row N
      -r, --renumber        replace the first column with row numbers
      -k, --skip-header     do not use the first row of the input as the header