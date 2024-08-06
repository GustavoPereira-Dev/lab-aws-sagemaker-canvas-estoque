# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".
- Para isso, siga o [passo a passo] descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.
- Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.
-   Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.
-   Faça o upload do dataset no SageMaker Canvas.

### 2. Construir/Treinar

-   No SageMaker Canvas, importe o dataset que você selecionou.
-   Configure as variáveis de entrada e saída de acordo com os dados.
-   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

### 5. Resultado

- Dataset utilizado: "dataset-1000-com-preco-promocional-e-renovacao-estoque"
- Alvo: Coluna "QUATIDADE_ESTOQUE"
- Id: "ID_PRODUTO"
- Validação de Datas: "DATA_EVENTO"

#### Métricas

- AVGwQL (0.39): chamado de Erro Quadrático Médio Ponderado, é uma métrica que combina o RMSE com pesos diferentes para diferentes amostras que pode ser utilizada quando algumas amostras são mais importantes que outras. Valores baixos indicam melhor ajuste.
- MAPE (0,132): chamado de Erro Absoluto Percentual Médio, é usado para avaliar modelos de regressão, especialmente em previsão de séries temporais, sendo expresso em porcentagem, facilita a comunicação dos resultados para pessoas não técnicas. Um MAPE baixo indica que o modelo está prevendo com precisão.
- WAPE (0,108): chamado de Erro Percentual Absoluto Ponderado, é semelhante ao MAPE com a diferença que pondera os erros percentuais absolutos. É útil para previsões de demanda, onde a magnitude das observações varia muito. Valores baixos indicam melhor ajuste.
- RMSE (6): chamado de Raiz do Erro Quadrático Médio, é uma métrica amplamente usada para medir o desempenho de modelos de regressão que calcula o erro médio nas unidades originais da variável alvo. Valores baixos indicam melhor ajuste do modelo.
- R² (0.240): chamado de Coeficiente de Determinação, ele avalia a proporção da variabilidade da variável dependente explicada pelo modelo. Varia entre 0 e 1; quanto mais próximo de 1, melhor o ajuste do modelo aos dados observados.
- MASE (0,50): chamado de Erro Médio Absoluto de Escala Média, ele compara o erro absoluto médio do modelo com o erro absoluto médio de um modelo de referência (como a média móvel) e é útil para séries temporais com sazonalidade.


