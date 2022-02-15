# Configuration of a specification

## configuration guidelines

The `config` directory contains files describing specifications.
Each file can contains one or more configurations, it is therefore *always a json list*.

##  configuration 

```
{
  "name": "mijn-applicatieprofiel-ap",
  "type": "ap",
  "eap": "MijnApplicatieprofiel-AP.eap",
  "diagram": "MijnApplicatieprofiel",
  "template": "mijn-applicatieprofiel-ap.j2",
  "title": "Mijn Applicatieprofiel",
  "publication-state": "https://data.vlaanderen.be/id/concept/StandaardStatus/OntwerpStandaard",
  "publication-date": "2020-01-31",
  "license": "https://data.vlaanderen.be/id/licentie/modellicentie-gratis-hergebruik/v1.0",
  "contributors-file": "stakeholders.csv",
  "contributors-column": "MijnKolom",
  "site": "site-skeleton/mijn-applicatieprofiel-ap",
  "feedbackurl": "https://github.com/Informatievlaanderen/OSLOthema-mijnThema/issues",
  "standaardregisterurl": "https://data.vlaanderen.be/standaarden/TODO/CORRECT-URL/index.html"
}
```

- *name*: the name (identifier) of the configuration. The name is used as part of the URL on which the specification is published.
- *type*: the kind of specification. Possible values are `ap|oj|impl|voc`.
- *eap*: the filename of the EAP file located in the root of this repository.
- *diagram*: the name of the diagram identifying the specification in the EAP file.
- *template*: the template to use to generate the html representation of the specification.
- *title*:  the human readible title to be used in the html representation of the specification or other artificats.
- *publication-state* :  the status of publication, must be a concept from the Codelist [StandaardStatus](https://data.vlaanderen.be/id/conceptscheme/StandaardStatus).
- *publication-date*: the date in xsd:Date format when the specification is published. In the standardsregistry dates for different stages in the goverance process are recorded. This is the most recent data that corresponds to the governance process.
- *license*: the licence underwhich this specification is distributed
- *contributors-file*: the CSV file in the root of the repository containing the contributors for the specification. Per default, it is called stakeholders.csv
- *contributors-column*: the column which determines the contribution of a specification. This allows to group the participation in one file and exploit it in several specifications. Either one can decide to create for each specification a separate file.
- *feedbackurl*: the url of the location where one can provide feedback about the specification. Per default, it is the issue list from this repository.
- *standaardregisterurl*: the url referring back to the page where the governance of the specification is published. 

