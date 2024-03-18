# Gemma-Model-Finetuning-Using-Lora
Fine tuning Domain Specific dataset (Personal Dataset) on Gemma 2B Model 

![gemma-img](https://github.com/AjayK47/Gemini-File/assets/88961945/40456066-4ad4-41d2-bd91-8771a6b51688)

#### This Model is Finetuned on a single P100 GPU , which is Freely available in Kaggle 

This repository contains the code and data for fine-tuning a small language model (SLM) for the specific domain of Indian history. The project demonstrates how to adapt a pre-trained language model to better understand and generate text relevant to this historical context.

### Requirements
- Kaggle/collab Account
- GPU access in Kaggle/collab
- Hugging Face API Key

### Project Overview

Large language models (LLMs) have shown remarkable capabilities in natural language processing tasks. However, fine-tuning them for specific domains remains crucial to unlock their full potential. This project explores the adaptation of the GEMMA model for analyzing Indian history, utilizing a dedicated Indian history dataset. We employ techniques like BitsAndBytes quantization and LoraConfig customization to optimize the model for causal language modeling tasks within this domain.

### Usage:
- clone the repository
```bash
   git clone https://github.com/AjayK47/Gemma-Model-Finetuning-Using-Lora.git
   ``` 
- Run the Jupyter Notebooks in the following order:
    - `dataset-preprocessing.ipynb`
    - `gemma-finetuned-model-inference.ipynb`
    - `gemma-it-finetuned.ipynb`
 
- You can Try Out My Hugging Face Model from here
      - https://huggingface.co/Ajayk/indian-history-gemma-instruction-finetuned

### Dependencies

Install the dependencies using the following command:
```
pip install -r requirements.txt
```

### Methodology
The project follows these key steps:

  - Data Preprocessing:
      Select and clean a specific Domain dataset.
      Format the data into the GEMMA model chat template.
  - Fine-tuning:
      - Use the SFTTrainer from the Hugging Face Transformers library.
      - Incorporate domain specific parameters for causal language modeling.
      - Optimize training parameters (e.g., learning rate, epochs).
      - Integrate Per-sample Feature Transform (Peft) for enhanced adaptability.
  - Evaluation and Deployment:
       - Evaluate the fine-tuned model on relevant tasks (e.g., text summarization, question answering).
       - Save and Push the model to Hugging Face.
   
### Future Work

- Potential future directions include:

     - Expanding the approach to other domains and languages.

     - Exploring alternative compact language models.

     - Developing techniques to understand the model's reasoning and decision-making processes.
 
### Contribution
- Contributions to this project are welcome!

### License

This project is licensed under the MIT License.




