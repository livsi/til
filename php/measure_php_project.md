# CLI tools for quick size measure of PHP project

Old-days famous tool - [phploc](https://github.com/sebastianbergmann/phploc) package to measure project size was archived by Sebastian on Jan 10, 2023.

New tool from author of Rector - [Tomas Votruba](https://github.com/TomasVotruba) - [lines](https://github.com/TomasVotruba/lines). Installed with composer, has json and text output

```
  Filesystem                                         count
  Directories ......................................... 32
  Files .............................................. 160

  Lines of code                           count / relative
  Code ................................... 15 521 / 70.9 %
  Comments ................................ 6 372 / 29.1 %
  Total .................................. 21 893 /  100 %

  Structure                                          count
  Namespaces .......................................... 32
  Classes ............................................ 134
   * Constants ........................................ 91
   * Methods ....................................... 1 114
  Interfaces .......................................... 20
  Traits ............................................... 4
  Enums ................................................ 1
  Functions ........................................... 36
  Global constants ..................................... 0

  Methods                                 count / relative
  Non-static .............................. 1 058 /   95 %
  Static ..................................... 56 /    5 %

  Public .................................... 875 / 78.5 %
  Protected .................................. 90 /  8.1 %
  Private ................................... 149 / 13.4 %
```