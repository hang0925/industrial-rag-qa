# industrial-rag-qa
基于RAG技术的工业质检智能问答系统，使用LangChain+DeepSeek+FAISS构建，支持基于国家标准文档的精准问答

**核心技术栈：** LangChain + FAISS + DeepSeek API + Streamlit

**背景：**
工厂积累了大量质检文档，查阅效率低
大模型直接回答会产生幻觉，工业场景风险高

**技术：**

RAG = 先检索文档，再让模型基于文档回答

Embedding = 把文字转成向量（本质是特征提取）

FAISS = 向量数据库，语义相似度检索

DeepSeek = 生成最终回答

**联系专业：**

Embedding特征提取 = 模式识别核心

向量检索 = 模式匹配

整个系统 = 感知+决策的智能系统
