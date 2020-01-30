# DSA-Machine Learning : Don't model the world. Model the Mind

 Definição 1: Machine learning ou Aprendizado de Máquina é um método de análise de dados que automatiza o desenvolvimento de modelos analíticos. Usando algoritmos que aprendem iterativamente a partir dos dados, o aprendizado de máquina permite que os computadores encontrem insights ocultos sem serem explicictamente programados para procurar algo específico.
 
 Definição 2: Inteligência artificial é um conjunto de teorias e de técnicas empregadas com a finalidade de desenvolver máquinas capazez de simular a inteligência humana.
 
 Definição 3: Algoritmos de aprendizagem de máquina aprendem a induzir uma função ou hipótese capaz de resolver um problema a partir de dados que representam instâncias(registros de dados do passado) do problema a ser resolvido.
 
 Definição 4: Aprendizagem Não-Supervisionada é o termo usado quando um programa pode automaticamente encontrar padões e relações em um conjunto de dados. Seu objetivo é organizar os dados de alguma forma ou descrever sua estrutura. Os algoritmos mais comuns são: K-Means, o Singular Value Decomposition(SVD) e o Principal Component Analysis(PCA).
 
 Definição 5: Modelos Descritivos: prospectam dados históricos buscando gerar conhecimento sobre a massa de dados.
 
 Definição 6: Modelo preditivo é uma função que, aplicada a uma massa de dados, consegue identificar padrões ocultos e prever o que poderá ocorrer.
 
 # Modelo preditivo
  - Identificar com a maior precisão possível o problema de negócio, quanto mais precisa a pergunta, mais precisa será a resposta e, portanto, maior o valor da resposta. 
  Definição 7: Modelo Preditivo é uma função matemática **aproximada**, encontrada através do treinamento com dados e que permite fazer previsões.
  - O objetivo do aprendizado de máquina é aprender a aproximação da função f que melhor representa a relação entre os atributos de entrada(chamadas variáveis preditoras) com a variáver target.
  
 
 # Como Funciona a Aprendizagem de Máquina
  - Conceito: Um componente chave do processo de aprendizagem é a generalização.
  - Se um algoritmo de Machine Learning não for capaz de generalizar uma função matemática que faça previsões sobre novos conjuntos de dados, ele não está aprendendo nada e sim memorizando os dados, o que é bem diferente.
  - Para poder generalizar a funçaõ que melhor resolve um problema, os algoritmos de Machine Learning se baseiam em 3 componentes:
    - Representação: O algoritmo de ML cria um modelo que apresenta um resultado para um determinado conjunto específico de inputs. A representação é um conjunto de modelos que o algoritmo pode aprender.
    - Avaliação: determina que modelo funciona melhor para criar o resultado esperado.
    - Otimização: busca entre os modelos criados, o que melhor gera o resultado esperado.
  
 # Elementos Essenciais do Processo de Aprendizagem
   - Um padrão existe
   - Não há um único modelo matemático que explique esse padrão
   - Dados estão disponíveis
   
 
  
 
 # Principais Métodos de Aprendizagem
  - Métodos Baseados em Instância
    - Considera a proximidade entre as instâncias na realização das previsões. O conceito por trás é que os dados tendem a estar concentrados em uma mesma região no espaço de entrada. Métodos de aprendizagem baseados em instâncias assumem que as instâncias podem ser representadas como pontos em um espaço Euclidiano. Ponto importante é que podemos usar outras medidas de distância tb, como distância de Manhattan, a qual aplica pesos diferenciados às diversas variáveis do conjunto de dados.
    - Os métodos de aprendizagem baseados em instâncias são métodos **não paramétricos**(podem ser usadas distribuições arbitrárias sem a suposição de que a forma das entidades sejam conhecidas)
    - :thumbsdown: Desvantagem: alto custo para classificação. Toda computação ocorre no momento da classificação.
    - :pushpin: ao contrário das outras abordagens, **não** ocorre a construção de um modelo de classificação explícito. 
    - :pushpin: teste pode ser intenso computacionamente pois requer comparação com todos os exemplos de treinamento
    - :star: KNN é o principal representante desta categoria
    
    
  - Métodos Probabilísticos:
   - Relevantes por dois motivos:
     - Fornecem algoritmos de aprendizagem práticos: Aprendizagem Naive Bayes/Aprendizagem de Redes Bayesianas/Combinam conhecimento a priori com os dados observados.
     - Fornecem uma estrutura conceitual útil: fornecem a "norma de ouro"(regra do menor erro possível) para avaliar outros algoritmos de aprendizagem.
     - :mega: Cada exemplo de treinamento pode decrementar ou incrementar a probabilidade de uma hipótese ser correta.
     - o classificador 
     
          
  - Métodos Baseados em Procura: Pode ser utilizado para a seleção de variáveis no modelo.
  - Métodos Baseados em Otimização:
    - Redes Neurais Artificiais
    - SVM(Support Vector Machines)
 
 
  
 # MACHINE-LEARNING
 
