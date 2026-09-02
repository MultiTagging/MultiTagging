[![Paper](https://img.shields.io/badge/Paper-Electronics-blue)](https://doi.org/10.3390/electronics13234616)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19563271.svg)](https://doi.org/10.5281/zenodo.19563271)
[![GitHub release](https://img.shields.io/github/v/release/MultiTagging/MultiTagging)](https://github.com/MultiTagging/MultiTagging/releases)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](LICENSE.md)
[![GitHub Downloads](https://img.shields.io/github/downloads/MultiTagging/MultiTagging/total)](https://github.com/MultiTagging/MultiTagging/releases)
![Visitors](https://visitor-badge.laobi.icu/badge?page_id=MultiTagging.MultiTagging)
[![GitHub stars](https://img.shields.io/github/stars/MultiTagging/MultiTagging?style=social)](https://github.com/MultiTagging/MultiTagging/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/MultiTagging/MultiTagging?style=social)](https://github.com/MultiTagging/MultiTagging/network/members)

# 🏷️ MultiTagging
A vulnerable Ethereum smart contract labeling framework.

---

## ✨ Features
The MultiTagging framework provides several functions through the following components:
- **🏷️ Tagger:** Parses analysis tool reports to extract vulnerability tags and map them to common vulnerability labels, i.e., SWC codes and DASP Ranks.
- **📏 Evaluator:** Measures tool performance using different evaluation metrics.
- **🗳️ Elector:** Elects the sample label based on votes from a number of tools. It supports two threshold-based voting methods (`AtLeastOne` and `Majority`) and one power-based voting method.
- **📊 Plotter:** Plots evaluation results in different formats.
---

## 🛠️ Supported Tools
* The components of the MultiTagging framework can be utilized for any analysis tool except for the Tagger.
* Currently Tagger supports 6 tools: <A Href="https://github.com/smartbugs/MAIAN">MAIAN</A>, <A Href="https://github.com/Consensys/mythril">Mythril</A>, <A Href="https://github.com/Decurity/semgrep-smart-contracts">Semgrep</A>, <A Href="https://github.com/crytic/slither">Slither</A>, <A Href="https://github.com/protofire/solhint">Solhint</A>, and <A Href="https://github.com/kupl/VeriSmart-public">VeriSmart</A>.
---

## 📦 Requirements
- [Python](https://www.python.org/) >= **3.11.7**  
  Recommended version: **3.12.2**
- You can run the MultiTagging framework using:
  - [Jupyter Notebook](https://jupyter.org/)
  - [Terminal](https://support.apple.com/en-sa/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac)

---

## 🚀 Usage

### 1. 📥 Clone the Repository

Clone the [MultiTagging repository](https://github.com/MultiTagging/MultiTagging):

```bash
git clone https://github.com/MultiTagging/MultiTagging.git
```

### 2. 📂 Go to the MultiTagging Directory

```bash
cd MultiTagging
```

### 3. 🗂️ Add Your Study Files

Add your study files to the following directories:

- [ToolReports](https://github.com/MultiTagging/MultiTagging/tree/main/ToolReports)
- [ToolAnalysisTime](https://github.com/MultiTagging/MultiTagging/tree/main/ToolAnalysisTime)
- [BaseDS](https://github.com/MultiTagging/MultiTagging/tree/main/BaseDS)

To retrieve study files from other folders, update the [Scripts/config.json](https://github.com/MultiTagging/MultiTagging/blob/main/Scripts/config.json) file accordingly.

### 4. ▶️ Run the MultiTagging Framework

There are three options:

#### 💻 Option 1: Terminal

1. Run [Main.py](https://github.com/MultiTagging/MultiTagging/blob/main/Main.py) to open the wizard program:

```bash
python3 Main.py
```

2. Select the required function and enter the requested input:

```text
MultiTagging Framework
..................................................

Enter the number of the selected function:
 1: Get the labeled data for the tool reports.
 2: Get vote-based labeled data.
 3: Get the evaluation report.
 4: Get the evaluation chart.
 5: Get tools overlap degree.
 6: Get tool efficiency scores.
 7: Exit
..................................................
```

3. Check the [Results](https://github.com/MultiTagging/MultiTagging/tree/main/Results) directory for the generated output.

#### 📓 Option 2: Jupyter Notebook

In a code cell, run [Main.py](https://github.com/MultiTagging/MultiTagging/blob/main/Main.py):

```python
run -i 'Main.py'
```

#### 🐍 Option 3: Within Your Python Code

You can call MultiTagging framework functions directly from your Python code.

For examples, see the [MultiTagging Demo](https://github.com/MultiTagging/MultiTagging_Demo.git).

---

## 🎬 Demo

The MultiTagging framework demo is available here:

- [MultiTagging Demo](https://github.com/MultiTagging/MultiTagging_Demo.git)
---

## 📚 Publication

The MultiTagging framework is described in the following publication:

**Alsunaidi, S. J., Aljamaan, H., & Hammoudeh, M. (2024).**  
*MultiTagging: A Vulnerable Smart Contract Labeling and Evaluation Framework.*  
**Electronics, 13(23)**, 4616.  
https://doi.org/10.3390/electronics13234616

If you use the MultiTagging framework in your research, please cite:

```bibtex
@article{alsunaidi2024multitagging,
  title     = {MultiTagging: A Vulnerable Smart Contract Labeling and Evaluation Framework},
  author    = {Alsunaidi, Shikah J. and Aljamaan, Hamoud and Hammoudeh, Mohammad},
  journal   = {Electronics},
  volume    = {13},
  number    = {23},
  pages     = {4616},
  year      = {2024},
  publisher = {MDPI},
  doi       = {10.3390/electronics13234616},
  url       = {https://doi.org/10.3390/electronics13234616}
}
```

### 📦 Archived Resource

The MultiTagging framework is archived on Zenodo:

- **MultiTagging Framework:** [https://doi.org/10.5281/zenodo.19563271](https://doi.org/10.5281/zenodo.19563271)

---

## 📄 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](LICENSE.md).

You may share and adapt the material for non-commercial purposes, provided appropriate credit is given.

For more details, see the [LICENSE.md](LICENSE.md) file.
