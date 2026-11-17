# Assistente de Manuais em PDF — NVIDIA RAG

**Autor:** Kaiky Yoshio Ono Marins  
**Categoria:** Python · Streamlit · RAG · IA generativa  
**Status:** Protótipo funcional de estudo

## Visão geral

Aplicação Streamlit que permite fazer perguntas em português sobre um manual em PDF. O fluxo carrega o documento, divide o conteúdo em trechos, cria representações vetoriais e recupera partes relevantes para apoiar as respostas do modelo.

## Recursos implementados

- Interface web com Streamlit.
- Leitura de documentos PDF com PyPDFLoader.
- Divisão de texto em trechos.
- Busca semântica com FAISS.
- Embeddings NVIDIA e modelo de chat NVIDIA.
- Respostas contextualizadas pelo conteúdo do manual.

## Tecnologias

- Python e Streamlit
- LangChain
- FAISS
- NVIDIA NIM
- PyPDF

## Como executar

1. Instale as dependências de `requirements.txt`.
2. Configure `NVIDIA_API_KEY` no arquivo `.env` local ou nos Secrets do Streamlit.
3. Execute `streamlit run app.py`.
4. Utilize o manual PDF incluído no repositório.

Não coloque `.env` ou chaves reais no Git. O arquivo `manual.pdf` faz parte do material de demonstração.

© 2026 Kaiky Yoshio Ono Marins.