Um modelo de aprendizagem é composto de: Espaço de hipóteses + Algoritmo de Aprendizagem.  O espaço de hipóteses contém os recursos com os quais podemos trabalhar. O algoritmo de aprendizagem recebe os dados e navega pelo espalo de hipóteses a fim de encontrar a melhor hipótese que gera o resultado desejado. Por exemplo, podemos usar o SVM no espaço de hipóteses e back propagation no algoritmo de aprendizagem.

 
:point_right: Validação: técnica para avaliar a qualidade do modelo ainda na etapa de treinamento. O dataset usado é um subconjunto dos dados de treinamento.
 
:point_right:Algoritmos de aprendizado de máquinas podem ser representados pela seguinte combinação: Representação + Avaliação + Otimização.
- Representação: Os modelos preditivos devem ser representados de forma que possam ser interpretados pelo computador. Quando escolhemos uma representação, estamos também escolhendo premissas que limitam o que determinado modelo é capaz de aprender. Esse conjunto de possíveis modelos é conhecido como espaço de hipóteses. Esse espaço explica porque alguns modelos não são capazes de aprender determinadas regras.
- Avaliação: a função de avaliação é utilizada para avaliar modelos dentro de um espaço de hipóteses. Dessa forma, podemos escolher um bom modelo dentre todas as possibilidades.
- Otimização: Método que usará a função de avaliação na busca por boas hipóteses.
:star: Generalização => Principal objetivo na construção do modelo preditivo.
- Cost Function: O objetivo do algoritmo de ML é aprender um modelo que minimize os erros. A força motriz por tráz de otimização na aprendizagem de máquinas é a resposta de uma função interna do algoritmo, denominada Cost Function. É uma função de avaliação que mede quão bem um algoritmo  mapeia a função alvo a partir dos dados fornecidos. De outra forma, a Cost Function descreve quão bem a resposta na área de respostas se encaixa no conjunto de dados que está sendo analisado. A Cost Function é o que realmente impulsiona o sucesso de uma aplicação de aprendizado de máquinas. 

-Espaço de Hipóteses(área de respostas): contém os recursos com os quais podemos trabalhar. O algoritmo de Aprendizagem recebe os dados e navega pelo espaço de hipóteses a fim de encontrar a melhor hipótese que gera o resultado desejado. A combinação do espaço de hipóteses com algoritmo de aprendizagem resulta no Modelo de Aprendizagem.


