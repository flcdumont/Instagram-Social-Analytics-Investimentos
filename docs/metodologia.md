# 🧱 Metodologia do Projeto

## 1. Coleta de Dados
- Ferramenta: **PhantomBuster (Instagram Hashtag Collector)**
- Hashtag: `#investimentos`
- Campos coletados: autor, legenda, data, curtidas, comentários, link do post.

## 2. Limpeza de Dados
- Ferramenta: **Python + pandas**
- Remoção de duplicatas e normalização de datas.

## 3. Análise de Sentimento (NLP)
- Ferramenta: **Transformers (Hugging Face)**
- Modelo: `nlptown/bert-base-multilingual-uncased-sentiment`
- Saída: positivo, neutro, negativo.

## 4. Análise de Rede (SNA)
- Ferramenta: **Python (networkx)** + **Gephi**
- Criação de grafo com base nas menções e interações entre usuários.

## 5. Dashboard
- Ferramenta: **Looker Studio**
- Fontes: `posts_clean.csv`, `comments_sentiment.csv`
- Métricas: Engajamento, Sentimento, Top Influenciadores, Crescimento Temporal.

## 6. Insights Automáticos
- Ferramenta: **ChatGPT / Narrative BI**
- Geração de insights descritivos baseados nas métricas e correlações observadas.