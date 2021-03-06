# Data Lineage between Relational databases

## Introduction

I've built a system that creates an easy-to-understand visualization graph and a Lineage report of the data spreading across two isolated databases where the various transformations, replication and similarity on it can be tracked. 


# Install

## Requirements

Developed and tested on [Python 3.8](https://www.python.org/downloads/)

Also, although it is not strictly required, the usage of a [virtualenv](
https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
interfering with other software installed in the system.

# Quickstart

To run the webapp

First, clone this github repository in your system.
Install all dependencies from [requirements.txt](https://github.com/Aayushmittalwebpage/Data-lineage-between-databases-app/blob/main/requirements.txt)

Run [app.py](https://github.com/Aayushmittalwebpage/Data-lineage-between-databases-app/blob/main/app.py)

```bash
streamlit run app.py
```

Enter postgresql database credentials and submit to get results


*OR*

Simply use [Lineage-notebook.ipynb](https://github.com/Aayushmittalwebpage/Data-lineage-between-databases-app/blob/main/Lineage-notebook.ipynb) jupyter notebook


## Algorithm Flow

![image](https://drive.google.com/uc?export=view&id=1DhIixB8LDmZtqmfb6E_XBsLK2cnv5GXT)
  
  
## System Design

![image](https://drive.google.com/uc?export=view&id=1BeHf8hnWbG-vy3y6dWqclwVP4TOt-Lfl)


## Why build lineage using machine learning and statistics?
While many solutions to the data lineage problem have been proposed before, all available attempts at tackling the problem rely either on handcrafted heuristics , code analysis , and/or manual annotation of data. While these are all valid ways of lineage tracing, they all have limitations. Code analysis requires access to the code, which may be inaccessible when dealing with external applications or if the code was lost/deprecated. Algorithms require a strict set of conditions to be able to run, such as knowing ahead of time all the possible transformations, which cannot always be satisfied. Finally, solutions that require annotations are great for future lineage tracing, but they were not designed to answer the question of where the present non-annotated data came from. This approach does not have these same limitations.