DSA-MACHINE LEARNING
- Técnicas de Redução da Dimensionalidade
  - Missing Values Ratio: em geral, **50%** ou mais de valores missing indica que devemos eliminar a variável.
  - Random Forests/Ensemble Trees: aplica-se machine learning para a seleção das variáveis.
  - Low Variance Filter: Do cálculo da variância da coluna, posso eliminar as que apresentarem baixa variância.
  - Forward Feature Construction: inicia o treinamento com 01(um) atributo e vai agregando outros atributos(se necessário), avaliando os resultados até chegar no mix de variáveis com melhor performance. 
  - High Correlation Filter: Minimiza-se o problema de colinearidade.
  - Backward Feature Elimination:
  - PCA: :mega: Necessita ser alimentado com dados **normalizados**. Técnica que pode ser utilizada para a geração de índices e agrupamento de indivíduos. A PCA é associada a ideia de redução da massa de dados, com menor perda possível da informação.
  
  
Feature Engineering
- enriquecimento dos dados: inserir novas informações no dataset para representar informações que não estavam no dataset original.
- variável dummy: é a representação de uma variável categórica.Realiza-se a conversão de uma variável texto para uma correspondente numérica.  É uma variável fictícia.


KNN (K-Nearest Neighbours) -Me diga com quem andas, que te direi quem és-
  - Considera o voto majoritário entre os rótulos de classe dos k vizinhos mais próximos. O algoritmo utiliza medidas de distância a fim de comparar os pontos de dados. Por exemplo, se k=3, o KNN vai comparar o novo ponto de dado com os 3 vizinhos mais próximos em cada classe e então fazer a votação.
  - É preciso **normalizar(na mesma escala)** os dados antes de aplicar o algoritmo. Isso se deve ao fato de que as medidas de distância são sensíveis à escala dos dados. O principal propósito da medida de distância é identificar os dados que são mais similares e que não são similares. A escolha da medida de distância influencia diretamente a performance de modelos criados com o knn.
  - A precisão da classificação utilizando o algoritmo KNN depende fortemente do modelo de dados. Na maioria das vezes os atributos precisam ser normalizados para evitar que as medidas de distância sejam dominadas por um único atributo.
    
  - Distâncias usuais:
    - Distância Euclidiana: padrão. Usar com medidas numéricas. Trata todas as dimensões de forma igual, tendo com ponto negativo a sua sensibilidade à pontos extremos.
    - Distância de Hamming: Opção para trabalhar com dados **categóricos** . A função principal é verificar se dois atributos são iguais ou não. Quando iguais, a distância é zero. Caso contrário, a distância é 1(um).
  
