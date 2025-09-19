# NCHHSTP-IO-MUST-Project
### MUST Busters Project

## 🌐 Overview
<img src="images/ghost_busters.png" alt="MUST Busters Logo" align="left" width="60" style="margin-right: 15px;" />

The MUST Busters project is a Python-based utility designed to scan and analyze network-based multi-user shared folders. It gives insights into data storage patterns across NCHHSTP shares. Helping the center understand **where** data resides, **how much** is stored (in **terabytes**), and **how old** it is. This tool was develop to support IT, Informatics and data governance teams in managing and planning network storage usage more effectively.
<br><br>

## 🧐 What is a Multi-User Share?

A **multi-user share** is a network folder accessible by a designated group of users. These are typically accessed via mapped drives or the **My Network Places** feature in Windows. This tool identifies and reports on these shares to assist with centralized storage management.
**MUST** (Multi-User Share Tool) is  multi-user share is a network-based file folder that can only be accessed by a designated group of users. Generally, these are accessed on your computer through the My Network Places icon. This tool is used to request new multi-user shares and to manage access to established multi-user shares.

## 🧭 Shared Drive Scanner Overview

- Performs recursive scans of one or more shared root directories
  - Collects and stores detailed metadata for:
  - Total storage used, measured in terabytes (TB)
  - File counts by directory and file type
  - File age statistics, including:
    - Oldest and newest file timestamps
    -Average last modified time
  - Storage usage breakdown by subdirectory, depth, and hierarchy
- All results are persisted in a normalized SQL database schema
  - Enables efficient querying, reporting, and integration with dashboards  
  - Supersedes prior CSV or JSON output formats, which are no longer practical at scale
  - Includes a logging system for traceability, diagnostics, and error auditing

## 🛠️ Getting Started

### Prerequisites

- Python 3.7 or higher
- Access to network shared drives (mapped or UNC paths)
- Read permissions for scanned directories

### Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-org/must-tool.git
cd must-tool
pip install -r requirements.txt
```

**⚖️ SHARE IT Act Information**

This repository is in compliance with the SHARE IT Act (Secure, Harmonized, and Accountable Resource Efficiency for Information Technology). This section can be updated according to the [CDC Metadata Implementation Guide](https://docs.cdc.gov/docs/ea/codeshare/implementation-guide#readmemd-override-optional-markers).

For More Information or access to the source code see below:
- Department: Health and Human Services (HHS)
- Agency: Centers for Disease Control and Prevention (CDC)
- Organization: National Center for HIV, Viral Hepatitis, STD, and Tuberculosis Prevention (NCHHSTP)
- Contact Name: NCHHSTP Informatics Office
- Contact Email: [adgapps@cdc.gov](mailto:adgapps@cdc.gov?subject=Share%20IT%20Act%20Inquiry:%20GitHub%20NCHHSTP-IO-MUST-Project)
- Version: 0.9.x
- Status: Active
- Keywords: MUST Busters, Multi-User Share Tool, Python, SQLLite, Excel, Informatics, IT 
- Contract#: NA
- Exemption: NA



## 📝 AI Contribution Notice 
- This project includes source code and documentation created with assistance from AI-based tools such as GitHub Copilot and other large language model (LLM) technologies. These tools were employed to accelerate development, support brainstorming, and enhance productivity.  

- All AI-assisted content has been reviewed by a human for accuracy and quality before inclusion. While care has been taken to verify the results, no warranty is expressed or implied. No confidential, proprietary, or personally identifiable information (PII) was provided to the AI tools. All interactions were restricted to generic, non-identifying questions and prompts.  


