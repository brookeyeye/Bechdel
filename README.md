# Rethinking the Bechdel Test with NLP
This project utilizes sentiment analysis, readability scoring, topic modeling, and more language processing techniques to measure gender bias in film dialogue and to investigate whether the Bechdel Test is a valid indicator of good female representation.

The Bechdel Test was created by cartoonist Alison Bechdel in 1986 as a metric of gender bias in film. The criteria: if a film has 1. at least two female characters, 2. who talk to each other, 3. about something other than a man, the film has appropriate female representation. 

## Table of Contents
[Software and platform](#software-and-platform)

[Installation](#installation)

[Navigation](#how-to-navigate-this-repo)

[Features](#features)

[Contributing](#contributing)

[License](#license)

## Software and platform

This project was developed using Python 3.13.5 on MacOS and requires the following packages:
- pandas>=2.0.0
- numpy>=1.23.5
- matplotlib>=3.7.0
- seaborn>=0.12.0
- scipy>=1.10.0
- statsmodels>=0.14.0
- scikit-learn>=1.3.0
- ipykernel>=6.0.0
- notebook>=7.0.0
- spacy
- textstat
- sentence-transformers
- torch

## Installation

Create a new environment:
```bash
conda create -n bechdelEnv --file new_bechdel_env.txt python=3.9
conda activate bechdelEnv
```

Download this repository:
```bash
git clone https://github.com/brookeyeye/Bechdel
cd Bechdel
```

Install required packages: 
```bash
pip install -r new_bechdel_env.txt
```

Install SpaCY:
```bash
python -m spacy download en_core_web_sm
```

## How to navigate this repo

```text
Project/
├── The_Read_Me_File
├── Data/
│   ├── 1. InputData/
│   │   ├── Input_Data_Files
│   │   └── Metadata/
│   │       ├── Data_Sources_Guide
│   │       └── Codebooks
│   ├── 2. AnalysisData/
│   │   ├── Analysis_Data_Files
│   │   └── The_Data_Appendix
│   └── 3. IntermediateData/
├── Scripts/
│   ├── ProcessingScripts/
│   ├── DataAppendixScripts/
│   ├── AnalysisScripts/
│   └── The_Master_Script
└── Output/
    ├── DataAppendixOutput
    └── Results
```

For detailed description of input data, see Project/Data/1. InputData/Metadata

## Features

- Dataframe with 100,000+ lines of dialogue from 250+ films, tagged by gender of speaker
- Text scored for:
  - Sentiment analysis
  - Flesch-Kincaid readability
  - Syntactic role (dependency parsing)
  - Frequency of hedging words
  - Cosine similarity of male/female dialogue
  - Frequency of imperative sentences
- Statistical analysis:
  - Significance of the difference in above metrics for male/female dialogue
  - Correlation of Bechdel passing/failing with above metrics

## Contributing

Pull requests are welcome. ... 

## License

... 

