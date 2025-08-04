# Interview-Trainer-Agent

This repository contains sample code and deployment workflows for creating an AI-powered Interview Trainer Agent using IBM Cloud watsonx.ai Studio. The project leverages IBM’s cutting-edge generative AI, retrieval-augmented generation (RAG), and Agent Lab to deliver a robust, cloud-hosted assistant that helps users prepare for job interviews through realistic simulation, dynamic question generation, and personalized coaching.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [How to Use](#how-to-use)
- [Setup Instructions](#setup-instructions)
- [Repository Structure](#repository-structure)
- [Requirements](#requirements)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Project Overview

**Interview-Trainer-Agent** is a generative AI project developed in [IBM Cloud watsonx.ai Studio](https://www.ibm.com/products/watsonx-ai), featuring a conversational agent that mimics real interview scenarios, generates tailored question sets, provides coaching using industry best practices (e.g., STAR method), and offers actionable feedback for interview performance improvement.

The project includes Jupyter Notebooks that cover the full lifecycle: agent creation, local testing, deployment as an AI service in IBM Cloud, and API-based interactions.

---

## Key Features

- **Agent Lab Integration:** Easily configure and experiment with AI agents in the watsonx.ai Studio environment.
- **RAG-enabled Knowledge Base:** Uses vector search to ground answers in up-to-date, domain-specific information.
- **Dynamic Question Generation:** Produces technical, behavioral, and HR interview questions based on job role and experience level.
- **Coaching and Feedback:** Delivers structured feedback, model answers, and improvement tips using methods like STAR.
- **Multi-tool Support:** Integrates search tools (Google, DuckDuckGo, Wikipedia, WebCrawler) for extended context and relevancy.
- **Cloud-native Deployment:** Seamless promotion and deployment of AI services in IBM Cloud Spaces.
- **Safe & Compliant:** Avoids handling any personally identifiable information (PII) and includes phishing/scam warnings where relevant.

---

## Architecture

- **watsonx.ai Studio:** Collaborative environment for developing, testing, and deploying AI models and agents.
- **Agent Lab:** Drag-and-drop and code-based interface to configure conversational agents with modular tools and instructions.
- **LangChain + LangGraph:** For agent orchestration, conversation memory, and custom tool integration.
- **IBM Cloud Spaces & Deployments:** Hosts the deployed AI service for REST API access.

---

## How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/Sayantanpoddar/Interview-Trainer-Agent.git
cd Interview-Trainer-Agent
```

### 2. Open in IBM watsonx.ai Studio

- Go to [IBM Cloud watsonx.ai Studio](https://dataplatform.cloud.ibm.com/) and create a new project.
- Upload the notebook files (`.ipynb`) from this repository to your project.

### 3. Install Required Packages

Ensure your runtime environment includes:
- Python 3.11
- `ibm-watsonx-ai`
- `langchain_ibm`
- `langgraph`
- Any other dependencies specified in notebook cells.

### 4. Obtain IBM Cloud API Key

- [Create an API key](https://cloud.ibm.com/docs/account?topic=account-userapikey) via IBM Cloud dashboard.
- Paste your API key when prompted in the notebook.

### 5. Configure & Test Agent

- Use **`interview trainer agent code.ipynb`** to:
  - Authenticate with IBM Cloud.
  - Configure models, parameters, and tools.
  - Run local tests and simulate interview sessions.

### 6. Deploy Agent as a Service

- Use **`interview trainer deployment code.ipynb`** to:
  - Promote agent assets to a Cloud Space.
  - Deploy the agent as an online AI service.
  - Test deployment with sample API payloads.

### 7. REST API Usage

Once deployed, your agent can be accessed via REST API endpoints provided by IBM Cloud. See the output cells in `interview trainer deployment code.ipynb` for example payloads and usage patterns.

---

## Repository Structure

```
.
├── interview trainer agent code.ipynb         # Agent configuration, setup, and local test notebook
├── interview trainer deployment code.ipynb    # Deployment, promotion, and API test notebook
```

---

## Requirements

- IBM Cloud account with access to watsonx.ai Studio
- IBM Cloud API key (for authentication)
- Python 3.11 environment (Watson Studio runtimes are recommended)
- Required Python libraries (see notebooks for `pip install` instructions)

---

## License

Licensed Materials - Copyright © 2024 IBM.  
This repository and its source code are released under the terms of the [ILAN License](https://www14.software.ibm.com/cgi-bin/weblap/lap.pl?li_formnum=L-AMCU-BYC7LF).

For more details, refer to the License Terms provided in the notebooks.

---

## Acknowledgements

- Built with IBM watsonx.ai and Agent Lab
- Sample notebook headers and deployment workflows adapted from [IBM Watson Machine Learning Samples](https://github.com/IBM/watson-machine-learning-samples)
- For additional documentation, tutorials, and API references, visit the [official watsonx.ai documentation](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/agent-lab.html).

---

> **Note:** The notebook code was auto-generated using Agent Lab in watsonx.ai Studio. Modifying the notebook structure or cell order may affect execution. For reproducibility, follow the documented workflow in the provided order.
