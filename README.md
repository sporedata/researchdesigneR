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

## Pre-requisites

Pre-requisites include the types of variables you should have in order to conduct the analysis, be they already collected or about to be prospectively collected. They also include logistic requirements, for example the availability of electronic health record, images, a certain type of biomarker, or even access to a patient population where the data could be collected. Last, other requirements are less tangible, such as the presence of equipoise to conduct a randomized trial.


## Mock conclusions


Mock conclusions represent the most frequent structure for conclusions reached at the end of a typical analysis with that method. Although they are similar to a traditional research hypothesis, Alvin Feinstein believed that stating formally stating a conclusion would force researchers to think through exacly they might want to say at the end of their research project. Another way to think about mock conclusions is to assume that these will be the three or four main bullet points in a final slide called Conclusions when you are presenting your article at the top conference of your medical society. Of course, whether your mock conclusions match the final results is not relevant, the key concept is that you think through what you would ideally like to be able to say. 

## Methods

We list reporting guidelines to enhance the reproducility and overall quality of your article. Most of them are included in the [Equator Network](https://www.equator-network.org/), and many have been developed following at standard methodology.<!-- @todo include reference for methodology -->. In cases where a specific guideline does not exist, we might provide a collection of similar guidelines or a group of articles that might provide guidance.

## Results 

We provide a list of open source software packages in, most commonly, R, Python, or Julia languages. Many of these packages will have tutorials and code that is ready to run. 

## Suggested companion methods

This is a list of other methods that might be used in conjunction with the method being described. The rationale for this parallel use is explained.
<!-- 
@todo

## Learning materials  
get list from other vimwiki
extract the essence of each method with hooks to other methods - watercolor for blending

# References
--> 



