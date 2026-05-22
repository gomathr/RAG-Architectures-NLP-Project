# Retrieval-Augmented Generation (RAG) Architectures for Large Language Models

**NLP / Retrieval-Augmented Generation Research Project**

**Repository:** RAG-Architectures-NLP-Project
**Author:** Gomathi Ramesh
**University:** Rice University
**Program:** Master’s in Data Science
**Project Type:** NLP / Retrieval-Augmented Generation / Large Language Model Research
**Course Project:** Research-Oriented Investigation of Baseline, Enhanced, and Agentic RAG Architectures


## Development and Evaluation of Baseline, Enhanced, and Hierarchical Agentic Retrieval-Augmented Generation (RAG) Architectures for Improving Large Language Models

## Project Overview

This project explores Retrieval-Augmented Generation (RAG) to improve the performance of large language models by incorporating external knowledge retrieval and reducing hallucinated responses.

The project experimentally investigates and evaluates multiple RAG architectures, including Baseline RAG, Enhanced RAG (LightRAG-style), and Agentic RAG with hierarchical retrieval, using the HotpotQA dataset with pretrained and fine-tuned Qwen models.

The study focuses on improving answer quality, faithfulness, and multi-hop reasoning capabilities through retrieval-augmented large language models, parameter-efficient fine-tuning (LoRA), and comparative evaluation using EM, F1, BERTScore, and RAGAS metrics.

## Dataset

- HotpotQA dataset is used for training, validation, and testing

## Tools and Libraries

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- BGE-M3 Embeddings
- FAISS
- Qwen / Qwen2.5 Models
- LoRA / PEFT
- NumPy
- Pandas
- scikit-learn
- Matplotlib
- Seaborn
- RAGAS
- BERTScore
- Google Colab GPU environment


## My Contributions

### A) Dataset and Model Selection

* Contributed to dataset selection, preparation, and preprocessing using the HotpotQA dataset
* Selected and configured pretrained components for all RAG architectures, including the encoder (BGE-M3), vector database (FAISS), and generator (Qwen)

### B) System Design

* Designed and implemented the Baseline RAG architecture using pretrained models

### C) Fine-Tuning of the Generator (Qwen)

* Developed the fine-tuning strategy using Supervised Fine-Tuning (SFT) with LoRA
* Designed comparative experiments between pretrained and fine-tuned models using EM and F1 metrics, demonstrating measurable performance improvements

### D) Hyperparameter Tuning (Validation Set)

* Developed helper functions for hyperparameter tuning across multiple configurations, including top-k retrieval, temperature, and maximum token settings
* Analyzed validation performance and selected optimal configurations for final evaluation

### E) Visualization and Experimental Analysis

* Developed helper functions for comparative visualization of pretrained and fine-tuned model performance using bar charts and evaluation plots
* Created visualizations for hyperparameter tuning experiments and applied optimal configurations to the final test set

### F) Evaluation Methods

* Conducted comprehensive evaluation using EM, F1, BERTScore, and RAGAS metrics

### G) Key Findings

* Fine-tuning the Qwen generator using SFT with LoRA improved retrieval-augmented question answering performance compared with the pretrained baseline model
* Enhanced and Agentic RAG architectures demonstrated stronger multi-hop reasoning and contextual retrieval capabilities compared with the Baseline RAG system
* Comparative evaluation using EM, F1, BERTScore, and RAGAS metrics showed improvements in answer quality, faithfulness, and retrieval effectiveness after fine-tuning
* Experimental analysis highlighted the importance of retrieval strategies and parameter-efficient fine-tuning for improving large language model performance in multi-document question answering tasks

### H) Additional Contributions to the Team

* Created the fine-tuned model artifact (`qwen_hotpotqa_lora_final.zip`) and provided it for integration into Enhanced and Agentic RAG architectures
* Shared helper-function designs for hyperparameter tuning, evaluation (EM/F1), and visualization workflows
* Led documentation organization and report structuring for the project


## Project Structure

- `HotpotQA_BaselineRAG.ipynb`  
  - Implementation of Baseline RAG using pretrained Qwen models and fine-tuned Qwen LoRA adapters  

- `HotpotQA_BaselineRAG_FineTune.ipynb`  
  - Supervised Fine-Tuning (SFT) with LoRA on the Qwen generator model, including hyperparameter experimentation and performance comparison between pretrained and fine-tuned models  

- `HotpotQA_Enhanced_RAG.ipynb`  
  - Enhanced RAG (LightRAG-style) implementation with improved retrieval integration using the fine-tuned Qwen model  

- `Final_Project_Evaluation_Methods.ipynb`  
  - Evaluation pipeline for EM, F1, BERTScore, and RAGAS metrics, including comparative visualization and performance analysis across Baseline, Enhanced, and Agentic RAG architectures  

- `predictions_baseline.jsonl`  
  - Prediction outputs generated from the Baseline RAG architecture  

- `predictions_enhanced.jsonl`  
  - Prediction outputs generated from the Enhanced RAG architecture  

- `predictions_agentic.jsonl`  
  - Prediction outputs generated from the Agentic RAG architecture  

- `predictions_baseline_scored.jsonl`  
  - Evaluation-scored outputs for Baseline RAG predictions  

- `predictions_enhanced_scored.jsonl`  
  - Evaluation-scored outputs for Enhanced RAG predictions  

- `predictions_agentic_scored.jsonl`  
  - Evaluation-scored outputs for Agentic RAG predictions  

- `qwen_hotpotqa_lora_final.zip`  
  - Fine-tuned Qwen LoRA adapters used across the RAG architectures  

- `rag_evaluation_results.pdf`  
  - Comparative evaluation visualizations and overall performance analysis reports  

- `rag_evaluation_heatmap.pdf`  
  - Heatmap-based visualization and ranking analysis across evaluation metrics  

- `README.md`  
  - Project overview, contributions, methodology summary, and repository documentation
 
```text
├── README.md
├── notebooks/
│   ├── HotpotQA_BaselineRAG.ipynb
│   ├── HotpotQA_BaselineRAG_FineTune.ipynb
│   ├── HotpotQA_Enhanced_RAG.ipynb
│   └── Final_Project_Evaluation_Methods.ipynb
├── outputs/
│   ├── predictions_baseline.jsonl
│   ├── predictions_enhanced.jsonl
│   ├── predictions_agentic.jsonl
│   ├── predictions_baseline_scored.jsonl
│   ├── predictions_enhanced_scored.jsonl
│   └── predictions_agentic_scored.jsonl
├── models/
│   └── qwen_hotpotqa_lora_final.zip
├── docs/
│   ├── rag_evaluation_results.pdf
│   └── rag_evaluation_heatmap.pdf
```

  
## Repository Note

This repository focuses on my individual contributions and research-oriented implementation for the RAG architectures project. It includes notebook-based implementations, prediction outputs, evaluation artifacts, fine-tuned model adapters, and comparative analysis across Baseline, Enhanced, and Agentic RAG systems.

The complete team project additionally included integrated scripts, configuration files, and collaborative implementation components developed as part of the overall system.
