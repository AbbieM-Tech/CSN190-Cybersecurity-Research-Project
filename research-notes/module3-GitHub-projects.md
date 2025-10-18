Topic 1: Automated Vulnerability Assessment Tool Development
GitHub Project 1: OWASP. (2024). Nettacker - Automated Penetration Testing Framework
Citation: OWASP. (2024). Nettacker - Automated Penetration Testing Framework. GitHub. https://github.com/OWASP/Nettacker
Project Type: Security Tool / Automated Vulnerability Scanner
Synopsis: Nettacker is an OWASP project designed to automate network scanning and information gathering. It performs vulnerability assessments using multiple scanning modules (HTTP, FTP, SSH, etc.) and outputs structured reports (JSON/HTML). This project demonstrates practical
workflows and modular scanner design. Limitations: Command-line interface only; requires Python 3.7+, moderate configuration skills. Stats: ~3.7k stars | ~900 forks | active updates 2024
Link: https://github.com/OWASP/Nettacker
Relevance Rating: 5/5 - Directly demonstrates automated vulnerability assessment design and modular scanning logic

 GitHub Project 2: Project Discovery. (2024). Nuclei - Fast Vulnerability Scanner Based on Templates.
 Citation: ProjectDiscovery. (2024). Nuclei – Fast, customizable vulnerability scanner with YAML-based DSL. GitHub. https://github.com/projectdiscovery/nuclei 
Project Type: Security Tool (Vulnerability Scanner) 
Synopsis: Nuclei is a powerful, high-performance open-source scanner that uses a YAML-based templating language to enable custom vulnerability detection across applications, APIs, networks, DNS, cloud configurations, etc. It’s used widely in security operations for custom scanning, has 
large community support (stars/forks suggest significant adoption), and is designed for automation in CI/CD pipelines. Limitations: While extremely capable, it focuses on templated scanning rather than building from scratch an assessment engine; learning curve for creating custom templates.
Link: https://github.com/projectdiscovery/nuclei
Relevance Rating: 5/5 — Highly relevant: demonstrates automation of vulnerability assessment, template-based detection logic, integration with CI/CD — useful as reference or component in your tool development.

Comparison Notes -Automated Vulnerability Assessment Projects
* Automated Approach: Nettacker focuses on modular command-based scanning; Nuclei emphasises template-based extensibility.
* Usability: Nuclei offers smoother integration int CI/CD workflows; Nettacker requires more manual setup
* Community & Maintanence: Both are active; Nuclei has larger user base and ecosystem
* Value for Research: Nettacker highlights foundational design of scanning logic; Nuclei illustrates scaling and template reuse in automation
* Best Use Cases: Nettacker - teaching or prototyping scanning logic. Nuclei - production-level automation and vulnerability coverge

  Questions From Research
  1. How can multiple scanning frameworks (like Nettacker and Nuclei) be integrated to improve coverage and reduce false positives?
  2. What data models or formats are most effective for aggregation and comparing results from different scanners?
  3. How might AI or ML improve automated vulnerability detection accuracy or prioritisation?
 
 Topic 2: Secure Code Review - Common Vulnerabilties in Python Applications
Github Project 1: PyCQA. (2024). Bandit - Sucrity Linting Tool for Python.
 Citation: PyCQA. (2024). Bandit – Security static analyzer for Python code. GitHub. https://github.com/PyCQA/bandit 
Project Type: Security Tool (Static Code Analyzer for Python) 
Synopsis: Bandit analyses Python code by building an AST (abstract syntax tree) and running “plugins” to detect common security issues (e.g., unsafe uses of subprocess, insecure imports, etc.). It currently has ~ 7.4k stars, good community support, and supports integration with CI pipelines 
and containerized usage. Limitations: Focuses on certain classes of issues, may not cover complex logic vulnerabilities or framework-specific issues fully; possibly higher false-positive rate for some checks. 
Link: https://github.com/PyCQA/bandit 
Relevance Rating: 5/5 — Directly applicable to secure code review in Python; an excellent baseline tool to study and compare against.

GitHub Project 2: python-security. (2020). PyT - Static Analysis Tool for Detecting Security Vulnerabilities in Python Web Apps.
Citation: python-security. (2020). pyt – Static Analysis Tool for Detecting Security Vulnerabilities in Python Web Applications. GitHub. https://github.com/python-security/pyt 
Project Type: Security Tool / Static Analysis for Python (Research/Proof-of-Concept) 
Synopsis: ‘pyt’ is a static analysis tool designed for Python web applications. It uses control flow graphs, data flow analysis and fixed-point computations to detect issues such as command injection, SSRF, SQL injection, XSS and directory traversal. This is directly aligned with your topic of 
common vulnerabilities in Python code and code review. Limitations: The project appears older, may not be actively maintained, fewer stars/forks, and likely limited in coverage compared to more modern tools. 
Link: https://github.com/python-security/pyt 
Relevance Rating: 4/5 — Strong match for Python code review and vulnerability detection; some risk that the tool is outdated or less mature than alternatives.

Comparison Notes
* Purpose Overlap: Both perform static analysis but with different scopes - Bandit = production-ready linter #; PyT = research prototype exploring deeper code-flow logic.
* Detection Depth: Bandit uses rule-based AST scanning; PyT uses full data-flow analysis for more complex path tracing
* Maintenance & Community: Bandit = Active; PyT = arrchived/limited
* Educational Value: Bandit demonstrates practical integration into developer workflows; PyT shows underlying theory and algorithmic design
* Best Use Cases: Bandit - real-world secure review pipelines. PyT - academic or experimental research into static analysis.

Questions from Research
1. How can static and dynamic analysis tools complement each other in Python code reviews?
2. What approaches could minimise false positives in automated code scanners?
3. How can researchers maintain and update security rules set as Python libraries evolve?
