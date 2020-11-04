# Thesis Guidance Committee Reports Template


<img src="https://github.com/mida-project/report_tgc_template/blob/main/assets/banner_1000x200.png?raw=true" width="100%" />

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://github.com/mida-project/report_tgc_template/blob/master/LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/mida-project/report_tgc_template?style=flat-square)](https://github.com/mida-project/report_tgc_template/commits/master)
[![HitCount](http://hits.dwyl.io/mida-project/report_tgc_template.svg)](http://hits.dwyl.io/mida-project/report_tgc_template)
[![OpenCollective](https://opencollective.com/oppr/backers/badge.svg?style=flat-square)](#backers)
[![OpenCollective](https://opencollective.com/oppr/sponsors/badge.svg?style=flat-square)](#sponsors)
[![Gitter](https://img.shields.io/gitter/room/gitterHQ/gitter.svg?style=flat-square)](https://gitter.im/opprTeam)
[![Twitter](https://flat.badgen.net/twitter/follow/opprGroup)](https://twitter.com/opprGroup)


# Instructions

The [`report_tgc_template`](https://github.com/mida-project/report_tgc_template) repository can be used for the Thesis Guidance Committee Reports at [Instituto Superior Técnico](http://tecnico.ulisboa.pt/) (IST) of [PDEI](https://fenix.tecnico.ulisboa.pt/cursos/deic) (or other Doctoral Programs), as it follows the regulations published by the Scientific Council of IST. The all source of the template is available inside the `src/` folder, so please open it first. To start using, just open and modify your data as follows.

## Cover

In the `cover.tex` file insert your data (your full name, titles, supervisors names, date, degree, etc.):

	\title{}
	\subtitle{}
	\author{}
	\degree{}
	\supervisor{}
	\othersupervisor{}
	\date{}

## Chapters

The content of your report will be written in the files of the `chapters/` folder. Do not modify the `header` in all those documents, except the name of the document as it contains compilation directives. If you need to add more **Chapters**, just create new `.tex` file and add the header.

If you do not need that many **Chapters** in your report, just comment the lines in the main document:

```
document.tex
```

For example, if you do not need a *6th* **Chapter**, comment the following lines:

```
%Chapter 6
\input{chapters/chap006.tex}
% If Printing on DOUBLE SIDED pages, the second page should be white.
% Otherwise, comment the following command:
\cleardoublepage
```

## Bibliography

This file is the default bibliography database. If you are using [mendeley.com](mendeley.com) as Reference Manager, you can link the `.bib` file to your account in that swervice in order to keep the data automatically synchronized.

For those purposes, replace that file with your own file, and if the name is different, just modify the corresponding line in in the main document `document.tex` file:

```
\bibliography{bibliography/references}
```