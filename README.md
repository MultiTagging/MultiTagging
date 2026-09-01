# MultiTagging
A vulnerable Ethereum smart contract labeling framework.
## Features
The MultiTagging framework provides several functions through the following components:
*  **Tagger:** It parses analysis tool reports to extract vulnerability tags and map them to the common vulnerability labels, i.e., SWC codes and DASP Ranks.
*  **Evaluator:** It measures the performance of the tool using different evaluation metrics.
*  **Elector:** It elects the sample label based on votes of a number of tools. It supports two Threshold-based vote methods (AtLeastOne and Majority) and one Power-based vote method.
*  **Plotter:** It plots the evaluation results in different formats.
## Supported Tools
* The components of the MultiTagging framework can be utilized for any analysis tool except for the Tagger.
* Currently Tagger supports 6 tools: <A Href="https://github.com/smartbugs/MAIAN">MAIAN</A>, <A Href="https://github.com/Consensys/mythril">Mythril</A>, <A Href="https://github.com/Decurity/semgrep-smart-contracts">Semgrep</A>, <A Href="https://github.com/crytic/slither">Slither</A>, <A Href="https://github.com/protofire/solhint">Solhint</A>, and <A Href="https://github.com/kupl/VeriSmart-public">VeriSmart</A>.
## Requirements
*  <A Href="https://www.python.org/">Python</A> >=3.11.7 (Recommended 3.12.2)
*  You can run MultiTagging framework using <A Href="https://jupyter.org/"> Jupyter Notebook</A> or from <A Href="https://support.apple.com/en-sa/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac">Terminal</A>.
## Usage
1.   Clone <A Href="https://github.com/MultiTagging/MultiTagging"> MultiTagging repository </A>
   ```
      git clone https://github.com/MultiTagging/MultiTagging.git
   ```
2.   Go to the MultiTagging home directory.
   ```
      cd MultiTagging
   ```
3.   Add your study's files in <A Href="https://github.com/MultiTagging/MultiTagging/tree/main/ToolReports">ToolReports</A>, <A Href="https://github.com/MultiTagging/MultiTagging/tree/main/ToolAnalysisTime">ToolAnalysisTime</A>, and <A Href="https://github.com/MultiTagging/MultiTagging/tree/main/BaseDS">BaseDS</A>. To retrieve study files from other folders, you can alternatively update the <A Href="https://github.com/MultiTagging/MultiTagging/blob/main/Scripts/config.json"> Scripts/config.json </A> file.
4.   Run the MultiTagging framework, there are three options:
      1. **Terminal Option:**
         1.   Run <A Href="https://github.com/MultiTagging/MultiTagging/blob/main/Main.py">Main.py</A> to open the wizard program. 
         ```
         python3 Main.py
         ```
         2.   Pass your choices and enter the requested input to get the output.
         ```
         MultiTagging Framework
         ..................................................
         
         Enter the number of the selected function:
          1: Get the labeled data for the tool reports.
          2: Get vote-based labeled data. 
          3: Get the evaluation report.
          4: Get the evaluation chart.
          5: Get tools overlap degree.
          6: Get tool efficiency scores 
          7: Exit
         ..................................................
         ```
         3.   Check the <A Href="https://github.com/MultiTagging/MultiTagging/tree/main/Results">Results</A> directory to get the saved output.
      2. **Jupyter Notebook:**
         * In a code cell, Run <A Href="https://github.com/MultiTagging/MultiTagging/blob/main/Main.py">Main.py</A> to open the wizard program. 
      ```
      run -i 'Main.py'
      ```
      3. **Within your Python code**
        *   You can call any function of the MultiTagging framework directly. Check the <A Href="https://github.com/MultiTagging/MultiTagging_Demo.git">MultiTagging Demo</A>
## Demo
*  The MultiTagging framework demo is available here: <A Href="https://github.com/MultiTagging/MultiTagging_Demo.git">MultiTagging Demo</A>

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
