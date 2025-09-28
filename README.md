
# Análise de Atrasos de Voos (2020–2022)

Este projeto consiste em um notebook de análise de dados que investiga atrasos de voos entre os anos de 2020 e 2022. A análise oferece insights detalhados sobre aeroportos, companhias aéreas, padrões temporais e tendências mensais de atrasos, com recomendações para otimização operacional.

---


## Introdução

O objetivo desta análise é fornecer uma visão detalhada dos atrasos de voos, definidos como partidas com mais de 15 minutos de atraso, a partir de dados de 36 arquivos CSV, totalizando mais de 2,4 milhões de registros. Os insights são direcionados a profissionais do setor aéreo, pesquisadores e stakeholders interessados em eficiência operacional.

---

## Dados Utilizados

* **Arquivos de voos:** 36 arquivos CSV contendo informações sobre partidas, chegadas, situação do voo, aeroportos e companhias aéreas.
* **Dados de aeroportos:** arquivo CSV complementar com informações de identificação, nome e localização dos aeroportos.
* **Período analisado:** 2020, 2021 e 2022.

---

## Preparação e Limpeza

* Leitura robusta de múltiplos arquivos CSV, tratando diferentes separadores (`;` ou `,`) e linhas de cabeçalho inconsistentes.
* Filtragem para voos **REALIZADOS** e conversão de colunas de datas e horários para `datetime`.
* Cálculo de atrasos em minutos para partida e chegada, considerando apenas valores não negativos.
* Marcação de voos atrasados (`Voo Atrasado`) com atraso superior a 15 minutos.
* Derivação de colunas adicionais: dia da semana, período do dia e ano.
* Junção com dados de aeroportos (quando disponíveis).

---

## Como Executar

1. Ajustar os caminhos dos arquivos CSV de voos e aeroportos no notebook.
   https://drive.google.com/drive/folders/1zyrjujAG3FgXfNAKPQZ0BAaqoMWO5Bu_?usp=drive_link
3. Executar o notebook em ambiente Jupyter ou Google Colab.
4. Instalar dependências: `pandas`, `numpy`, `plotly`.
