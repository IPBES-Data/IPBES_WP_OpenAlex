---
title: OpenAlex as the Literature Database of Choice
subtitle: White Paper
date: today
author:
  - name: Rainer M Krug
    id: sb
    orcid: 0000-0002-7490-0066
    email: Rainer@krugs.de
    affiliation: 
      - name: University of Zurich
        city: Zürich  
        state: ZH
        url: www.uzh.ch
    roles: [author, editor]
abstract: > 
  The short abstract goes here 
  and can go over multiple lines. ...
# keywords:
#   - aaaaa
#   - bbbbb
license: "CC BY"
copyright: 
  holder: No idea
  year: 2023
citation: 
  type: report
  container-title: IPBES Technical Guidelines Series
  doi: xx.xxx/zenodo.xxxxxxxx
doi: xx.xxx/zenodo.xxxxxxxx
version: 0.0.1

format:
    html:
        toc: true
        toc-depth: 4
        toc_expand: true
        embed-resources: true
        code-fold: true
        code-summary: 'Show the code'
        keep-md: true
    pdf: default
---







**Reviewed by**:

- 

*For any inquires please contact [aidin.niamir\@senckenberg.de](mailto:aidin.niamir@senckenberg.de)* 


## Introduction
[OpenAlex](https://openalex.org) is a scholary data source as for example [Web of Science](https://www.webofscience.com/wos/) or [Scopus](https://www.scopus.com/).


## Advantges OpenAlex in comparison to other databases

The comparison needs to be done inseveral aspects which are:

- available works and number of OpenAccess works
- global coverage (i.e. Global South)
- openness of data and code used
- Web Access and API quality
- costs

We will go throuh these points in more detail now.

### Available Works and Number of OpenAccess works


|   | Number of works  | Open Access Works  |  Citations  |  Price  |  Data Openness  |  Org Structure  |
|---|---|---|---|---|---|---|
| OpenAlex  |  243M  |  48M  |  1.9B  |  Freemium  |  Fully open, CC0 license  |  Non-profit |
| Scopus  |  87M  |  20.5M (ref)  |  1.8B  |  Subscription  |  Closed  |  For Profit |
| Web of Science (core)  |  87M (ref)  |  12M (ref)  |  1.8B  |  Subscription  |  Closed  |  For Profit |
| Dimensions  |  135M  |  29M (ref)  |  1.7B  |  Freemium  |  Partly open, personal use  |  For Profit |
| Google Scholar  |  389M (estimated)  |  ?  |  ?  |  Free  |  Closed  |  For Profit |
| Crossref  |  145M  |  20M  |  1.45B  |  Free  |  Fully open, CC0 license  |  Non-profit |

(From: [OpenAlex](https://openalex.org))


### Global Coverage (i.e. Global South)

OpenAlex has a broad coverage for articles and authors from the Global South, which is not the case for other databases [REF???](REF???).

![From: [OpenAlex](https://openalex.org/stats)](./figures/OpenAlex Current Stats 06 Nov 2023.png)

### Openness of Data and Code used

OpenAlex is free and open, i.e. it is free to use for everybody
without any subscription or registration, by design. The data is freely available (database dumps are possible and easy to do) and the code used is also openly available.

### Web Access and API quality

OpenAlex has, as the other scholary data sources, a [web interface](https://openalex.org/works).  It is still in beta phase, so elements can change and aspects will improve over time, 
but it is already very usable and based on personal preferences easier to use than WoS or Scopus.

API access is important for accessing the database programmatically. An example is a search for all articles covering a specific topic. Usually, this is an iterative provess which needs refinement 
of the search terms. THe traditional way is to type the search term in the search box and at east writew down the number of hits, change the search term and repeat the process. especially when other 
comparisons should also be done (e.g. assessment of cerrtain key-papers are in the search results). This is a very tedious process and can be automated using the API. In this case, the search is 
defined e.g. in R or any other programming language and the search is done automatically. The results are then analysed and the search terms are refined and the search is repeated, and the results 
can be shown in a clear, concise and reproducible report.

In contrast to the APIs assessed, (WoS, Scopus), the [OpenAlex API(https://docs.openalex.org)] is relatively simple but provides all the neccessary functionality needed for IPBES and for all 
other tasks. 

To simplify the API usage even more, the excellent R package [openalexR](https://docs.ropensci.org/openalexR/articles/A_Brief_Introduction_to_openalexR.html) is available to access the API from [R](https://www.r-project.org/).

### Costs

OpenAlex is free to use, which is not the case for most other databases. If the limit for free usage (100k API calls per day with a maximum of 10 per second) is not enaough, 
a Premium subscription is offered. The pricing is determined on a case by case basis.

For the use cases of IPBES, the free tier is more than enough, especially as the API restrictions are email based and multiple users can use their own email adresses..

The API is, as is the access through the website, free for OpenAlex.

In contraast, the API costs for WoS are getting into the several thousands per dollars per year. In addition to the costs,


## Conclusion

@article{Michael2023,
  title = {A Systematic Evidence Map of Intervention Evaluations to Reduce Gang-Related Violence},
  author = {Michael, Richardson and Mark, Newman and Gregory, K. Berry and Claire, Stansfield and April, Coombe and James, Hodgkinson},
  year = {2023},
  month = jun,
  journal = {Journal of Experimental Criminology},
  pages = {undefined},
  publisher = {{Springer Science+Business Media}},
  issn = {1572-8315, 1572-8315},
  doi = {10.1007/s11292-023-09574-w},
  langid = {english},
  keywords = {/unread},
  file = {/Users/rainerkrug/Library/Mobile Documents/com~apple~CloudDocs/Zotero Attachments/2023/Michael2023__Michael et al_2023_A systematic evidence map of intervention evaluations to reduce gang-related.pdf}
}
