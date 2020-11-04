# Thesis Guidance Committee Reports Template


<img src="https://github.com/mida-project/report_tgc_template/blob/main/assets/banner_1000x200.png?raw=true" width="100%" />

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://github.com/mida-project/report_tgc_template/blob/master/LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/mida-project/report_tgc_template?style=flat-square)](https://github.com/mida-project/report_tgc_template/commits/master)
[![HitCount](http://hits.dwyl.io/mida-project/report_tgc_template.svg)](http://hits.dwyl.io/mida-project/report_tgc_template)
[![OpenCollective](https://opencollective.com/oppr/backers/badge.svg?style=flat-square)](#backers)
[![OpenCollective](https://opencollective.com/oppr/sponsors/badge.svg?style=flat-square)](#sponsors)
[![Gitter](https://img.shields.io/gitter/room/gitterHQ/gitter.svg?style=flat-square)](https://gitter.im/opprTeam)
[![Twitter](https://flat.badgen.net/twitter/follow/opprGroup)](https://twitter.com/opprGroup)

This repository contains the template for a **Thesis Guidance Committee Reports** sample. The general template can be found on the [`src/`](src/) directory. A version of the template can also be found on the [Overleaf](https://www.overleaf.com/read/shkbwkxdpmgb) platform. We used the [LaTeX](https://www.latex-project.org/) format, a typesetting system that includes features designed for the production of technical and scientific documentation. [LaTeX](https://www.latex-project.org/) is available as [free software](https://www.latex-project.org/lppl/). For more detailed information regarding this repository please follow our [wiki](https://github.com/mida-project/report_tgc_template/wiki).

## Instructions

The [`report_tgc_template`](https://github.com/mida-project/report_tgc_template) repository can be used for the Thesis Guidance Committee Reports at [Instituto Superior Técnico](http://tecnico.ulisboa.pt/) (IST) of [PDEI](https://fenix.tecnico.ulisboa.pt/cursos/deic) (or other Doctoral Programs), as it follows the regulations published by the Scientific Council of IST. The all source of the template is available inside the `src/` folder, so please open it first. To start using, just open and modify your data as follows.

### Cover

In the `cover.tex` file insert your data (your full name, titles, supervisors names, date, degree, etc.):

	\title{}
	\subtitle{}
	\author{}
	\degree{}
	\supervisor{}
	\othersupervisor{}
	\date{}

### Chapters

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

### Bibliography

This file is the default bibliography database. If you are using [mendeley.com](mendeley.com) as Reference Manager, you can link the `.bib` file to your account in that swervice in order to keep the data automatically synchronized.

For those purposes, replace that file with your own file, and if the name is different, just modify the corresponding line in in the main document `document.tex` file:

```
\bibliography{bibliography/references}
```

## Table of contents

* [Prerequisites](#Prerequisites)
* [Usage](#Usage)
* [Roadmap](#Roadmap)
* [Contributing](#Contributing)
* [License & Copyright](#License--Copyright)
* [Team](#Team)
* [Acknowledgements](#Acknowledgements)

## Prerequisites

The following list is showing the required dependencies for this project to run locally:

* [Git](https://git-scm.com/) or any other Git or GitHub version control tool
* [LaTeX](https://www.latex-project.org/)

Here are some tutorials and documentation, if needed, to feel more comfortable about using and playing around with this repository:

* [Git Tutorial](https://git-scm.com/docs/gittutorial)
* [GitHub Quick Tutorial](https://guides.github.com/activities/hello-world/)
* [LaTeX Tutorial](https://www.latex-tutorial.com/)

## Usage

Usage follow the instructions here to setup the current repository and extract the present source. To understand how the hereby repository is used for, read the following steps.

### Installation

At this point, the only way to install this repository is manual. Eventually, this will be accessible through any package manager.

Nonetheless, this kind of installation is as simple as cloning this repository. Virtually all Git and GitHub version control tools are capable of doing that. Through the console, we can use the command below, but other ways are also fine.

```bash
git clone https://github.com/MIMBCD-UI/avi-2020-short-paper.git
```

Optionally, the module/directory can be installed into the designated Python interpreter by moving it into the site-packages directory at the respective Python directory.

### Demonstration

Please, feel free to try out our source. It is a script called `main.tex` at the `src/` directory. It can be used as follows:

```bash
latex src/main.tex
```

## Roadmap

[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/3819/badge)](https://bestpractices.coreinfrastructure.org/projects/3819)

We need to follow the repository goal, by addressing the thereby information. Therefore, it is of chief importance to scale this solution supported by the repository. The repository solution follows the best practices, achieving the [Core Infrastructure Initiative (CII)](https://bestpractices.coreinfrastructure.org/en/projects/3172) specifications.

Besides that, one of our goals involves creating a configuration file to automatically test and publish our code to pip or any other package manager. It will be most likely prepared for the [GitHub Actions](https://github.com/features/actions). Other goals may be written here in the future.

## Contributing

This project exists thanks to all the people who [contribute](CONTRIBUTING.md). We welcome everyone who wants to help us improve this downloader. As follows, we present some suggestions.

### Issuer

Either as something that seems missing or any need for support, just open a [new issue](https://github.com/mida-project/report_tgc_template/issues/new). Regardless of being a simple request or a fully-structured feature, we will do our best to understand them and, eventually, solve them.

### Developer

We like to develop, but we also like collaboration. You could ask us to add some features... Or you could want to do it yourself and fork this repository. Maybe even do some side-project of your own. If the latter ones, please let us share some insights about what we currently have.

## Information

The current information will summarize important items of this repository. In this section, we address all fundamental items that were crucial to the current information.

### Related Repositories

The following list, represents the set of related repositories for the presented one:

- [`repo-template-datasets`](https://github.com/MIMBCD-UI/repo-template-datasets)

- [`project-report-2-logo`](https://github.com/MIMBCD-UI/project-report-2-logo)

### License & Copyright

Copyright &copy; 2020 [Instituto Superior Técnico](http://tecnico.ulisboa.pt/)

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

The [`avi-2020-short-paper`](https://github.com/MIMBCD-UI/avi-2020-short-paper) repository is distributed under the terms of [MIT](LICENSE) license and [CC-BY-SA-4.0](COPYING) copyright. Permissions of this license are conditioned on making available complete elements from this repository of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved.

### Team

Our team brings everything together sharing ideas and the same purpose, developing even better work. In this section, we will nominate the full list of important people for this repository, as well as respective links.

#### Authors

* Francisco Maria Calisto [ [Website](http://www.franciscocalisto.me/) | [ResearchGate](https://www.researchgate.net/profile/Francisco_Maria_Calisto) | [GitHub](https://github.com/FMCalisto) | [Twitter](https://twitter.com/FMCalisto) | [LinkedIn](https://www.linkedin.com/in/fmcalisto/) ]

#### Promoters

* Nuno Nunes
* Jacinto Nascimento
* Hugo Lencastre
* Nádia Mourão
* Bruno Dias
* Bruno Oliveira
* Luís Ribeiro Gomes
* Carlos Santiago

#### Acknowledgements

Assistance provided by all intervenients is greatly appreciated. This work was partially supported by national funds through [FCT](http://fct.pt/) and [IST](http://tecnico.ulisboa.pt/) through the [UID/EEA/50009/2013](https://www.fct.pt/apoios/projectos/consulta/vglobal_projecto.phtml.en?idProjecto=147329&idElemConcurso=8999) project, [BL89/2017-IST-ID](http://ist-id.pt/en/) grant.

### Supporting

Our organization is a non-profit organization. However, we have many needs across our activity. From infrastructure to service needs, we need some time and contribution, as well as help, to support our team and projects.

<span>
  <a href="https://opencollective.com/oppr" target="_blank">
    <img src="https://opencollective.com/oppr/tiers/backer.svg" width="220">
  </a>
</span>

#### Contributors

This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].

#### Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/oppr#backer)]

<span>
  <a href="https://opencollective.com/oppr#backers" target="_blank">
    <img src="https://opencollective.com/oppr/backers.svg?width=890">
  </a>
</span>

#### Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/oppr#sponsor)]

<span>
  <a href="https://opencollective.com/oppr/sponsor/0/website" target="_blank">
    <img src="https://opencollective.com/oppr/sponsor/0/avatar.svg">
  </a>
</span>

<br />

<span>
  <a href="http://www.fct.pt/" title="FCT" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/fct_footer.png?raw=true" alt="fct" width="20%" />
  </a>
</span>
<span>
  <a href="https://www.fccn.pt/en/" title="FCCN" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/fccn_footer.png?raw=true" alt="fccn" width="20%" />
  </a>
</span>
<span>
  <a href="https://www.ulisboa.pt/en/" title="ULisboa" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/ulisboa_footer.png?raw=true" alt="ulisboa" width="20%" />
  </a>
</span>
<span>
  <a href="http://tecnico.ulisboa.pt/" title="IST" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/ist_footer.png?raw=true" alt="ist" width="20%" />
  </a>
</span>
<span>
  <a href="http://hff.min-saude.pt/" title="HFF" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/hff_footer.png?raw=true" alt="hff" width="20%" />
  </a>
</span>

##### Departments

<span>
  <a href="http://dei.tecnico.ulisboa.pt" title="DEI" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/dei_footer.png?raw=true" alt="dei" width="20%" />
  </a>
</span>
<span>
  <a href="http://deec.tecnico.ulisboa.pt" title="DEEC" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/deec_footer.png?raw=true" alt="dei" width="20%" />
  </a>
</span>

##### Laboratories

<span>
  <a href="http://sipg.isr.tecnico.ulisboa.pt/" title="SIPG" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/sipg_footer.png?raw=true" alt="sipg" width="20%" />
  </a>
</span>
<span>
  <a href="http://welcome.isr.tecnico.ulisboa.pt/" title="ISR" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/isr-lisboa_footer.png?raw=true" alt="isr" width="20%" />
  </a>
</span>
<span>
  <a href="http://larsys.pt/" title="LARSys" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/larsys_footer.png?raw=true" alt="larsys" width="20%" />
  </a>
</span>
<span>
  <a href="https://www.m-iti.org/" title="M-ITI" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/iti_footer.png?raw=true" alt="iti" width="20%" />
  </a>
</span>
<span>
  <a href="http://www.inesc-id.pt/" title="INESC-ID" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/inesc-id_footer.png?raw=true" alt="inesc-id" width="20%" />
  </a>
</span>

##### Domain

<span>
  <a href="https://europa.eu/" title="EU" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/eu_footer.png?raw=true" alt="eu" width="20%" />
  </a>
</span>
<span>
  <a href="https://www.portugal.gov.pt/" title="Portugal" target="_blank">
    <img src="https://github.com/mida-project/meta/blob/master/brands/pt_footer.png?raw=true" alt="pt" width="20%" />
  </a>
</span>
