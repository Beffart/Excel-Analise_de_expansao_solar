# 📊 Análise de Fatura de Energia Solar e Projeção de Expansão do Sistema (Excel)


[Acesse aqui a análise completa!](https://github.com/Beffart/Excel-Analise_de_expansao_solar/tree/main)

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


### 📊 Tratamento de Dados Faltantes

Como não havia dados históricos de consumo para os meses de novembro e dezembro, foi adotada a seguinte metodologia:

- Novembro: mediana do consumo entre janeiro e maio

- Dezembro: mediana do consumo entre junho e outubro

Essa abordagem garante:

- Coerência sazonal

- Continuidade da análise anual

- Redução de distorções nos resultados

<img width="563" height="352" alt="dados_entrada" src="https://github.com/user-attachments/assets/321ce5f3-b4e6-4544-b943-ec2e1154061e" />


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


<img width="684" height="352" alt="dados_analise" src="https://github.com/user-attachments/assets/ca8eed14-8ad7-4383-858f-31b241f0763c" />


## ☀️ Simulação de Expansão do Sistema Fotovoltaico

As últimas colunas, de “Nova Geração Proposta” até “Fatura com Expansão do Sistema”, são baseadas em uma simulação realizada em software específico de energia solar.

Essas colunas representam:

- Geração estimada após a expansão

- Geração total projetada

- Nova fatura estimada considerando o sistema expandido

📌 Aqui é apresentado ao cliente um cenário futuro realista, com base em dados técnicos e simulação profissional.


<img width="487" height="352" alt="dados_projecao" src="https://github.com/user-attachments/assets/0e70430a-cf8d-4fe4-9334-944f81a26aad" />


## 📈 Visualizações e Gráficos

O arquivo contém visualizações claras e objetivas, pensadas para facilitar a compreensão do cliente.

### 📉 Gráfico de Linha — Situação Atual

O primeiro gráfico de linha compara:

💸 Fatura estimada sem energia solar

⚡ Fatura atual com o sistema fotovoltaico existente

➡️ Esse gráfico evidencia o impacto positivo do sistema já instalado.

<img width="883" height="210" alt="linha_01" src="https://github.com/user-attachments/assets/9bc8cff2-2f23-4d72-8dff-054cc09bb2e7" />


### 📉 Gráfico de Linha — Projeção com Expansão

O segundo gráfico de linha apresenta:

Situação atual da fatura

Projeção da fatura após a expansão do sistema

<img width="881" height="234" alt="linha_02" src="https://github.com/user-attachments/assets/85694374-1b79-4d28-9389-70d6c04bc52f" />


➡️ Permite ao cliente visualizar claramente o benefício financeiro futuro, caso opte por uma expansão do sistema.

## 🥧 Gráfico de Pizza — Consumo vs Geração

O gráfico de pizza mostra:

🔌 Energia total necessária pelo cliente

☀️ Energia efetivamente gerada pelo sistema

➡️ Excelente recurso visual para explicar déficit ou sobra energética.


<img width="329" height="289" alt="pizza" src="https://github.com/user-attachments/assets/8320738a-12fc-4e49-b467-f3c46abb80b7" />


## 📌 Indicadores-Chave (KPIs)

O dashboard apresenta dois KPIs principais, focados em tomada de decisão:

💰 Economia anual atual proporcionada pelo sistema fotovoltaico

<img width="513" height="236" alt="KPI_01" src="https://github.com/user-attachments/assets/f9820cdb-77a6-4330-8adb-190e0cf78b9d" />


📈 Economia anual projetada caso o cliente opte pela expansão

<img width="512" height="234" alt="KPI_02" src="https://github.com/user-attachments/assets/4a887712-b180-4e44-9045-16213cd82f7c" />


Esses indicadores consolidam toda a análise técnica em valores financeiros claros e objetivos.

🎯 Conclusão

Este arquivo foi desenvolvido para apoiar decisões técnicas e comerciais no setor de energia solar, unindo:

- Dados reais de fatura

- Análises técnicas consistentes

- Simulações profissionais

- Visualizações claras para o cliente

O projeto demonstra como o Excel pode ser utilizado como uma poderosa ferramenta de análise energética, servindo tanto para estudos técnicos quanto para apresentações comerciais e tomada de decisão.
