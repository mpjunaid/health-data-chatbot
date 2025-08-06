# FHIR Parser for RAG Applications

This project offers a Python library for transforming complex **FHIR-formatted JSON healthcare data** into a streamlined, LLM-friendly format. By converting FHIR resources into a simpler structure, this tool enables large language models (LLMs) to accurately understand and process patient information, making it ideal for building advanced **Retrieval-Augmented Generation (RAG)** systems.

---

## 🚀 Purpose & Performance

Working with raw FHIR data can be challenging for LLMs due to its verbose and nested nature. This library tackles that problem by preprocessing the data into an experimental, structured format that is easily digestible.

We've conducted extensive testing with various models and found that this parsing approach significantly boosts performance. Our benchmarks show a **100% QA accuracy** across all tested models—including **LLaMA 3.2 (1B and 8B)**, **Gamma**, and **Gemini**. Accuracy was measured using a binary output (1 for match, 0 for no match) against a set of manually evaluated true/false questions.

While Gemini showed an ability to work with raw FHIR data, the costs associated with direct processing make our parsing solution a much more efficient and cost-effective alternative.

---

## ✨ Key Features

- **Efficient Parsing:** Converts FHIR JSON into a simplified, tabular, and human-readable format.
- **LLM-Optimized Output:** The output format is specifically designed for seamless integration with LLM-powered RAG applications.
- **High Accuracy:** Achieves perfect QA accuracy across a range of LLM models.

The parser currently supports the following FHIR resource types:

- `Condition`
- `DiagnosticReport`
- `Encounter`
- `MedicalRequest`
- `Patient`

---


