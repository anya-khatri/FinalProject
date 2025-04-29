# Backdoor Trigger-Based Attacks on Open-Source LLMs

This project investigates the vulnerability of open-source large language models (LLMs) to **trigger-based backdoor attacks**. It explores how different types of triggers — **lexical**, **pattern-based**, and **noisy** — affect model behavior during and after fine-tuning.

## Prerequisites

Make sure the following are installed:

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Git (for cloning repo)



1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>


## Running the Notebook in Google Colab (Step-by-Step)

- **Open the notebook**  
  - Navigate to the `.ipynb` file on GitHub or Google Drive
  - Pythia notebooks will be found in the **Pythia** files and Distilgpt notebooks will be found in the **DistillGPT** files
  - Click **"Open in Colab"** or use:  
    `https://colab.research.google.com/github/<your-repo>/<path-to-notebook>.ipynb`

- **Install dependencies**
- In the first code cell (or open a new one), install all necessary Python packages:
  
    `!pip install -r requirements.txt`

- **Set up the runtime**  
  - Go to `Runtime > Change runtime type`  
  - Select **GPU** as the hardware accelerator (recommended)  
  - Click **Save**

- **Run one cell at a time**  
  - Click the **play button** next to the first cell  
  - Wait for it to complete (a green check appears when done)  
  - Continue to the next cell and repeat the process

- **Run training**  
  - Execute the fine-tuning cells step-by-step  
  - Monitor for warnings or GPU memory issues (adjust batch size if needed)

- **Run evaluation cells**  
  - Test model responses with clean and triggered inputs  
  - Use `print()` or logging to observe and compare behavior

- **Download results**  
  - Save outputs to Drive or download locally using:
    ```python
    from google.colab import files
    files.download("your_output_file.txt")
    ```
