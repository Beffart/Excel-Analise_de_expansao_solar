# 📊 Análise de Fatura de Energia Solar e Projeção de Expansão do Sistema (Excel)

## 📌 Introdução

Este projeto consiste em uma análise detalhada da fatura de energia elétrica de um cliente com sistema fotovoltaico já instalado, bem como uma simulação financeira e energética de expansão do sistema solar.

O objetivo principal do arquivo é:

- Avaliar o consumo real do cliente

- Quantificar a economia atual proporcionada pelo sistema fotovoltaico

- Projetar como a fatura se comportaria sem energia solar

- Simular o impacto financeiro e energético de uma expansão do sistema fotovoltaico

Todo o estudo foi desenvolvido em Excel, utilizando dados reais de faturas, cálculos analíticos próprios e resultados de simulação provenientes de software especializado em energia solar.

<img width="1292" height="651" alt="Geral" src="https://github.com/user-attachments/assets/67e4516f-5d50-437c-8ea3-27997927a073" />

## 🛠️ Habilidades em Excel Utilizadas

Este projeto demonstra o uso prático de Excel aplicado ao setor de energia:

🧮 Fórmulas condicionais e estatísticas

📊 Gráficos de linha e pizza

📐 Análise de consumo e geração energética

📉 Comparativos financeiros

🧠 Modelagem de cenários

📁 Organização e estruturação de dados técnicos



## 🧠 Estrutura e Lógica do Arquivo

O arquivo está organizado de forma didática e sequencial, facilitando tanto a leitura técnica quanto a apresentação ao cliente.

### 🧾 Dados de Entrada — Fatura do Cliente

As colunas iniciais, compreendidas entre “Mês” e “Energia Injetada”, são dados reais extraídos diretamente das faturas de energia elétrica do cliente, incluindo:

📅 Mês de referência

Datas de leitura

Dias faturados

⚡ Energia consumida (kWh)

💰 Valor da fatura

🔄 Energia injetada na rede

📌 Esses dados representam a situação real e atual do cliente.

## 📐 Análises Técnicas Realizadas

As colunas compreendidas entre “Geração” e “Energia Necessária” correspondem às análises desenvolvidas manualmente, com base nos dados da fatura e em critérios técnicos.

- Essas análises incluem:

- Estimativa de geração do sistema atual

- Autoconsumo

- Consumo total real do cliente

- Estimativa da fatura caso o cliente não possuísse energia solar

- Energia total necessária para suprir o consumo anual

### 📊 Análise de geração solar


A análise da geração do cliente foi obtida via sistema de monitoramento. Dentro do excel a análise foi obtida pela seguinte fórmula:

```
=SUMIFS(
    Resumo_Monitoramento!B:B;
    Resumo_Monitoramento!A:A; ">=" & Análise!$B4;
    Resumo_Monitoramento!A:A; "<=" & Análise!$C4
)
````

Desta forma, foi possível comparar os valores de geração com os valores exatos da medição obtidos na fatura do cliente.

### 📊 Tratamento de Dados Faltantes

Como não havia dados históricos de geração para os meses de novembro e dezembro, foi adotada a seguinte metodologia:

- Novembro: mediana da geração entre janeiro e maio

- Dezembro: mediana da geração entre junho e outubro

Essa abordagem garante:

- Coerência sazonal

- Continuidade da análise anual

- Redução de distorções nos resultados

## ☀️ Simulação de Expansão do Sistema Fotovoltaico

As últimas colunas, de “Nova Geração Proposta” até “Fatura com Expansão do Sistema”, são baseadas em uma simulação realizada em software específico de energia solar.

Essas colunas representam:

- Geração estimada após a expansão

- Geração total projetada

- Nova fatura estimada considerando o sistema expandido

📌 Aqui é apresentado ao cliente um cenário futuro realista, com base em dados técnicos e simulação profissional.

## 📈 Visualizações e Gráficos

O arquivo contém visualizações claras e objetivas, pensadas para facilitar a compreensão do cliente.

### 📉 Gráfico de Linha — Situação Atual

O primeiro gráfico de linha compara:

💸 Fatura estimada sem energia solar

⚡ Fatura atual com o sistema fotovoltaico existente

➡️ Esse gráfico evidencia o impacto positivo do sistema já instalado.

### 📉 Gráfico de Linha — Projeção com Expansão

O segundo gráfico de linha apresenta:

Situação atual da fatura

Projeção da fatura após a expansão do sistema

➡️ Permite ao cliente visualizar claramente o benefício financeiro futuro.

## 🥧 Gráfico de Pizza — Consumo vs Geração

O gráfico de pizza mostra:

🔌 Energia total necessária pelo cliente

☀️ Energia efetivamente gerada pelo sistema

➡️ Excelente recurso visual para explicar déficit ou sobra energética.


## 📌 Indicadores-Chave (KPIs)

O dashboard apresenta dois KPIs principais, focados em tomada de decisão:

💰 Economia anual atual proporcionada pelo sistema fotovoltaico

📈 Economia anual projetada caso o cliente opte pela expansão

Esses indicadores consolidam toda a análise técnica em valores financeiros claros e objetivos.
