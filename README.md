# TinyLlama-medical-qa-system
Medical question answering system based on TinyLlama
```

## README.md 内容
```markdown
# Medical QA System
基于 TinyLlama 的医疗问答系统

## 功能特点
- 基于 TinyLlama-1.1B-Chat 模型
- 使用 LoRA 进行医疗领域微调
- 多 Agent 协作的问答系统
- 支持医学文献检索和分析

## 安装说明
1. 克隆仓库：
```bash
git clone https://github.com/yourusername/medical-qa-system.git
cd medical-qa-system
```

2. 安装依赖：
```bash
pip install -r requirements.txt
```

3. 下载模型：
```bash
python scripts/download_models.py
```

## 使用方法
1. 基本使用：
```python
from src.model import TransformersLLM
from src.agents import create_agents

# 创建向量存储
vectorstore = create_vectorstore()

# 创建agents
agents = create_agents(vectorstore)

# 处理查询
query = "What are the common treatments for diabetes?"
result = process_query(query, *agents)
```

2. 高级配置请参考 `docs/usage.md`

## 模型信息
- 基础模型：TinyLlama/TinyLlama-1.1B-Chat-v1.0
- LoRA 模型：[您的模型链接]

## License
MIT

## 引用
如果您使用了本项目，请引用：
[citation information]
```

## requirements.txt
```
langchain>=0.1.0
transformers>=4.36.0
torch>=2.1.0
peft>=0.7.0
faiss-cpu>=1.7.4
```
