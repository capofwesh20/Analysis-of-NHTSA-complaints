# Vehicle Complaints Analysis Project

![image](https://github.com/capofwesh20/Analysis-of-NHTSA-complaints/assets/35642413/abf30447-5823-474d-9806-cd2eac5636ec)


## Project Overview
This project focuses on analyzing vehicle complaints data to uncover patterns, associations, and topics within consumer reports. Utilizing advanced data processing techniques, associative rule mining, and topic modeling, we aim to identify common issues reported by vehicle owners, understand the broader themes in complaints, and potentially detect emerging trends in vehicle-related problems.

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Methodology](#methodology)
  - [Data Preprocessing](#data-preprocessing)
  - [Associative Rule Mining](#associative-rule-mining)
  - [Topic Modeling (On Going)](#topic-modeling-on-going)
- [Key Findings](#key-findings)
- [How to Use This Repository](#how-to-use-this-repository)
  - [Requirements](#requirements)
  - [Running the Analysis](#running-the-analysis)
- [Contributing](#contributing)

## Data Source
The dataset comprises vehicle complaints submitted over a period, including detailed narratives (`DESCRIPTION OF THE COMPLAINT`), specific components involved (`SPECIFIC COMPONENT'S DESCRIPTION`), vehicle models, and other related information from NHTSA and can be accessed at [NHTSA Datasets and APIs](https://www.nhtsa.gov/nhtsa-datasets-and-apis#investigations).

## Methodology

### Data Preprocessing
- Cleaned and preprocessed textual data from the `DESCRIPTION OF THE COMPLAINT` field.
- Aggregated noun phrases by vehicle model to prepare data for associative rule mining.

### Associative Rule Mining
- Applied the FP-growth algorithm to discover frequent itemsets and generate rules based on the occurrence of specific noun phrases.
- Experimented with different support thresholds to balance the discovery of meaningful patterns against the generation of too many uninformative rules.

### Topic Modeling (On Going)
- Despite having specific component descriptions, we employed topic modeling to:
  - Discover broader themes across complaints.
  - Identify misclassified or unlabeled data.
  - Detect emerging trends and issues not captured by specific component descriptions.

## Key Findings
- **Associative Rule Mining**: Identified significant associations between specific complaints and vehicle models, revealing common and recurring issues.
- **Topic Modeling**: Uncovered broader themes in complaints, such as issues related to safety, performance, and user experience, that transcend individual components.

## How to Use This Repository

### Requirements
- Python 3.8+
- Libraries: pandas, numpy, matplotlib, scikit-learn, gensim, mlxtend

### Running the Analysis
1. Clone the repository to your local machine.
2. Install the required Python libraries.
3. Run the Jupyter Notebooks provided to replicate the analysis or explore the dataset with your own queries.

## Contributing
Contributions to this project are welcome! Please submit issues or pull requests through GitHub, or contact the repository owner for more information.
