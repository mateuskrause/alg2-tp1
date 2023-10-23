# alg2-tp1

Trabalho prático sobre geometria computacional para a disciplina DCC207. Criação de algoritmos de envoltória convexa e verificação de interseção de segmentos para o problema de classificação em aprendizado de máquina supervisionado.

Autores: @brisabn, @mateuskrause, @henriquemv23

## Objetivos

Se tem como meta a criação de um modelo que tem como objetivo atribuir rótulos a amostras desconhecidas com base nas características extraídas de um conjunto de treinamento. A premissa fundamental é a de que, ao entender as características principais das amostras de treinamento com diferentes rótulos, nosso algoritmo será capaz de generalizar e fazer previsões precisas para novos dados.
Para isso, delimitamos o escopo como sendo de dados bidimensionais e com duas classificações. Conjunto de dados com um número maior de características e classificações devem ser reduzidos utilizando outros algoritmos, como o SVD. Caso as classificações não sejam linearmente separáveis, apenas informamos não ser possível obter um modelo de classificação. 

Dado um Dataset bidimensional com duas classes, exploramos:
 - Determinar a envoltória convexa das classes, e com isso, verificar se são linearmente separáveis (podem ser separadas por uma única linha reta no plano);
 - Definir um modelo de classificação que traça uma reta perpedicular ao segmento mínimo entre as classes, e, com isso, determinar qual classe cada ponto pertence a partir da divisão da reta;
 - Avaliar o desempenho do classificador utilizando as seguintes métricas: precisão, revocação e f1-escore.

Nos algoritmos para reduzir dimensionalidade e avaliação de resultados, excepcionalmente, utilizamos algoritmos já disponíveis, visto que nosso objetivo é apresentar uma implementação de algoritmos geométricos.

## Exemplos

A seguir alguns exemplos de classificações feitas pelo algoritmo:

### Iris

Linearmente separável.  
Precisão: 1.0  
Revocação: 1.0  
F1-score: 1.0  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/6abbd92b-8aa8-42ff-83ce-74823291df36)


### Lymphography

Linearmente separável.  
Precisão: 0.5  
Revocação: 1.0  
F1-score: 0.6666666666666666  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/1d2b2208-f6dc-4290-a1f0-cc966eb465b8)

### Dermatology

Linearmente separável.  
Precisão: 1.0  
Revocação: 1.0  
F1-score: 1.0  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/ff0d1203-f106-4017-a6db-04a75da62655)


### Synthetic-3

Linearmente separável.  
Precisão: 0.9782608695652174  
Revocação: 0.9782608695652174  
F1-score: 0.9782608695652174  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/74f839df-e16a-4604-9d8d-de852ddafbbc)


### Twonorm

Não é linearmente separável.

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/05c7b09f-4b0d-4599-b221-4156798b0dd9)


