# Começar devagar ou acelerado? Uma análise Exploratória de Dados (Maratona de Boston 2015–2017)

Projeto de análise exploratória de dados em Python que investiga o impacto da estratégia de ritmo (*pacing*) no desempenho de **79.038 corredores** da Maratona de Boston (edições de 2015, 2016 e 2017).

**Pergunta central:** *Qual estratégia traz o melhor resultado na maratona: começar devagar ou acelerado?*

---

## Principais Resultados

A análise testou três hipóteses sobre o comportamento dos atletas ao longo dos 42,2 km:

1. **Otimização de tempo:** Apenas **4,4%** dos corredores começaram mais devagar (*negative split*, fazendo a segunda metade mais rápida que a primeira), mas concluíram a prova em média **18,7 minutos (8,0%) mais rápido** do que quem largou acelerado (215,2 min contra 233,9 min).
2. **A parede dos 30 km:** Quem larga em ritmo forte começa a perder velocidade antes mesmo da metade da prova e sofre uma queda brusca perto do km 30 (passando de 5,08 min/km nos 5K para 6,09 min/km nos 35K). Já quem começa devagar mantém constância e ainda acelera no trecho final (4,93 min/km nos 40K).
3. **Regularidade de ritmo:** Corredores que mantêm baixa variação de ritmo ao longo dos trechos terminam a maratona, em média, **58,2 minutos (22,0%) mais rápido** do que atletas com alta oscilação de velocidade (206,0 min contra 264,2 min).

---

## Estrutura do Repositório

```text
├── Análise Final/    #Estudo finalizado
│   ├── Maratona Boston (Apresentação final).pdf     
│   └── Análise_de_dados_em_pyhton.ipynb   
├── Análise Parcial/    #Estudo inicial
│   └── Maratona Boston (Apresentação parcial).pdf
│   └── Análise_de_dados_parcial.ipynb
├── DataSets (.csv)/    #Datasets utilizados no estudo
│   └── marathon_results_2015.csv
│   └── marathon_results_2016.csv
│   └── marathon_results_2017.csv
└── README.md
```

---

## Tecnologias Utilizadas

* **Python 3** (executado via Google Colab)
* **Pandas** — unificação, limpeza e agrupamento dos dados
* **NumPy** — classificação das estratégias de corrida
* **Matplotlib** — geração dos gráficos comparativos

---

## Base de Dados e Como Executar

Os dados públicos utilizados estão disponíveis no Kaggle: [Boston Marathon Results (2015–2017)](https://www.kaggle.com/datasets/rojour/boston-results).

Para reproduzir a análise:

1. Baixe os três arquivos CSV (`marathon_results_2015.csv`, `marathon_results_2016.csv` e `marathon_results_2017.csv`);
2. Abra o arquivo `Análise Final/Analise_de_dados_em_python.ipynb` no **Google Colab**;
3. Faça o upload dos três arquivos CSV para a sessão do Colab;
4. No menu superior, clique em **Ambiente de execução > Executar tudo**.
