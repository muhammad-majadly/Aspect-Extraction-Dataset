# Aspect Extraction Dataset for Scientific Papers

This dataset contains annotated scientific sentences for aspect extraction in research papers, focusing on peer review aspects. The sentences are labeled according to the following aspects: contribution, motivation, experimental claims, claims support, or none. The dataset comprises sentences from a collection of papers in the fields of Computer Science and Electrical Engineering.

## Table of Contents
- [Dataset Overview](#dataset-overview)
- [Data Structure](#data-structure)
- [Annotation Process](#annotation-process)
- [Aspects](#aspects)
- [Statistics](#statistics)
- [Citation](#citation)

## Dataset Overview
The dataset consists of sentences from **55 research papers** in total:
- **45 Computer Science papers** sourced from conferences like EACL, CONLL, and ICLR.
- **10 Electrical Engineering papers** sourced from *Electrical Engineering Journal* and *Natelectron*.

Each sentence is labeled according to its corresponding aspect, providing a structured way to understand the content of scientific papers.

## Data Structure
The dataset is organized as follows:

- **labeled_sentences.csv**: The file containing all labeled sentences in the dataset.
  - `sentence`: Text of the sentence.
  - `aspect`: The assigned aspect label (e.g., Contribution, Motivation, Experimental Claims, Claims Support, None).

### Aspect Categories
The aspect labels assigned to each sentence are as follows:
- **Contribution**: Describes the key contributions of the paper.
- **Motivation**: Highlights the motivation or rationale behind the work.
- **Experimental Claims**: Contains statements about experimental findings.
- **None**: Sentences not related to any specific aspect.

## Annotation Process
Two annotators with expertise in NLP and machine learning conducted the annotation. In cases of disagreement, the PhD student (first author) annotation was selected. The annotation process reached a high agreement level with a kappa statistic of **0.893**.

Annotators were given detailed instructions and examples for each aspect category. Specific assumptions guided aspect location:
- **Motivation** and **Experimental Claims** sentences are expected to appear mainly in the Abstract and Introduction sections.
- **Claims Support** sentences are typically found in the Results section.

## Statistics
The dataset contains **1,222 labeled sentences** in total.

## Citation

If you use this dataset in your research, please cite the following paper:

```bibtex
@article{majadly2024leveraging,
  title={Leveraging peer-review aspects for extractive and abstractive summarization of scientific articles},
  author={Majadly, Muhammad and Last, Mark},
  journal={International Journal of Data Science and Analytics},
  pages={1--14},
  year={2024},
  publisher={Springer}
}


