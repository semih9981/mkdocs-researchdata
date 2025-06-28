# Project Insights

This file documents key findings, experiences, and outcomes from our genome data project.

---

## 1. What Was Tried

During the project, we experimented with various approaches and technologies to process and analyze genetic sequence data:

* Connection between Pywikibot and Wikibase to upload the dataset to the Wikibase API
* Automated connection to the Wikibase API for data integration using Wikibase-CLI and various bash scripts
* Development of custom preprocessing scripts in Python for sequence normalization and simplification
* Creation of SPARQL queries for targeted data extraction

---

## 2. What Was Used

The following tools and methods were used for the implementation of the project:

* Python libraries:

  * `pandas` for data manipulation

* Wikibase Cloud instance as the central knowledge base

* Bash Scripting to create custom upload scripts for the Wikibase-API

* SPARQL for complex data queries

* GitHub for version control and team coordination

* Regular meetings with supervisors for alignment and feedback

---

## 3. What Worked Well

* The preprocessing scripts reliably read and processed the sequences
* SPARQL queries provided accurate and targeted results for data analysis
* **Wikibase-cli** worked well for creating and editing entries via the shell, although uploading nearly 40,000 records took several hours

---

## 4. What Didn’t Work

* Difficulties with the automated connection between pywikibot and the Wikibase API caused delays and increased workload
* Storing complete RNA sequences in the knowledge base was not practical due to the data volume
* QuickStatements failed because commands were too long and caused the tool to freeze and in general just weren't as reliable as using bash scripts paired with wikibase-cli
* Creating Properties as basic Datatypes didnt work with the basic SPARQL Queries and therefore had to be changed to Wikibase-items
* Upload of all 40000 Items didnt work, due to multiple connection errors during the running code
* Sometimes claims for each Items werent set correctly, leading to an incosistency in the instance


---

## 5. Technical Challenges & Solutions

During the integration of data into Wikibase, several tools and approaches were tested:

* **Pywikibot** was initially used, but failed since it could not establish a connection to the Wikibase API.
* **QuickStatements** was also attempted, but the commands were too long for the tool and caused it to hang or crash.
* The final and successful solution was **Wikibase-cli**. This tool allowed for the creation and editing of entries directly via the shell. The only downside was that uploading nearly 40,000 entries required several hours and also failed in the end. Claims werent set correctly

