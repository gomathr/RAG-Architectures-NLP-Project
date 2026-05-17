# RAG Architectures for Question Answering (HotpotQA) - NLP Project
Development and Evaluation of Baseline, Enhanced and Hierarchical Agentic Retrieval
Augmented Generation (RAG) Architectures for Improving Large Language Models
This project explores Retrieval-Augmented Generation (RAG) to improve the performance of large language models by incorporating external knowledge and reducing hallucinations. 
We evaluate multiple RAG architectures, including Baseline RAG, Enhanced RAG (LightRAG), and Agentic RAG with hierarchical retrieval, on the HotpotQA dataset. The study focuses on improving answer quality, faithfulness, and multi-hop reasoning using pretrained transformer-based models and evaluation metrics.
## My Contributions

### A) Dataset and Model Selection
- Contributed to dataset selection (HotpotQA), preparation and preprocessing 
- Selected and configured pretrained models for all RAG architectures, including the encoder (BGE-M3), vector database (FAISS), and generator (Qwen)

### B) System Design
- Designed and implemented the Baseline RAG architecture using pretrained models  

### C) Fine-Tuning of the Generator (Qwen)
- Developed the fine-tuning strategy using Supervised Fine-Tuning (SFT) with LoRA  
- Designed experiments comparing pretrained and fine-tuned models using EM and F1 metrics, demonstrating performance improvements  

### D) Hyperparameter Tuning (Validation Set)
- Created helper functions to perform hyperparameter tuning across multiple configurations, including top-k retrieval, temperature, and maximum tokens  
- Analyzed model performance and selected optimal configurations  

### E) Visualization Setup
- Developed helper functions to visualize experimental results using comparative bar charts (pretrained vs fine-tuned models)  
- Created visualizations for hyperparameter tuning across multiple configurations, and applied optimal values to the final test set  

### F) Evaluation Methods
- Conducted comprehensive evaluation using EM, F1, BERTScore, and RAGAS metrics  

### G) Additional Contributions to the Team
- created the zip file 'qwen_hotpotqa_lora_final.zip and Provided this zip file for integration into Enhanced and Agentic RAG architectures  
- Shared helper function designs for hyperparameter tuning, evaluation (EM and F1), and visualization  
- Led documentation and report structuring in an organized manner  

## Dataset

- HotpotQA dataset is used for training, validation, and testing

## Project Structure

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


## Repository Note

This repository focuses on my individual contributions and research-oriented implementation for the RAG architectures project. It includes notebook-based implementations, prediction outputs, evaluation artifacts, fine-tuned model adapters, and comparative analysis across Baseline, Enhanced, and Agentic RAG systems.

The complete team project additionally included integrated scripts, configuration files, and collaborative implementation components developed as part of the overall system.
