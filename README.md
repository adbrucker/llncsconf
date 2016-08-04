# llncsconf
LaTeX package extending Springer's llncs class.

## Installation 
Copy `llncsconf.sty` in a directory that is searched by LaTeX
(e.g,. either your `texmf` tree or the local directory with your main
LaTeX file.

## Usage
In a LaTeX file that uses Springer's `llncs` class, just add
```
    \usepackage{llncsconf}
```
to use the style. The package supports the following options:
  * `crop`: crops the page (PDF) to the page size (152x235mm) used by
    the LNCS proceedings books (and the official PDFs offered by
    Springer),
  * `rcsinfo`: adds RCS revision information to the first page of
    the document,
  * `svninfo`: adds subversion/svn revision information to the
    first page of the document,
  * `submitted`: adds a *submitted to ... please to no distribute* note
    to the first page.
  * `intended`: adds a *submitted to ... please to no distribute* note
    to the first page.
  * `llncs`: typesets a copy of Springer's copyright note. This should
    satisfy Springer's requirements for self-archiving. 
  * `proceedings`: typesets a note in which proceedings the paper was
    published (similar to `llncs` without Springer's copyright note).

Moreover, the package requires two commands to be executed:
* `\conference{name of the conference}` which takes one argument,
  i.e., the name of the conference. This is used when one of the
  options `submitted` or `intended` is used for loading the package.
* `\llncs{book editors and title}{start page}` which takes two
  arguments: first the information about the book (e.g., editors,
  title) and, second, the start page of the chapter (contribution).
  

## License
This project is dual-licensed under a 2-clause BSD-style license and/or 
the LPPL version 1 or any later version. 
