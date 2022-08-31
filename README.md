# Curate.outbreak.info Data and results
This Repository contains de-identified data from curate.outbreak.info, a project in which citizen scientists thematically classified COVID-19 datasets collected primarily from Zenodo and Figshare during the first few months of the COVID-19 outbreak.

### About the data
Each user was instructed to classify datasets with up to 5 thematic categories and instructed to preferentially categorize with specific categories over broad categories whenever possible.

Each dataset was classified by at least 3 citizen scientists. For each dataset, a category needed to have been selected by at least 65% of the users to be considered valid for that category. Users were also asked to mark Datasets which could not be classified (ie- did not have sufficient information, were not in their language).

### Analyzing the results
To analyze the performance of citizen scientists, specific categories were mapped to the broader categories for comparison with predictions by an out-the-box algorithm that was trained on LitCovid-classified abstracts. Out of 530 dataset classifications which had reached the threshold needed (ie- 65% of users agreed on a category for this dataset), 344 of the datasets matched the predictions of the algorithm. 186 dataset classifications did not match the classification predicted by the algorithm and were manually inspected.

#### Manual evaluation of non-matches
Of the 186 dataset classifications that were manually inspected due to disagreement between predicted category and citizen science curated category:

* 46 were found to match both the curated and predicted categories (the categories are not necessarily mutually exclusive)
* 62 were found to better match the curated category due to limitations of LitCovid categories
* 54 were found to better match the algorithm than the curators
* 16 were found to match neither curator nor algorithm well
* 8 ignored (pdb datasets) due to the limited availability of metadata

Given the above findings, the number of expected true positives is estimated to be 452, false positives to be ~78

#### The Categories
The specific subcategories (left) are mapped to the broader category (right)
{"Clinical":"Clinical",
  "Case Descriptions":"Clinical",
  "Risk Factors":"Clinical",
  "Diagnosis":"Diagnosis",
  "Symptoms":"Diagnosis",
  "Rapid Diagnostics":"Diagnosis",
  "Antibody Detection":"Diagnosis",
  "Virus Detection":"Diagnosis",
  "Testing Prevalence":"Diagnosis",
  "Pathology/Radiology":"Diagnosis",
  "Forecasting":"Forecasting",
  "Mechanism":"Mechanism",
  "Virus Factors":"Mechanism",
  "Host Factors":"Mechanism",
  "Immunological Response":"Mechanism",
  "Mechanism of Infection":"Mechanism",
  "Mechanism of Transmission":"Mechanism",
  "Prevention":"Prevention",
  "Public Health Interventions":"Prevention",
  "Individual Prevention":"Prevention",
  "Transmission":"Transmission",
  "Host/Intermediate Reservoirs":"Transmission",
  "Viral Shedding / Persistence":"Transmission",
  "Treatment":"Treatment",
  "Vaccines":"Treatment",
  "Pharmaceutical Treatments":"Treatment",
  "Repurposing":"Treatment",
  "Biologics":"Treatment",
  "Medical Care":"Treatment",
  "Epidemiology":"Epidemiology",
  "Molecular epidemiology":"Epidemiology",
  "Classical epidemiology":"Epidemiology",
  "Behavioral Research":"Behavioral Research"}