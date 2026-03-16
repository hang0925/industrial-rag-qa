# 工业质检智能问答系统

基于RAG技术构建的工业质量检测领域智能问答系统

## 项目简介

本项目使用RAG（检索增强生成）技术，读取工业检测国家标准PDF文档建立知识库，
实现基于文档内容的精准问答，有效解决大模型幻觉问题。

## 技术栈

- LangChain：RAG框架
- DeepSeek API：大语言模型
- HuggingFace bge-small-zh：中文Embedding模型
- Chroma：向量数据库
- Python 3.13

## 知识库文档

- GB/T 46608-2025 钢管无损检测 表面缺陷机器视觉检测技术通则
- GB/T 46978-2026 无损检测 金属结构交流电磁场检测方法
- GB/T 33207-2025 无损检测 在役非铁磁性金属 管内氧化物堆积的磁性检测方法

## 使用方法

### 1. 安装依赖
pip install langchain langchain-community langchain-openai

pip install langchain-chroma chromadb pypdf

pip install sentence-transformers

### 2. 建立向量库
python create_database.py

### 3. 问答查询
python query_data.py "你的问题"

## 示例

输入：钢管表面缺陷检测有哪些方法

输出：根据文档，钢管表面缺陷检测的方法是机器视觉检测方法，
具体包括二维和/或三维检测方式。

来源：GB/T 46608-2025

