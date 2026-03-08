# Parliamentary Inquiry Text Mining

## Context

Parliamentary inquiries in Australia are committee-led investigations that gather information, assess evidence, and report findings to parliament to support stronger legislation, public policy, and public awareness. A key feature is public participation: individuals and organizations can lodge submissions so their views are considered in policy development.

For this project, the dataset focuses on submissions to the inquiry into the conduct of the 2025 federal election. The full public submissions list (295 submissions) is published by the Australian Parliament at:

- [Inquiry submissions list (2025 federal election)](https://www.aph.gov.au/Parliamentary_Business/Committees/Joint/Electoral_Matters/2025federalelection/Submissions)

To simplify analysis, these submissions have been downloaded as PDFs and stored locally in `docs/`.

- **Primary data**: PDF submissions in `docs/`.
- **Metadata use**: Filenames include submission numbers and submitter indicators; use this metadata to enrich interpretation.
- **Analysis unit**: Each submission is treated as a document for NLP preprocessing and analysis.
- **Privacy note**: Some files are marked "Name withheld"; report findings at aggregate/theme level rather than personal level.
- **Legislation background**: Additional electoral legislation FAQs can be referenced via Australian Electoral Commission resources ([AEC website](https://www.aec.gov.au/)).

## Project Overview

This project uses Natural Language Processing (NLP) to analyze a large collection of public text submissions related to an electoral inquiry. The goal is to transform unstructured text into clear, evidence-based insights through code, visual analysis, and interpretation.

The project is designed as an end-to-end analytical report: from raw document ingestion to interpretable findings and recommendations. The main deliverable is a notebook-based report that combines documented code, charts, and plain-language interpretation.

## Purpose

- Explore and understand real-world public discourse through text data.
- Extract meaningful patterns, themes, and signals from submissions.
- Connect technical NLP analysis with clear narrative communication.
- Support informed understanding of the inquiry through interpretable findings.

## Objectives

- Load, clean, and organize the corpus of submission documents.
- Use metadata (such as filenames and submitter indicators) to enrich analysis context.
- Apply multiple text analysis techniques to explore language patterns and themes.
- Produce clear visualizations that support interpretation.
- Explain each method and result in plain language.
- Synthesize key findings into a concise, evidence-backed conclusion.

## Analysis Workflow

1. **Ingest** submission files and extract text.
2. **Clean and preprocess** text (normalization, tokenization, stopword handling, optional stemming/lemmatization).
3. **Explore** corpus characteristics (document lengths, frequent terms, lexical patterns).
4. **Apply methods** (for example: word frequency analysis, topic modeling, clustering, or regex-based pattern mining).
5. **Visualize and interpret** findings in clear, non-technical language.
6. **Conclude** with key insights, limitations, and recommendations.

## Repository Structure

- `docs/` - source submission PDFs.
- `Parliamentary_Inquiry_Text_Mining_Report.ipynb` - main report notebook.
- `README.md` - project overview and setup guidance.
- `.gitignore` - local environment and cache exclusions.

## Python Environment

Create and activate the local virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install required libraries (example starter set):

```bash
pip install jupyter pandas numpy matplotlib seaborn nltk scikit-learn
```

## Run the Report

Launch Jupyter and open the notebook:

```bash
jupyter notebook
```

Then open `Parliamentary_Inquiry_Text_Mining_Report.ipynb` and run cells from top to bottom.

## Expected Outputs

- A reproducible notebook with documented analysis steps.
- Visual summaries of language patterns and themes.
- An evidence-based narrative that answers the inquiry-focused research questions.
