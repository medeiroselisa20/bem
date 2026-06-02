# 📊 Análise de Séries Temporais do Consumo Musical no Brasil (Spotify Dataset)

## 📌 Visão Geral

Este projeto aplica técnicas de **mineração de dados e análise de séries temporais** para entender o comportamento do consumo musical no Brasil durante a pandemia de COVID-19 (2020–2021).

A análise foi realizada com base em dados de streams do Spotify, com foco em identificar padrões, tendências e oportunidades de previsão.

---

## 🎯 Problema de Negócio

Como o comportamento de consumo de música evoluiu ao longo do tempo durante a pandemia?

Este projeto busca responder perguntas como:

- Existem artistas que dominaram os streams nesse período?
- Como o volume de streams se comportou ao longo dos meses?
- É possível prever tendências futuras com base no histórico?

---

## 📊 Base de Dados

- Fonte: Spotify Charts  
- Período analisado: Fev/2020 até Dez/2021  
- Frequência: diária  
- Variável principal: número de streams  

### Variáveis principais:
- `Streams` (numérica contínua)  
- `Rank` (numérica discreta)  
- `Artista`, `Música`, `Região` (categóricas)  

---

## ⚙️ Metodologia

### 🧹 Pré-processamento
- Tratamento de valores ausentes utilizando **mediana**
- Separação de artistas em músicas com múltiplos participantes (feat)
- Filtragem dos dados para Top 200

### 📊 Análise Exploratória
- Identificação dos artistas com maior volume de streams
- Análise de distribuição dos dados
- Gráficos de tendência (line plot) e dispersão

### 📉 Análise de Séries Temporais
- ACF (Autocorrelation Function)
- PACF (Partial Autocorrelation Function)
- Identificação de dependências temporais

### 🔍 Decomposição da série
- Tendência
- Sazonalidade
- Resíduos

### 🤖 Modelagem
- ARIMA (seleção via AIC)
- Evolução para SARIMA (inclusão de sazonalidade)

---

## 📈 Resultados

- O modelo **ARIMA capturou a tendência**, mas apresentou limitações nos resíduos (padrão não aleatório)
- A inclusão da sazonalidade (**SARIMA**) melhorou significativamente o ajuste do modelo
- O modelo apresentou melhor desempenho para previsões de curto prazo
- Evidência de comportamento não estacionário na série temporal

---

## 💡 Principais Insights

- O consumo musical apresentou mudanças relevantes durante a pandemia
- Houve concentração significativa de streams em poucos artistas
- A série apresenta padrões temporais que exigem modelagem com componente sazonal
- Modelos simples podem não capturar toda a complexidade do comportamento do usuário

---

## ⚠️ Limitações

- Distribuição não normal dos dados
- Presença de outliers
- Redução de precisão em previsões de longo prazo

---

## 🚀 Próximos Passos

- Testar modelos mais avançados (ex: Prophet, LSTM)
- Incluir variáveis externas (ex: lançamentos, eventos)
- Refinar modelagem de sazonalidade

---

## 🛠️ Tecnologias Utilizadas

- KNIME  
- Python (integração no fluxo)  
- Modelos ARIMA / SARIMA  

---

## 📁 Estrutura do Projeto

📦 spotify-time-series-analysis

├── README.md  
→ Explicação do projeto e principais insights

├── knime/  
→ Contém o workflow do KNIME utilizado na análise

├── report/  
→ Contém o relatório completo do projeto em PDF

├── images/  
→ Contém os gráficos gerados no KNIME (ACF, decomposição, forecast)



## 🤝 Conexão com o Negócio

Este projeto demonstra como a análise de séries temporais pode ser aplicada para:

- Antecipar tendências de comportamento do consumidor  
- Apoiar tomada de decisão orientada a dados  
- Identificar padrões relevantes para estratégias de negócio  

Experiência diretamente conectada à minha atuação em **Customer Success**, onde análise de comportamento e histórico de dados são essenciais para tomada de decisão.

---

## 👤 Sobre mim

Sou profissional com experiência em Customer Success e análise de dados, atualmente em transição para a área de **Data Analytics**, aprofundando conhecimentos em modelagem, visualização e análise de dados.

📫 Vamos nos conectar: https://www.linkedin.com/in/elisa-barbosa-a81853146/
