# dual-architecture-culinary-ai
Dual-architecture AI recommendation system combining fine-tuned Llama 3 (QLoRA) and Hybrid RAG with FAISS + Gemini to generate context-aware, hallucination-resistant culinary recommendations.

Bridging the Semantic Gap in Culinary Recommendations
Overview

An advanced dual-architecture AI system designed to solve semantic understanding challenges in recipe recommendation systems.

The project combines:

A fine-tuned Meta Llama 3 (8B) model optimized using QLoRA for strict ingredient-constrained recipe generation.
A Hybrid Retrieval-Augmented Generation (RAG) pipeline integrating FAISS and Gemini API for semantic recipe exploration and contextual recommendation.

The architecture balances creativity, accuracy, semantic understanding, and hallucination resistance.

Problem Statement

Traditional recommendation systems rely on keyword matching methods such as:

TF-IDF
Collaborative Filtering
Matrix Factorization

These systems fail to understand abstract user intent such as:

Comfort food
Light dinner
Rainy day recipes
Protein-rich meals

Large Language Models solve semantic understanding but introduce hallucinations and high computational cost.

This project bridges both challenges using a hybrid dual-model architecture.

Core Features

✔ Fine-tuned Meta Llama 3 (8B) model
✔ QLoRA 4-bit quantization
✔ LoRA adapter fine-tuning
✔ Chain-of-Thought instruction tuning
✔ FAISS semantic retrieval pipeline
✔ Gemini API integration
✔ Hybrid RAG architecture
✔ Hallucination-resistant generation
✔ Ingredient-constrained recipe generation
✔ Semantic understanding of abstract user queries

Model 1: Fine-Tuned Domain Expert

The first module focuses on strict recipe generation.

Architecture
Base Model → Llama 3 8B
Quantization → QLoRA (4-bit NF4)
Fine-Tuning → PEFT + LoRA adapters
Training Framework → Unsloth
Dataset → 6000 Indian recipes
GPU → Tesla T4
Performance
Metric	Result
Perplexity	3.92
Ingredient Accuracy	87.2%
Latency	35–45 ms/token

Model 2: Hybrid RAG Architecture

Second module handles abstract semantic queries.

Components
Sentence Transformers all-MiniLM-L6-v2
FAISS vector database
Gemini API generative reasoning layer
Tech Stack
LLM Engineering
Meta Llama 3
QLoRA
LoRA
PEFT
Unsloth
NLP
Sentence Transformers
Semantic Embeddings
Prompt Engineering
Chain of Thought (CoT)
Retrieval
FAISS
Vector Similarity Search
Dense Retrieval
Libraries
PyTorch
Transformers
HuggingFace
Pandas
NumPy
Scikit-learn
Performance Highlights
Metric	Performance
Training Perplexity	3.92
Ingredient Constraint Accuracy	87.2%
Latency	35–45 ms/token
Dataset Size	6000 Recipes
Quantization	4-bit NF4
Research Contributions

This project demonstrates:

Efficient fine-tuning of large language models on consumer hardware
Hybrid retrieval + generation architecture
Reduction of hallucination in domain-specific LLM applications
Semantic recommendation systems beyond keyword matching
Edge-compatible AI deployment using quantization
Applications
Intelligent Recipe Recommendation Systems
Nutrition Recommendation Systems
Personalized Food Planning
AI Culinary Assistants
Healthcare Diet Recommendation Systems
Future Scope
Multimodal ingredient recognition using Computer Vision
Voice-based AI cooking assistant
Personalized nutrition recommendation engine
Edge deployment on mobile devices
Healthcare dietary planning integration
