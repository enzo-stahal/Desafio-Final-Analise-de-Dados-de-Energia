# Desafio Final — Análise de Dados de Energia com API Pública

## 📌 Sobre o projeto

Este projeto foi desenvolvido como parte da disciplina de **Soluções em Energias Renováveis e Sustentáveis**, do curso de **Ciência da Computação**.

O objetivo da atividade é analisar o comportamento da **carga elétrica** de uma região atendida pelo **Sistema Interligado Nacional (SIN)** utilizando dados obtidos diretamente de uma **API pública do Operador Nacional do Sistema Elétrico (ONS)**.

A análise foi realizada utilizando Python e bibliotecas para manipulação, análise e visualização de dados.

## 🎯 Objetivos

O projeto tem como objetivos:

* Construir um DataFrame a partir dos dados obtidos pela API do ONS;
* Inspecionar e organizar os dados;
* Identificar e tratar valores ausentes;
* Verificar os tipos das variáveis;
* Calcular indicadores estatísticos da carga elétrica;
* Identificar períodos de alta demanda;
* Criar diferentes critérios de análise;
* Produzir gráficos para visualização dos dados;
* Elaborar um relatório técnico com base nos resultados obtidos;
* Realizar uma validação crítica das conclusões apresentadas.

## 📊 Dados analisados

Inicialmente, foi analisada a área de carga:

* **Área:** SP — São Paulo
* **Período:** 01/08/2025 a 07/08/2025
* **Sistema:** Sistema Interligado Nacional (SIN)
* **Fonte:** Operador Nacional do Sistema Elétrico (ONS)

Os dados utilizados correspondem à **Carga Verificada do ONS**.

## 🔎 Metodologia

A análise foi dividida em diferentes etapas.

### 1. Construção e inspeção dos dados

Os registros retornados pela API são transformados em um DataFrame utilizando a biblioteca Pandas.

São realizadas análises como:

* visualização dos primeiros registros;
* quantidade de linhas e colunas;
* identificação dos atributos;
* análise dos tipos de dados;
* estatísticas descritivas.

### 2. Organização dos dados

Os principais atributos são selecionados e recebem nomes mais simples para facilitar a análise.

Também são verificadas:

* informações de data e hora;
* valores ausentes;
* representação numérica da carga;
* organização cronológica das observações.

### 3. Indicadores da carga elétrica

São calculados os seguintes indicadores:

* carga mínima;
* carga máxima;
* carga média;
* mediana;
* amplitude entre o máximo e o mínimo;
* quantidade total de medições.

Esses indicadores são utilizados para avaliar o comportamento geral da carga durante o período analisado.

### 4. Períodos de alta demanda

Foi definido como **alta demanda** todo registro cuja carga seja superior a **90% da carga máxima observada**.

Para esse critério são calculados:

* limiar de alta demanda;
* quantidade de registros;
* percentual em relação ao total;
* maior valor de carga;
* data e horário do pico, quando disponíveis.

### 5. Segundo critério de análise

Além do critério de alta demanda, é utilizado um segundo recorte considerando os registros com **carga acima da média**.

Esse segundo conjunto é comparado com os registros classificados como alta demanda.

### 6. Visualização

São produzidos pelo menos dois gráficos:

1. comportamento da carga ao longo do tempo;
2. distribuição dos valores de carga.

Os gráficos são utilizados para auxiliar na interpretação dos resultados.

## 🛠️ Tecnologias utilizadas

* **Python**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Requests**
* **Google Colab**
* **API pública do ONS**

### Notebook

O arquivo `Desafio_Final_Energia_ONS_Completo.ipynb` contém os códigos, resultados, gráficos, análises e relatório desenvolvidos durante a atividade.

## 🌐 Fonte dos dados

Os dados foram obtidos por meio da API pública do **Operador Nacional do Sistema Elétrico (ONS)**.

### Portal de dados do ONS

https://dados.ons.org.br/

### Conjunto de dados — Carga de Energia Verificada

https://dados.ons.org.br/dataset/carga-energia-verificada

### API utilizada

https://apicarga.ons.org.br/prd/cargaverificada

## 📈 Resultados

Os resultados quantitativos da análise, incluindo os indicadores estatísticos, períodos de alta demanda, pico de carga e gráficos, estão apresentados no notebook.

As conclusões foram elaboradas com base nos resultados produzidos durante a análise, evitando atribuir causas às variações que não possam ser comprovadas pelos dados.

## 🤖 Uso de Inteligência Artificial

O notebook prevê o uso do **Gemini** como apoio para a elaboração do relatório técnico.

A IA recebe os resultados calculados pela equipe e auxilia na organização e redação do relatório. Posteriormente, o texto gerado é submetido a uma **validação crítica**, verificando se as informações apresentadas são compatíveis com os dados, indicadores e gráficos obtidos.

## 👥 Disciplina

**Curso:** Ciência da Computação
**Disciplina:** Soluções em Energias Renováveis e Sustentáveis

## 📚 Referências

**Operador Nacional do Sistema Elétrico — ONS**

Portal de dados:
https://dados.ons.org.br/

Dataset:
https://dados.ons.org.br/dataset/carga-energia-verificada

API:
https://apicarga.ons.org.br/prd/cargaverificada
