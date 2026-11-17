# Assistente de Manuais em PDF — NVIDIA RAG

**Autor:** Kaiky Yoshio Ono Marins  
**Portfólio:** [kaikysec.vercel.app](https://kaikysec.vercel.app/)  
**Categoria:** Python · Streamlit · RAG · IA generativa  
**Status:** Protótipo funcional de estudo

## Visão geral

Aplicação em Streamlit que permite fazer perguntas em português sobre um manual em PDF. Em vez de depender apenas de uma resposta genérica do modelo, o fluxo recupera trechos do documento e os utiliza como contexto para gerar a resposta.

## Problema e proposta

Manuais extensos podem ser difíceis de consultar. O projeto experimenta uma interface de perguntas e respostas que ajuda a localizar informações relevantes no documento fornecido.

## Como funciona

1. O manual PDF é carregado e seu texto é extraído.
2. O conteúdo é dividido em trechos menores.
3. Embeddings são gerados para representar os trechos.
4. O FAISS indexa os vetores e permite a busca semântica.
5. Os trechos recuperados são enviados como contexto ao modelo de linguagem.

## Funcionalidades implementadas

- Interface de chat com Streamlit.
- Leitura de PDF com PyPDFLoader.
- Divisão do documento em trechos.
- Busca semântica com FAISS.
- Embeddings NVIDIA e modelo de chat via NVIDIA NIM.
- Respostas contextualizadas pelo conteúdo recuperado.

## Tecnologias

- Python e Streamlit
- LangChain
- FAISS
- NVIDIA NIM
- PyPDF

## Como executar

1. Instale as dependências listadas em `requirements.txt`.
2. Configure `NVIDIA_API_KEY` em um arquivo `.env` local ou nos Secrets do ambiente de hospedagem.
3. Execute `streamlit run app.py`.
4. Utilize o manual PDF incluído no repositório.

## Limitações e cuidados

Este é um protótipo de estudo. A recuperação pode não encontrar o trecho correto e modelos de linguagem podem gerar respostas imprecisas. Confira sempre a resposta no PDF original. Não use o resultado como única fonte para decisões técnicas ou de segurança.

Nunca envie arquivos `.env` ou chaves reais ao Git.

## O que este projeto demonstra

- Construção de um fluxo RAG sobre documentos.
- Integração entre interface, embeddings, banco vetorial e modelo de linguagem.
- Organização de uma aplicação de IA em etapas compreensíveis.

© 2026 Kaiky Yoshio Ono Marins.
