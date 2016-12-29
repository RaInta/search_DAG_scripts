# search_DAG_scripts
Scripts to make end-to-end DAG for continuous gravitational wave searches

The overarching script is [set_up_search_DAG.sh](set_up_search_DAG.sh). 

This initializes a number of important variables and calls a host of other scripts (most of which unfortunately we don't have room for here).

This then creates a DAG (<a href="https://en.wikipedia.org/wiki/Directed_acyclic_graph">Directed Acyclic Graph</a>) within <a href="https://research.cs.wisc.edu/htcondor/">HTCondor's parallel control flow</a>.

The full pipeline is quite complicated (see the flowchart below). However, the DAG is set up so the entire pipeline is automated to the point of 'fire and forget'. Many of the steps in the pipeline require thousands, or even tens of thousands, of compute jobs at a time.

<img src="https://github.com/RaInta/search_DAG_scripts/blob/master/BOTR_flowchart20131212.jpg" width="600">
