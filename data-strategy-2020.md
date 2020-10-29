# Data strategy for Akvaplan-niva

Authors:
  * [Conrad Helgeland](mailto:conrad.helgeland@akvaplan.niva.no)
  * [Anita Evenset](mailto:anita.evenset@akvaplan.niva.no)

Citation: Akvaplan-niva (2020). {Title}. {DOI}.

Modified: 2020-10-28

Status: draft

Version: v0.0.0-pre

License: https://creativecommons.org/publicdomain/zero/1.0/


## 1. Introduction

[Akvaplan-niva](https://akvaplan.niva.no)'s data must be published on the web to become easy to find, use, visualise, and trust.

Data consumers should get access to primary, standardised data via processable data streams, regardless of size and type of data.

Data should be published in a machine-actionable dataset catalog, built using linked data principles, ensuring data disoverability, data citeability, and also fully automated data retrieval.

The heart of this strategy is building reproducable data production pipelines using the best of breed open source software, based on a streaming architecture for handling large quantities of semi-structured and unstructured input data.

Once this strategy is implemented, Akvaplan-niva will have taken a significant step towards increased transparency, data traceability, and trustworthiness.


## 2. User perspectives
_Human users_ should be able to find Akvaplan-niva data using either a regular internet search, or through specialist data search platforms, eg. Google's [Dataset Search](https://datasetsearch.research.google.com/).

Once found, a human user should be able to access a landing page presenting each dataset. The landing page should reside on a permanent address on Akvaplan-niva's secure web space. This enables referring to and sharing of datasets via their web address.

Great care should be given in presenting the data and including all relevant information needed to access, cite, and use the data. Links should be provided for downloading data and for finding related information, including related datasets.

Data should be previewable, preferably via interactive visualisations and live code examples. For biological diversity data, [GBIF's landing pages may act as a paradigm](https://www.gbif.org/dataset/ead6339f-39f8-46be-b059-d1c48d88ab29).

To signal a commitment to the long-term stability and permanence of a published dataset, each dataset should be connected to a digital object identifier ([DOI](https://doi.org)).

_Machines_, or programmable agents, should be able to access Akvaplan-niva's data through a standardised data catalog, following [linked data](https://www.w3.org/DesignIssues/LinkedData.html) principles.

At the highest level, the programmable agent will get a list of available data catalogs, each representing a domain-specific data repository (a data storage service). Once inside a data catalog, the agent will receive a list of all datasets, and their data distributions. Consequently, it is trivial for the agent to obtain a complete representation of a dataset, or a replica of the entire repository. The agent simply follows links expressed in standardised data model (in eg. DCAT/[JSON-LD](https://json-ld.org/)) and issue a regular HTTP GET request for each of the linked resources.


## 3. Best practices
While Akvaplan-niva has an open [data policy](https://nmdc.no/resources/nmdc/Akvaplan-niva-dataforvaltningspolitikk.pdf), strategic action is needed to get data published. As [civic data activists](https://sunlightfoundation.com/policy/documents/ten-open-data-principles/) have pointed out, open data policies mean little if not primary, complete, and machine-readable data is freely available and downloadable in a timely manner.

### FAIR
The [FAIR](https://doi.org/10.1038/sdata.2016.18) principles are now widely used as guidelines for improving data quality, by requiring that data is findable, accessible, interoperable, and reusable.

Since 2017, [Norway's Research Council](https://www.forskningsradet.no/en/Adviser-research-policy/open-science/open-access-to-research-data/) requires that sponsered research data is managed in accordance with the FAIR principles.

### W3C
Both humans and machines need to access data via the web. Akvaplan-niva's data publishing should incorporate the guidelines and principles from [W3C](https://w3.org)s' on standardising the web platform, and in particular their recommendations: [Data on the Web Best Practices](https://www.w3.org/TR/dwbp/) and [Data Catalog Vocabulary (DCAT) - Version 2](https://www.w3.org/TR/vocab-dcat-2/).

### International expertise
Akvaplan-niva data management practices should continue to be sensitive to best practices and recommandations from experts working with scientific data management, in particular:
  * https://www.rd-alliance.org – and the [TRUST](https://www.nature.com/articles/s41597-020-0486-7) principles
  * https://theodi.org/
  * https://www.worlddatasystem.org/


### Norwegian authorities

Operating from Norway, Akvaplan-niva should also incorporate guidelines and strategies from Norwegian authorities:
  * https://www.regjeringen.no/en/dokumenter/national-strategy-on-access-to-and-sharing-of-research-data/id2582412/
  * https://www.regjeringen.no/no/dokumenter/retningslinjer-ved-tilgjengeliggjoring-av-offentlige-data/id2536870/


## Appendix

### The Research Council’s guidelines
1.0 Research data must be stored/archived in a safe and secure manner.
2.0 Research data must be made accessible for reuse.
3.0 Research data should be made accessible at an early stage.
4.0 Research data must be accompanied by standardised metadata.
5.0 Research data must be provided with a license for access, reuse and redistribution.
6.0 Research data should be made accessible at the lowest possible cost.
7.0 The management of research data must be described in a data management plan.
[Source]((https://www.forskningsradet.no/siteassets/publikasjoner/1254032622112.pdf)) 