- Aprendizagem Não Supervisionada-Clustering
  - A partir dos dados de entrada, mas sem um conhecimento prévio da saída gerada, é possível descobrir alguns padrões e criar um modelo que seja capaz de automaticamente agrupar os dados de acordo com as similaridades. É necessário uma boa dose de interpretação, necessitando conhecimento dos dados, do negócio e dos detalhes técnicos dos algoritmos. ** A busca dos padrões no KNN não é muito diferente do que é feito pelos humanos**
  - O principal objetivo da técnica de Clustering é encontrar grupos com máxima homogeneidade dentro do grupo e máxima heteregoneidade entre os grupos.
  - Como nem sequer sabemos o que estamos procurando, o clustering é usado para a **descoberta de conhecimento**, ao invés de fazer previsões.
  - A clusterização também é usada na mineração de dados, onde ocorre uma descoberta automática dos padrões.
  - Exemplo do uso de clusterização:
    - Segmentação de clientes em grupos com  demografia semelhante ou padrões de compra para campanhas de marketing direcionadas.
    - Simplificação de grandes conjuntos de dados agrupando características com valores semelhantes em um número menor de categorias homogêneas.
 - A distância não pode ser a melhor forma para encontrar similaridade entre os dados, tendo em vista que os valores dos atributos podem ser não escalares.
 - Os rótulos de classe obtidos de um classificador sem supervisão não possuem significado intrínseco.
 - **Aprendizagem semi-supervisionada**:Se começarmos com dados sem rótulo(sem variável target), podemos usar o clustering para criar rótulos de classe. A partir daí, podemos aplicar algoritmo supervisionado, como árvores de decisão para encontrar os preditores mais importantes dessas classes.
 - Clustering Hierárquico(agrupamento):
   - Mais comum
   - Tem hierarquia. Isso é feito iterativamente mesclando clusters menores em cluster maiores.
 - Clustering Particional:
   - Os clusters são gerados e avaliados usando um critério pré-definido específico, que inclusive é específico do domínio, ou seja, da área de negócio de onde os dados foram coletados. Uma vez que cada cluster formado é mutuamente exclusivo, nunca pode haver uma relação hierárquica entre os clusters. Não estamos preocupados com a hierarquia dos clusters,  mas sim com sua independência.
   
   -***A qualidade do agrupamento depende do algoritmo escolhido, da função de distância e da aplicação. Diz-se que a qualidade de um modelo de cluster é superior, quando a distância inter-cluster é maximizada e a distância intra-cluster é minimizada. ***
   
   
  - K-Means
    - Atribui cada um dos n exemplos de dados a um dos k clusters, onde k é um número que foi determinado previamente.
    - O algoritmo **atribui** exemplos a um conjunto inicial de k clusters.
    - **Atualiza** as atribuições ajustando os limites de cluster de acordo com os exemplos que estão no cluster.
    - Os centros são selecionados ao acaso dentro do conjunto de dados.
    - O algoritmo k-means é altamente sensível à posição inicial do centro dos clusters. Ou seja, a forma como é iniciado o treinamento tem um impacto substancial sob o conjunto final de clusters. Solução para este problema é modificar o algoritmo de tal forma a usar métodos diferentes para a escolha dos centros iniciais.
    - K-means++: método alternativo ao K-means, que propõe um método alternativo para a seleção dos centros de cluster iniciais. Propõe um método eficiente de se aproximar da solução de cluster otimizada.
    - Às vezes, o número de clusters é definido por requisitos de negócio ou a motivação para a análise. ***Na prática, o conhecimento do problema provavelmente ditará o caminho a ser seguido ***
    - Sem qualquer conhecimento prévio, uma regra geral sugere que k seja igual à raiz quadrada de (n/2), onde n é o número de exemplos no conjunto de dados. Na grande maioria das vezes, o tipo de problema e o conunto de dados já fornece uma noção do valor ideal de k.
    
    
    
    
    
    
   
 
 
  
  
   
  

- NAIVE BAYES
  - Um dos algoritmos de ML mais usados
  - Utilizados com grande/médios conjunto de treinamento e os atributos que descrevem as instâncias são condicionalmente independentes(a informação de um evento não é informativa sob nenhum outro)
  - Utilizado em medicina em classificadores de textos.
  - Ao treinar o classificador, calcula-se uma distribuição geradora para cada classe. Na fase de classificação, calcula-se qual a distribuição tem a maior probabilidade de ter gerado, por exemplo, cada documento

- MÉTODOS ENSEMBLE : Grupo de algoritmos de machine learning.
  - Aprendizado por agrupamento. Uni-se as saídas de diferentes modelos para encontrar a melhor resposta para o problema.
  - Os métodos ensemble selecionam uma coleção de hipóteses e combinam as suas previsões. Ex: geram-se 100 árvores de decisão diferentes que voltam na melhor classificação. 
  - Métodos ensemble consistem em vários modelos trabalhando em conjunto de forma que podemos escolher a melhor opção para nosso método preditivo.
  - Os classificadores ensemble predizem a classe de um registro elegendo a maioria dos votos feitas pelos classificadores base, como que procurando uma segunda, uma terceira opinião. Podemos inputar peso a cada opinião, combinando opiniões e esperando uma combinação mais bem informada de todas as disponíveis.
  - Os métodos ensemble tb são conhecidos como sistemas de classificação múltipla 
  - Métodos de implementação: 
     - Estatísticas Simples: esquema de votação- escolher a predição que mais se repetiu. Em problemas de regressão em que as saídas dos modelos é uma variável contínua, pode-se trabalhar com a média(simples ou ponderada), ou até a mediana
     - Ensemble Baseado em Modelos: Podemos treinar outro modelo supervisionado para escolher o melhor resultado entre os modelos primários 
     - Métodos ensemble permitem aumentar consideravelmente o nível de precisão nas previsões do modelo preditivo.
     - Métodos ensemble são equivalentes à combinaçaõ de preditores, combinação de modelos. É uma técnica de aprendizagem supervisionada para combinar vários modelos fracos afim de produzir um modelo forte.
     - :exclamation: Métodos ensemble funcionam melhor com modelos fracamente relacionados.
     - Algoritmos: Bootstrap Aggregating, boosting e voting.
     
  
