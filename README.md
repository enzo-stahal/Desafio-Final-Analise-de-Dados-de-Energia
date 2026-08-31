# Desafio Final — Análise de Dados de Energia com API Pública

## Sobre o projeto do desafio

Projeto desenvolvido para a disciplina de **Soluções em Energias Renováveis e Sustentáveis**, do curso de **Ciência da Computação**.

O objetivo é analisar o comportamento da **carga elétrica de São Paulo**, utilizando dados da **API pública do Operador Nacional do Sistema Elétrico (ONS)**.

A análise foi realizada em **Python**, utilizando bibliotecas de manipulação e visualização de dados.

## Objetivos

* Obter dados de carga elétrica por meio da API do ONS;
* Criar e organizar um DataFrame com **Pandas**;
* Verificar e tratar valores ausentes;
* Analisar tipos e características dos dados;
* Calcular indicadores estatísticos da carga;
* Identificar períodos de alta demanda;
* Comparar diferentes critérios de demanda;
* Criar gráficos para visualizar os resultados;
* Elaborar e validar um relatório técnico.
  
## Dados analisados

* **Área:** SP — São Paulo
* **Período:** 01/08/2025 a 07/08/2025
* **Sistema:** Sistema Interligado Nacional (SIN)
* **Dados:** Carga Verificada
* **Fonte:** Operador Nacional do Sistema Elétrico (ONS)

## Metodologia

Os dados obtidos pela API foram transformados em um DataFrame e analisados utilizando **Pandas**.

Foram realizadas:

1. **Inspeção dos dados** — análise de registros, colunas, tipos e estatísticas;
2. **Organização** — seleção e renomeação de atributos, tratamento de datas e valores ausentes;
3. **Análise estatística** — cálculo de carga mínima, máxima, média, mediana, amplitude e quantidade de medições;
4. **Alta demanda** — identificação de registros com carga superior a **90% da carga máxima**;
5. **Segundo critério** — identificação dos registros com carga **acima da média**;
6. **Visualização** — criação de gráficos da carga ao longo do tempo e da distribuição dos valores.

## Tecnologias utilizadas

* Python
* Pandas
* Matplotlib
* Seaborn
* Requests
* Google Colab
* API pública do ONS

## Disciplina

**Curso:** Ciência da Computação
**Disciplina:** Soluções em Energias Renováveis e Sustentáveis

---

# Links e referências

### Portal de Dados do ONS

[https://dados.ons.org.br/](https://dados.ons.org.br/?utm_source=chatgpt.com)

### Dataset — Carga de Energia Verificada

[https://dados.ons.org.br/dataset/carga-energia-verificada](https://dados.ons.org.br/dataset/carga-energia-verificada?utm_source=chatgpt.com)

### API — Carga Verificada

[https://apicarga.ons.org.br/prd/cargaverificada](https://apicarga.ons.org.br/prd/cargaverificada?utm_source=chatgpt.com)

