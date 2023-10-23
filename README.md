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

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/069c419a-aa27-4431-a127-6ba43debefcd)



### Lymphography

Linearmente separável.  
Precisão: 0.5  
Revocação: 1.0  
F1-score: 0.6666666666666666  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/c34bfd40-1966-4231-9006-ecefe4f5088a)

### Dermatology

Linearmente separável.  
Precisão: 1.0  
Revocação: 1.0  
F1-score: 1.0  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/ac63f78f-f5c6-4a74-8f99-d7bef06ba6fe)

### Synthetic-3

Linearmente separável.  
Precisão: 0.9782608695652174  
Revocação: 0.9782608695652174  
F1-score: 0.9782608695652174  

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/4266e6c3-2ad2-4e25-867a-44cd31b47fd4)

### Twonorm

Não é linearmente separável.

![image](https://github.com/mateuskrause/alg2-tp1/assets/47651648/cea6b3b0-b171-443a-9ee9-b2caf20a3260)
