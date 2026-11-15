# Predição de Viradas no League of Legends (Esports Analytics)

**Autor:** Otto Ettinger  
**Instituição:** Centro Universitário de Jaguariúna (UniFAJ) - Ciência da Computação (TechDay 2026)

## Sobre o Projeto
Este projeto aplica algoritmos de Machine Learning para prever a probabilidade de vitórias de times que estão em desvantagem econômica aos 15 minutos em partidas competitivas de League of Legends. 

Como reversões de jogo (comebacks) são estatisticamente raras e representam a minoria dos cenários no cenário competitivo, o projeto foca em tratar o desbalanceamento dos dados utilizando reamostragem sintética (SMOTE). O modelo isola métricas de macro game — como diferença de ouro, abates e a evolução econômica entre os minutos 10 e 15 — para calcular a viabilidade matemática de uma virada.

## Estrutura do Repositório
* `lol_analise.py`: Pipeline principal de dados em Python. Inclui extração, pré-processamento, balanceamento (SMOTE), treinamento dos modelos (Decision Tree e MLPClassifier) e plotagem das métricas (Curva ROC, Precision-Recall e Matrizes de Confusão).
* `otto_lol_notebook.html`: Dashboard analítico e simulador preditivo. Uma interface web estática que aplica a regressão gerada pelo modelo, permitindo testar cenários de partida em tempo real.
* `2026_LoL_esports_match_data_from_OraclesElixir.csv`: Base de dados bruta contendo os registros de partidas competitivas oficiais.
* `requirements.txt`: Dependências do ambiente Python.

## Tecnologias Utilizadas
* Python (Pandas, NumPy)
* Scikit-Learn e Imbalanced-Learn
* Matplotlib e Seaborn
* HTML/CSS/JavaScript

## Como Executar

1. Clone o repositório para sua máquina local.
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
