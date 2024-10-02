# SaaS Terms and Conditions Risk Analyzer

## Overview

The **SaaS Terms and Conditions Risk Analyzer** is a web-based tool that helps businesses and individuals analyze SaaS vendors' Terms and Conditions (T&Cs) to identify potential risks. The tool uses natural language processing (NLP) and keyword matching to scan legal contracts for critical clauses that may introduce legal, financial, or operational risks for the buyer. These risks are categorized into various sections such as data privacy, intellectual property, liability, termination, and more.

This tool aims to help users quickly identify and assess risks hidden within lengthy contracts, enabling them to make informed decisions before accepting T&Cs from SaaS providers.

## Features

1. **Multiple Input Formats**:
   - **PDF Upload**: Upload a PDF version of the terms and conditions to be analyzed.
   - **URL Input**: Provide a URL link to a webpage containing the terms and conditions.
   - **Text Input**: Directly paste the text of the terms and conditions for analysis.

2. **Risk Categories**:
   The tool identifies and categorizes risks into the following categories:
   - **Data Privacy Risk**
   - **Liability Risk**
   - **Termination Risk**
   - **Intellectual Property Risk**
   - **Payment or Financial Risk**
   - **Service Level Agreement (SLA) Risk**
   - **Governing Law and Jurisdiction Risk**
   - **Force Majeure Risk**
   - **Confidentiality Risk**
   - **Warranty Risk**
   - **Third-Party Obligations Risk**
   - **Compliance Risk**
   - **Indemnity Risk**
   - **Modification of Terms Risk**
   - **Auto-Renewal Risk**
   - **Usage Restrictions Risk**
   - **License Scope Risk**
   - **Age Restrictions Risk**
   - **Prohibited Users Risk**
   - **Geographic Restrictions Risk**

3. **Interactive UI**:
   - Use the sidebar to upload a PDF, enter a URL, or paste text.
   - Risks are displayed with expandable sections explaining the risk category and the causes behind the risk.
   - Highlighted matched text that triggered the risk detection.

4. **Keyword Matching with NLP**:
   - Utilizes **spaCy's PhraseMatcher** to detect predefined risk-related keywords and phrases.
   - Provides explanations for the identified risks and matches the exact phrases that triggered the risk.

5. **Performance Optimization**:
   - Fast and efficient text extraction from PDFs and web pages using `pypdf` and `BeautifulSoup` respectively.
   - Displays results with a user-friendly interface powered by **Streamlit**.

## Installation

### Prerequisites
- Python 3.7+
- The following Python libraries:
  - `spacy`
  - `streamlit`
  - `pypdf`
  - `requests`
  - `beautifulsoup4`
  - `time`

### Step-by-step Installation Guide

1. Clone the repository
2. pip install -r requirements.txt
3. python -m spacy download en_core_web_sm
4. streamlit run app.py

### Example Usage
1. Launch the application by running streamlit run app.py.
2. Choose an option from the sidebar:
   - PDF: Upload a PDF containing the SaaS Terms and Conditions.
   - URL: Enter the URL of a webpage with the SaaS Terms and Conditions.
   - Text: Paste the Terms and Conditions in the provided text area.
3. Click on the Analyze T&C button to start the analysis.
4. The tool will display the identified risk categories and causes along with the matched text for each risk.
