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

- baseline_rag.ipynb – Implementation of Baseline RAG on pretrained and fine-tuned models  
- enhanced_rag.ipynb – Implementation of Enhanced RAG (LightRAG-style) on pretrained and fine-tuned models  
- qwen_hotpotqa_lora_final.zip – Fine-tuned Qwen model (LoRA adapters)  
- README.md – Project overview and documentation
- ## Repository Note

This repository focuses on my individual contributions and notebook-based implementation. The full team-integrated version includes additional scripts, configuration files, prediction outputs, and model artifacts for Baseline, Enhanced, and Agentic RAG pipelines.

Sample prediction files (.jsonl) represent model outputs used for evaluation across the different RAG architectures as part of the team project.
