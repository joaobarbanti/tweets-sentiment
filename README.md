##  📂 Classificador de sentimentos em tweets 

### Projeto com o intuito de utilizar modelos de machine learning e técnicas de NLP (Natural language processing) para classificar tweets sobre vacinas do coronavirus com base em seu sentimento, que se divide em tweets com sentimentos e escrita positiva, neutra e negativa.

## 💻 Processo Técnico

#### Comecei tratando e limpando os dados de texto dos tweets. No processo de identificar sentimentos em textos coisas como links, hashtags e pontuações excessivas precisam ser removidas pois em sua maioria não expressam nenhum tipo de sentimento humano, para eliminar esses atributos dos textos utilizei expressões regulares.
#### Em seguida utilizei a técnica de stemming para voltar todas as palavras dos tweets em sua forma original, esse processo torna qualquer modelo mais eficiente na hora de processar os dados pois reduz as variáveis de uma palavra que no fim expressam e representam a mesma coisa.
#### Usei o algoritmo TextBlob para classificar os textos com base em sua polarização, o algoritmo consome os textos dos tweets e os compara com seu dicionário de palavras, onde cada palavra ganha um nível de polarização que basicamente seria o sentimento que ela representa(positivo,negativo,neutro). Ele soma a polarização de cada palavra presente no texto e normaliza o resultado dando a cada tweet um valor maior que zero(positivo), zero(neutro) e menor que zero(negativo).
#### Para preparar o modelo de classificação primeiro usei o algoritmo CountVectorizer para tokenizar os dados de textos e os transformar em uma matriz de números, para assim serem usados no modelo. Com os dados prontos usei o modelo LogisticRegression para trabalhar com a classificação.

## 📂 Resultados:

### Desempenho modelo:
![desempenho modelo - tweets](https://github.com/user-attachments/assets/a9323a71-acd0-4bab-b33b-2ddbf30033dd)

### Palavras mais presentes em tweets classificados como positivos:
![positive words - tweet sentiment](https://github.com/user-attachments/assets/a61bbbe4-7230-4323-8fbd-987b03687120)
### Palavras mais presentes em tweets classificados como negativos:
![negative words - tweet sentiment](https://github.com/user-attachments/assets/6000d53d-931f-41b5-a424-2ea25d0df355)
### Palavras mais presentes em tweets classificados como neutros:
![neutral words - tweet sentiment](https://github.com/user-attachments/assets/3ea06485-e00b-49fc-91e9-b0d7263c7f0f)

### Gráficos importantes:
![download](https://github.com/user-attachments/assets/8bc427b6-e7f6-4155-bd4c-8524dc2ed4cc)
![download (1)](https://github.com/user-attachments/assets/d1f19bbd-64b7-4070-8dd0-312b419ffdcf)

## 💻 Tecnologias Usadas

##### Modelo LogisticRegression para classificação.
##### Biblioteca nlkt para processo de stemming
##### Biblioteca TextBlob para classificar textos com base em seus sentimentos.
##### Pandas e scikit learn para tratamento simples dos dados.


