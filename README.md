# TinyLlama-medical-qa-system
Medical question answering system based on TinyLlama
## Features
- Uses the TinyLlama-1.1B-Chat model
- Fine-tuned for the medical domain using LoRA
- Multi-agent collaborative question-answering system
- Supports medical literature retrieval and analysis

Installation Instructions
1. Clone the Repository：
```bash
git clone https://github.com/zkManuel0123/medical-qa-system.git
cd TinyLlama-medical-qa-system
```

2. Install Dependencies：
```bash
pip install -r requirements.txt
```

3. Download the Model：
using model_download.ipynb to download the models

## Usage
1. Basic Usage：
```python
from src.model import TransformersLLM
from src.agents import create_agents

# Create vector store
vectorstore = create_vectorstore()

# Create agents
agents = create_agents(vectorstore)

# Process a query
query = "What are the common treatments for diabetes?"
result = process_query(query, *agents)
```

## Model Information
- Base Model：TinyLlama/TinyLlama-1.1B-Chat-v1.0
- LoRA Model：https://huggingface.co/Kai0123/tinyllama-medical-qa-lora-model

## License
MIT

## Citation
If you use this project, please cite:
**Citation for Medical QA System**  
Kai Zhao. "TinyLlama-medical-qa-system." GitHub, 2024. Available at: https://github.com/zkManuel0123/medical-qa-system

**Citation for TinyLlama**  
Author(s) of TinyLlama. "TinyLlama Model." 

**Citation for Hugging Face Transformers**  
Thomas Wolf, et al. "Transformers: State-of-the-art Natural Language Processing." In Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations, 2020. Available at: https://github.com/huggingface/transformers

```
