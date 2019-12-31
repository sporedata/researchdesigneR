# researchdesigneR
Decision support for the design of patient-centered research

researchdesigneR provides decision support for data scientists having to choose a data science design and analytic strategy for patient-centered research projects. The software structure is pretty simple, with an operational classification of multiple data science methods connected to a system that allows for efficient searching. The latter is based on [fzf](https://github.com/junegunn/fzf), [rg](https://github.com/BurntSushi/ripgrep), [bat](https://github.com/sharkdp/bat), and [ag](https://github.com/ggreer/the_silver_searcher) to facilitate navigation. The classification hierarchy we use on the different methods is not comprehensive, authoritative, or even necessarily correct, i.e., intended to achieve a consensus among experts. The goal is pretty pedestrian: help data scientists choose an approach when faced with a research question. The classification is managed directly through the [wiki for this project](https://github.com/sporedata/researchdesigneR/wiki), meaning that if you are not happy about it you either create a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) or just [add or change the Wiki pages by hand](https://help.github.com/en/github/building-a-strong-community/adding-or-editing-wiki-pages).

We will soon be providing installation instructions, but for now check our [Wiki](https://github.com/sporedata/researchdesigneR/wiki), where we just started adding some content about individual methods and use cases.

<!--@todo 
# Cli demo
 --> 

# Installation instructions

Please install the following dependencies:

1. [R](https://www.r-project.org/), along with the [rmarkdown](https://cran.r-project.org/web/packages/rmarkdown/index.html) package.
2. [fzf](https://github.com/junegunn/fzf)
3. [ag](https://github.com/ggreer/the_silver_searcher)
4. [rg](https://github.com/BurntSushi/ripgrep)
5. [devicons](https://konpa.github.io/devicon/)
6. [bat](https://github.com/sharkdp/bat)
7. [Neovim](https://neovim.io/) - we do plan on releasing a version compatible with [Sublime Text](https://www.sublimetext.com/) later on.

The software is a minor modification from two previously posted snippets by [Dan Mikita](https://gist.github.com/danmikita/d855174385b3059cd6bc399ad799555e) <!-- https://gist.github.com/rpietro/3b618b645681229359a7f76b7f77addb --> and a file content search script posted in the [fzf examples page](https://github.com/junegunn/fzf/wiki/examples#searching-file-contents). <!-- https://gist.github.com/rpietro/c8ae12b048605a0ae120ea2a2a241c20 --> 

We have tested the software in [Manjaro](https://manjaro.org/), [Ubuntu](https://ubuntu.com/), and [Mint](https://linuxmint.com/), but if you encounter any difficulties please post an issue.

# Methods description: how we have structured it

Each data science method is described following the following structure: pre-requisites, mock conclusions, Methods, Results, suggested additional methods, and learning materials<!-- @todo add links -->. Of importance, each method is always described in the context of patient-centered use cases. For example, we know that a regression machine learning method is used to predict a numeric variable. One of its patient-centered use cases is then to predict a clinical score that is logistically challenging to obtain in the clinic, based on features (predicting variables) available from the electronic health record. An example would be to predict a frailty score from elderly patients attending a geriatric clinic. In this scenario, where patients don't have to undergo the full frailty evaluation as it is time consuming and slows down the clinic pace. Use cases are important since they are not "obvious" from the method, but are instead clever applications to patient-centered issues.


<!-- 
@todo
## Pre-requisites
variables already collected or to be collected
logistic - availability of electronic health record, or images, or a certain type of biomarker, or even access to a patient population where the data could be collected. other requirements are less tangible, such as the presence of equipoise to conduct a randomized trial
## Mock conclusions
alvin feinstein, 3 or 4, podium presentation at an important specialty conference, last slide
## Methods
equator network, reporting guidelines, sometimes enhanced if the guideline is felt to be missing important components
## Results
reporting guielines, open source packages 


## Suggested additional methods
in the context of a grant proposal. in other words, the other aims
future bpmn??


## Learning materials  
get list from other vimwiki

# References
--> 