- Redução de Dimensionalidade
  - PCA: Transforma ortogonalmente  as coordenadas originais de um conjunto de dados em um novo conjunto de coordenadas chamadas componentes principais. Como resultado, a primeira componente principal tem a maior variação possível. Cada componente subsequente tem a variância mais elevada possível sob a restrição que é ortogonal às componente anteriores. Manter apenas os primeiros componentes reduz a dimensionalidade dos dados, enquanto retém a maior parte da informação dos dados. :exclamation: A transformação PCA é sensível à escala relativa das variáveis originais. O intervalo de coluna de dados precisam ser **normalizados** antes de aplicar o PCA. As nova variáveis perdem interpretabilidade, logo, se a interprtação for importante, o PCA deixa de ser um método de redução de dimensionalidade.
  - PCA: Cada componente princial é uma combinação de atributos presentes no dataset. O primeiro componente principal é uma combinação linear dos atributos com máxima variância e determina a direção de maior variabilidade dos dados. Quanto maior a variabilidade capturada no primeiro componente principal, mais informação será capturada pelo componente.
  - PCA: Cada componente principal é uma combinação linear de todas a variáveis originais. São independentes entre si e estimados com propósito de reter em ordem de estimação o máximo de informação em termos da variação total contida nos dados. Os componentes principais são garantidamente independente, apenas se os dados forem normalmente distribuídos.
  -PCA: técnica que pode ser utilizada para geração de índices e agrupamento de indivíduos.
  -PCA: é associada à ideia de redução de massa de dados, com menor perda possível de informação.

- Decision Tree, Random Forest e Métodos Ensemble
  - Árvores de Desição
    - Defini-se um conjunto de regras e para cada regra há uma decisão que precisa ser tomada.
    - Podem ser usadas para problemas de Classificação e de Regressão.
    - Podem ser usadas para problemas de Classificação e de Regressão.
    - Considerações:
      - Qual atributo dever ser usado para iniciar a árvore?
      - Qua deve ser o atributo seguinte?
      - Quando parar de construir ramos na árvore(para evitar o overfitting) ?
    - Como definir o nó raiz e como realizar a divisão do conjunto de dados?
      - Estratégia Gulosa(Greedy Selection)
      - Divisão baseada em atributos nominais (divisão binária/divisão múltipla)
      - Divisão baseada em atributos contínuos
        - Decisão binária
        - Discretização(estática, dinâmica)
    - Entropia: medida da incerteza nos dados 
    - Ganho de Informação: indica quanto um determinado atributo sozinho consegue ajudar a classificar a base de dados. Redução da Entropia
    - :exclamation: Nos algoritmos ID3, C4.5 e C5.0, o nó raiz é escolhido com base em quanto do total da Entropia é reduzido, se aquele nó é escolhido.**Isso é chamado de ganho de informação**
    - Ganho de Informação = Entropia do sistema antes da divisão - Entropia do sistema após a divisão.
    - Pruning: Poda da árvore
    - Como definir o tamanho correto da árvore: Usando um conjunto de validação.
    - Usar métodos probabilísticos.
    
 
 
 
 
 
 

