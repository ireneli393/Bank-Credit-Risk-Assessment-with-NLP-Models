# Advanced-Name-Screening-and-Entity-Linking-with-Existing-NLP-Models


**Project Overview:**

In collaboration with Solytics Partners, we developed a machine learning system for **assessing credit risk in banking** by identifying high-risk individuals through the extraction and matching of names from negative news reports against a database.

**Approach and Methods:**

- **Name Entity Recognition (NER):** We implemented six distinct pre-trained models for NER: spaCy Large, spaCy Transformer, BERT-Large, BERT-CRF, XLM-RoBERTa, and XLNet-Base. The flow chart provided in the documentation offers a high-level overview of their structural nuances.
  
- **Name Matching:** We tested various name-matching techniques, including TF-IDF Similarity and Fuzzy Name Matching, with the Naive TF-IDF method proving most effective, especially when scaled to larger datasets.

**Key Findings:**

- **NER Models:** There was a trade-off between F1 score and inference time across the models. While the spaCy-transformer model achieved the highest F1 score, its slower inference time made it less suitable for high-volume processing. BERT-CRF and XLM-RoBERTa provided the best balance of accuracy and efficiency, aligning well with project requirements.

- **Name Matching:** We observed a similar trade-off between efficiency and accuracy. For larger datasets, the Naive TF-IDF and Clustered models had similar inference times (~420 seconds), with the Phonetic method being faster (~340 seconds). All models are ready for production, with the choice depending on specific business needs.

**Conclusion:**

This project successfully applied AI to credit risk assessment, demonstrating the utility of large language models and the effectiveness of the implemented NER models. The developed system is robust and ready for deployment, offering a strong solution for banking risk management.


Due to confidentiality, only part of the codes are added to this repository for reference.
