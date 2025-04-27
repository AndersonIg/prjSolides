Nesse projeto, trabalhei em um algoritmo genético convertendo o pkl para poder codar. 
Inicialmente, encontrei um problema com as cores, que não estavam no formato correto.  
A função cmap foi utilizada para convertê-las. O Matplotlib trabalha com cores por nome,  valores hexadecimais ou listas. 
A coluna Syndrome ID consiste em strings, que não são  cores válidas. Portanto, presumi que fossem identificadores para as síndromes e converti essa  coluna usando o 
LabelEncoder do scikit-learn.  
Os dados foram treinados com 320 características, mas eu estava tentando fazer previsões  com 1004 características. Como ele esperava receber os dados originais 
com as mesmas  características do treinamento, utilizei os índices dos vizinhos mais próximos encontrados na  matriz de distâncias para recuperar os rótulos 
correspondentes do treinamento (kneighbors).  

Ao final o gráfico dos 10 folds são gerados mostrando as taxas de verdadeiro positivo e falso positivo. 
Também criei testes automatizados para verificar algumas situações
