# NLX_LLM_Project_Conversational-AI
Fine-Tuned Conversational AI Job search chatbot using on Phi-3


In this project, we:
1. Preprocess the training data.
2. Load the Phi-3 Model and Fine=Tune the model
3. Use LoRA and QLoRA Fine-Tuning Techniques for comparative Analysis
4. Evaluate the models using various metrics like BLEU, METEOR, ROUGE Score and ARES.
5. Visualize the metrics and interpret the results and propose future directions.

## **Project Structure**

The project consists of the following files:

- **`code`**: Folder contains two subfolders containing the code for data preprocessing, model building, evaluation, and comparison of LoRA and QLoRA models.
- **`visualizations`**: Folder contains the visuals of the plots depicting the model comparison plots.
- **`report.pdf`**: A detailed report summarizing the project methodology, results, insights, and future work.
- **`README.md`**: This file, providing an overview of the project.

## **Running the Code**

You can run the code on **Google Colab** . Below are the steps:

### **Option 1: Running on Google Colab**

1. **Access Kaggle**:
   - Go to the [Colab website: (https://colab.research.google.com/)].
   - Sign in to your account (create an account if you don't have one).

2. **Create a New Colab Notebook**:
   - In your Colab account, create a new notebook by navigating to **Notebooks** and clicking **+ New Notebook** located on the bottom left.

3. **Upload the Dataset**:
   - Add the **training-1.csvs** to your Colab notebook:
     - Click on **Folder icon** on the left-hand side of the notebook.
     - Search for the dataset file and mount it.

4. **Upload the Notebook**:
   - Upload the implementation file into your Colab notebook.
   - Alternatively, you can copy and paste the code from **`NLX_QLoRA.ipynb`** into the cells of your Colab notebook.

5. **GPU Requirements**:
   - After setting up, On the top right corner you should be able to see "Connect" button, click the drop-down and click "View Resources". Then cllick on "Select runtime type" and change it to Python 3 and Hardware Accelerator as T4 GPU.
  
### **Key Sections of the Notebook**

- **Data Preprocessing**: 
  - Preprocesses the dataset by stemming, lemmatization and combining the job query and description pairs.
  
- **Model Building**:
  - Constructs and training of LoRA and QLoRA models on the preprocessed data . Beginning with Prompt Engineering of Instruction, Input and Output, followed by building the LoRA adapters and training the model.
  
- **Evaluation and Comparison**:
  - Evaluates the LoRA and QLoRA models using metrics like METEOR, RoUGE, BLEU.
