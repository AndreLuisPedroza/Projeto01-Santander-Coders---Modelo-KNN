# Projeto01-Santander-Coders---Modelo-KNN

  O algoritmo K-Vizinhos Mais Próximos (K-Nearest Neighbors) é uma abordagem de classificação que se baseia na proximidade dos vizinhos. É reconhecido como um dos modelos preditivos mais simples, pois não requer a formulação de uma hipótese matemática inicial. A essência desse método reside em identificar os 'k' vizinhos mais próximos do ponto a ser classificado e, com base nesses vizinhos, determinar sua classe predominante. Em outras palavras, o algoritmo busca os 'k' pontos mais próximos do ponto em questão e atribui a ele a classe mais frequente entre esses vizinhos.

- Problemática

Os dados abaixo são referentes ao cadastro de clientes de uma empresa de investimentos com suas respectivas carteira de investimentos, que indica se esse cliente tem o perfil de investidor Conservador, Moderado ou Agressivo. O nosso intuito é, a partir do investimento de alguns clientes que já tem um perfil definido, estimar esse perfil para aqueles que ainda não estão classificado, afim de oferecer novos produtos que sejam mais adequados a eles.

Os dados abaixo seguem o seguinte padrão:
[CPF: INT, Perfil Do Investidor: STRING, Carteira de Investimento: TUPLA]

- Regras
    1. Se você precisar de uma função para computar algo crie ela
    2. Não é permitido usar nenhum módulo externo como numpy e math
    3. Use apenas os objetos e fluxos visto até o momento no curso
    4. Se você tiver dificuldade de trabalhar com mais de 2 dimensões, pode utilizar apenas os dois primeiros valores de cada tupla
    5. O objetivo principal desse projeto não é encontrar o modelo de knn mais otimizado, mas sim você conseguir criar um modelo de KNN, independente se ele é o melhor ou não
    6. Não precisa se preocupar com a normalização das dimensões. É algo que vocês não viram

- Metodologia
  
Utilizou-se a *Distância Euclidiana* para determinar a distância entre os eventos. 
Para $N$ pontos, considere $P_i = (p_{i1}, p_{i2}, \dots, p_{in})$, para $i = 1, 2, \dots, N$. A distância euclidiana média entre todos os pontos é dada por:

\[
D = \frac{1}{{N(N-1)}} \sum_{i=1}^{N} \sum_{j=1, j \neq i}^{N} d(P_i, P_j)
\]

exemplo:

carteira1 : (x: 1, y: 1, z: 1)
carteira2 : (x: 2, y: 2, z: 1)
distância, é a raiz quadrada de: (2-1)2 + (2-1)2 + (1-1)2 em outras palavras: raiz quadrada de (1 + 1 + 0).

a distância entre esses dois pontos é de: 1.41
