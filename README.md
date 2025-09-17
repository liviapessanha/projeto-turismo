# Sistema de Assistente Turístico com LLM e RAG

**Trabalho acadêmico desenvolvido para a disciplina de Inteligência Artificial na Prática**.

Este projeto tem como objetivo criar um sistema capaz de classificar a intenção de consultas de turistas e direcioná-las para a cadeia de processamento adequada. O sistema permite gerar roteiros personalizados, responder perguntas sobre logística e fornecer informações locais utilizando técnicas de LLM e Retrieval-Augmented Generation (RAG).

---

## Objetivos do Trabalho

- **Roteiros personalizados**: Geração de itinerários com base no perfil do turista (cultural, gastronômico, aventura, etc.).  
- **Cadeias especializadas**: Cada tipo de pergunta é direcionado a uma chain específica:
  - Itinerary Chain (roteiro de viagem)
  - Logistics Chain (transporte e hospedagem)
  - Local Info Chain (informações locais, usando RAG)
- **RAG (Retrieval-Augmented Generation)**: Permite acessar informações externas atualizadas para respostas mais precisas.
- **Arquitetura modular**: Possibilita a fácil expansão com novas cidades, funcionalidades ou bases de conhecimento.

---

## Tecnologias Utilizadas

- **LangChain**: Orquestração das chains e prompts.  
- **Groq / Llama 3.3**: Modelo LLM de alto desempenho para gerar respostas.  
- **Pinecone**: Base de dados vetorial para implementação do RAG.  
- **HuggingFace Embeddings**: Transformação de texto em vetores para RAG.  
- **Python**: Linguagem principal do projeto, com notebooks `.ipynb` para facilitar a demonstração.

---


## Como Rodar

1. Crie um ambiente Python (recomendado Anaconda) e instale as dependências:

```bash
conda create -n turismo python=3.10
conda activate turismo
pip install -r requirements.txt
