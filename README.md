# 🛡️ Análise Operacional de Segurança AVSEC

![Dashboard Preview](img/dashboard_preview.png)

## 📌 Visão Geral do Projeto
Este projeto consiste no desenvolvimento de um painel analítico para acompanhamento das operações e acionamentos da equipe de segurança (**AVSEC**). O objetivo é fornecer visibilidade clara sobre o tempo total de gravação, os locais de maior ocorrência, os períodos do dia de maior demanda e a atuação da equipe de vigilantes.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Power Query (M):** Limpeza, tratamento e padronização de dados brutos de texto, correção de incongruências em datas e delimitadores.
* **DAX:** Criação de medidas de desempenho e formatação personalizada para acúmulo de tempo contínuo superior a 24 horas.
* **Power BI:** Modelagem de dados (Star Schema) e construção do relatório interativo.

---

## 🧹 Principais Desafios de ETL e Tratamento de Dados
Durante a fase de preparação de dados no Power Query, foram resolvidas diversas inconsistências da base original:
1. **Normalização de Datas:** Tratamento de entradas em padrões mistos (BR/EUA) e presença de delimitadores incorretos (`:` ao invés de `/`).
2. **Parsing de Texto Não Estruturado:** Extração precisa dos nomes dos vigilantes a partir da coluna de ações tomadas, lidando com variações de nomenclatura e múltiplos delimitadores (`até`, `a saída`, `a rampa`).
3. **Cálculo Acumulado de Tempo em DAX:** Resolução do limite nativo do Power BI de 24 horas na exibição do tempo total gravado através da conversão para segundos e reconversão em string `[HH:MM:SS]`.

---

## 📊 Principais Insights do Painel
* **Tempo Total Gravado:** Mais de **175 horas** de acionamentos registrados ao longo do período.
* **Concentração Espacial:** O **1º Pavimento** concentrou a grande maioria dos acionamentos (`~2.790` ocorrências).
* **Distribuição Temporal:** O período da **Manhã** representa a maior fatia dos acionamentos (`~59,5%`), seguido da **Tarde** (`~36%`).
* **Sazonalidade:** Pico acentuado de acionamentos no mês de **Janeiro** (`1.277` registros), apresentando estabilização nos meses subsequentes.

---

## 📂 Como Replicar este Projeto
1. Clone este repositório:
   ```bash
   git clone [https://github.com/SEU-USUARIO/dashboard-avsec-seguranca.git](https://github.com/SEU-USUARIO/dashboard-avsec-seguranca.git)
