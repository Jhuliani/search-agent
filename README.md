
# Search Agent — Sistema Multiagente com LangGraph, LangChain e Gemini

Este projeto implementa um estudo de um sistema multiagente capaz de responder perguntas complexas combinando:

- Busca na Web (Tavily)  
- Busca científica (arXiv)  
- Modelos de linguagem Gemini  
- Orquestração por grafo com LangGraph  

O objetivo é aprender como integrar LLMs + ferramentas + arquitetura multiagente para criar respostas mais completas e confiáveis.

---

## **Visão Geral**

O sistema recebe uma pergunta do usuário e realiza o seguinte fluxo:

1. **Agente Web** → faz uma busca geral usando Tavily  
2. **Agente Científico** → pesquisa artigos científicos no arXiv  
3. **Supervisor** → combina as respostas e gera uma resposta final estruturada  

O fluxo é controlado por um grafo no LangGraph:
START → web_search → scientific_search → supervisor → END



