# reportiquē
### Automated Project Report Generation using LLM
## Overview
reportiquē is a program for creating reports that use Large Language Models (LLMs) to convert code into detailed reports. 
This project enables users to input code in PDF format, which is then processed to produce organized reports with important project information including tasks completed, Detailed Analysis, Recommended Solutions, and challenges. The software improves project reporting's efficiency and transparency.

---

## Working

- The PDF with code is sent to a Large Language Model (LLM) to extract meaningful insights from the code.
- The insights are filled into a structured report template.
- **Sections in Report template**: 
  - Name, ID, Role, Sub Role, Project Name, Date
  - Tasks Completed
  - Detailed Analysis
  - Recommended Solutions
  - Challenges (additional)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Nivey03/Reportique.git
   ```
2. create a new environment after navigating into the 'enterprise_knowledge_retriever' folder:
   ```bash
   python -m venv env
   ```
3. activate the environment using:
    ```bash
   .\env\Scripts\activate
   ```
> [!WARNING]
> Get your own SAMBANOVA_API_KEY [from SambaNova Cloud Webpage](https://cloud.sambanova.ai/) else
> begin by deploying your LLM of choice (e.g., Llama 3 8B) to an endpoint for inference in SambaStudio. Use either the GUI or CLI, as described in the [SambaStudio endpoint documentation](https://docs.sambanova.ai/sambastudio/latest/endpoints.html).
> To integrate your LLM deployed on SambaStudio with this AI starter kit, update the API information by configuring the environment variables in .env file.
4. **Setup API keys**: (for cloud users)
   ```
   SAMBANOVA_API_KEY = "your_sambanova_key"
   ```
5. **Install and update pip**:
   ```bash
    pip install -r requirements.txt
   ```
**Run the streamlit cmd:**
   ```bash
streamlit run streamlit/app.py --browser.gatherUsageStats false   

   ```
