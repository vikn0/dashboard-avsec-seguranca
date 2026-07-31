# 🛡️ Análise Operacional e Ocorrências AVSEC

![Dashboard Preview](dashboard_preview.png)

Este relatório analisa os padrões operacionais, a distribuição temporal de ocorrências e a produtividade da equipe de segurança (**AVSEC**), utilizando dados consolidados do período.

---

## 1. Análise dos Dados

Os dados revelam uma forte concentração espacial e temporal nos acionamentos operacionais: a maioria esmagadora das ocorrências está centralizada no **1º Pavimento**, enquanto o período da **Manhã** responde pelo maior volume de demandas. O gráfico de linha temporal destaca o mês de **Janeiro** como um *outlier* de altíssima demanda (1.277 acionamentos), seguido por um padrão de estabilização nos meses subsequentes.

Entre os tipos de ocorrência, a categoria **Pedinte** representa a principal causa de acionamentos no local, seguida por **Comerciante Não Credenciado**.

---

## 2. Principais Indicadores Identificados (KPIs)

* **Acionamento Total:** 3.915 registros.
* **Tempo de Gravação Total:** 175h 30m 52s (tempo acumulado de acompanhamento).
* **Vigilante Mais Atuante:** Matheus.
* **Local Mais Utilizado:** Escadaria do EDG.
* **Distribuição por Período:** 
  * 🟢 **Manhã:** 59,57% dos acionamentos.
  * 🟡 **Tarde:** 36,07% dos acionamentos.
  * 🖤 **Noite:** 4,37% dos acionamentos.

---

## 3. Conclusões e Recomendações

* **Conclusão:** A operação de segurança apresenta uma demanda altamente previsível, concentrada no primeiro turno do dia e no primeiro pavimento. A redução de ocorrências após o pico de janeiro demonstra eficácia nas ações preventivas ou mudança no fluxo de frequentadores.
* **Recomendação:** A gestão operacional deve otimizar a escala de alocação dos vigilantes, reforçando a ronda no **1º Pavimento** durante o período da **Manhã** para mitigar abordagens de pedintes e comerciantes não credenciados, garantindo maior eficiência do efetivo.

---

## 🛠️ Tecnologias Utilizadas
* **Power Query (M):** Limpeza e parsing de dados textuais não estruturados.
* **DAX:** Tratamento de acumulado de tempo em formato contínuo (`[HH:MM:SS]`).
* **Power BI:** Modelagem e visualização de dados.
