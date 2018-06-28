# llncsconf

LaTeX package extending Springer's llncs class.

## Installation 

Copy `llncsconf.sty` in a directory that is searched by LaTeX
(e.g,. either your `texmf` tree or the local directory with your main
LaTeX file.

## Usage

In a LaTeX file that uses Springer's `llncs` class, just add
```tex
    \usepackage{llncsconf}
```
to use the style. The package supports the following options:
  * `crop`: crops the page (PDF) to the page size (152x235mm) used by
    the LNCS proceedings books (and the official PDFs offered by
    Springer). Please ensure that you *do not* have the option
    `a4paper` activated. Otherwise, cropping produces wrong results.
  * `rcsinfo`: adds RCS revision information to the first page of
    the document.
  * `svninfo`: adds subversion/svn revision information to the
    first page of the document.
  * `llncs`: typesets a copy of Springer's copyright note. This should
    satisfy Springer's requirements for self-archiving.
    You need to supply the DOI using `\llncsdoi{DOI}`.
  * `proceedings`: typesets a note in which proceedings the paper was
    published (similar to `llncs` without Springer's availability note).
  * `accepted`: adds a *accepted for publication at ...* note
    to the first page. This is useful for the phase where the camera
    ready version is prepared, but the publisher did not yet publish it.
  * `submitted`: adds a *submitted to ... please to no distribute* note
    to the first page.
  * `intended`: adds a *submitted to ... please to no distribute* note
    to the first page.

Moreover, the package requires two commands to be executed:
* `\conference{name of the conference}` which takes one argument,
  i.e., the name of the conference. This is used when one of the
  options `submitted` or `intended` is used for loading the package.
* `\llncs{book editors and title}{start page}` which takes two
  arguments: first the information about the book (e.g., editors,
  title) and, second, the start page of the chapter (contribution).
* `\llncsdoi{DOI}` which takes one argument,
  i.e., the DOI of the final publication available at Springer's web site.

## Self-Archiving

Sprinter states in his [Springer's Consent to Publish v3](http://resource-cms.springer.com/springer-cms/rest/v1/content/731196/data/v3):

> Author may only post his/her own version, provided acknowledgment is given 
> to the original source of publication and a link is inserted to the published
> article on Springer’s website. The link must be provided by inserting the DOI
> number of the article in the following sentence:
> "The final publication is available at Springer via 
> `http://dx.doi.org/[insert DOI]`".
The DOI (Digital Object Identifier) can be found at the bottom of the first page
of the published paper.

This package uses `https://doi.org` as `http://dx.doi.org` 
[is deprecated](https://www.doi.org/factsheets/DOIIdentifierSpecs.html).


## Authors

Main author: [Achim D. Brucker](http://www.brucker.ch/)

### Contributors

* [Oliver Kopp](https://github.com/koppor/)

## License

This project is dual-licensed under a 2-clause BSD-style license and/or 
the LPPL version 1.3c or (at your opinion) any later version. 

SPDX-License-Identifier: LPPL-1.3c+ OR BSD-2-Clause

## Master Repository

The master git repository for this project is hosted by the [Software
Assurance & Security Research Team](https://logicalhacking.com) at
<https://git.logicalhacking.com/adbrucker/llncsconf>.
