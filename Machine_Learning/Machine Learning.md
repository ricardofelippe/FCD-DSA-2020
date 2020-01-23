# DSA-Machine Learning : Don't model the world. Model the Mind

 Definição 1: Machine learning ou Aprendizado de Máquina é um método de análise de dados que automatiza o desenvolvimento de modelos analíticos. Usando algoritmos que aprendem iterativamente a partir dos dados, o aprendizado de máquina permite que os computadores encontrem insights ocultos sem serem explicictamente programados para procurar algo específico.
 
 Definição 2: Inteligência artificial é um conjunto de teorias e de técnicas empregadas com a finalidade de desenvolver máquinas capazez de simular a inteligência humana.
 
 Definição 3: Algoritmos de aprendizagem de máquina aprendem a induzir uma função ou hipótese capaz de resolver um problema a partir de dados que representam instâncias(registros de dados do passado) do problema a ser resolvido.
 
 Definição 4: Aprendizagem Não-Supervisionada é o termo usado quando um programa pode automaticamente encontrar padões e relações em um conjunto de dados. Seu objetivo é organizar os dados de alguma forma ou descrever sua estrutura. Os algoritmos mais comuns são: K-Means, o Singular Value Decomposition(SVD) e o Principal Component Analysis(PCA).
 
 
 
 
 
 
 
 # MACHINE-LEARNING

:point_right:Algoritmos de aprendizado de máquinas podem ser representados pela seguinte combinação: Representação + Avaliação + Otimização.
- Representação: Os modelos preditivos devem ser representados de forma que possam ser interpretados pelo computador. Quando escolhemos uma representação, estamos também escolhendo premissas que limitam o que determinado modelo é capaz de aprender. Esse conjunto de possíveis modelos é conhecido como espaço de hipóteses. Esse espaço explica porque alguns modelos não são capazes de aprender determinadas regras.
- Avaliação: a função de avaliação é utilizada para avaliar modelos dentro de um espaço de hipóteses. Dessa forma, podemos escolher um bom modelo dentre todas as possibilidades.
- Otimização: Método que usará a função de avaliação na busca por boas hipóteses.
:star: Generalização => Principal objetivo na construção do modelo preditivo.
- Cost Function: O objetivo do algoritmo de ML é aprender um modelo que minimize os erros. A força motriz por tráz de otimização na aprendizagem de máquinas é a resposta de uma função interna do algoritmo, denominada Cost Function. É uma função de avaliação que mede quão bem um algoritmo  mapeia a função alvo a partir dos dados fornecidos. De outra forma, a Cost Function descreve quão bem a resposta na área de respostas se encaixa no conjunto de dados que está sendo analisado. A Cost Function é o que realmente impulsiona o sucesso de uma aplicação de aprendizado de máquinas. 

-Espaço de Hipóteses(área de respostas): contém os recursos com os quais podemos trabalhar. O algoritmo de Aprendizagem recebe os dados e navega pelo espaço de hipóteses a fim de encontrar a melhor hipótese que gera o resultado desejado. A combinação do espaço de hipóteses com algoritmo de aprendizagem resulta no Modelo de Aprendizagem.


DSA-MACHINE LEARNING

- NAIVE BAYES
  - Um dos algoritmos de ML mais usados
  - Utilizados com grande/médios conjunto de treinamento e os atributos que descrevem as instâncias são condicionalmente independentes(a informação de um evento não é informativa sob nenhum outro)
  - Utilizado em medicina em classificadores de textos.
  - Ao treinar o classificador, calcula-se uma distribuição geradora para cada classe. Na fase de classificação, calcula-se qual a distribuição tem a maior probabilidade de ter gerado, por exemplo, cada documento

- MÉTODOS ENSEMBLE
  - Aprendizado por agrupamento
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
    - Ganho de Informação: redução da Entropia
    - :exclamation: Nos algoritmos ID3, C4.5 e C5.0, o nó raiz é escolhido com base em quanto do total da Entropia é reduzido, se aquele nó é escolhido.**Isso é chamado de ganho de informação**
    - Ganho de Informação = Entropia do sistema antes da divisão - Entropia do sistema após a divisão.
    - Pruning: Poda da árvore
    - Como definir o tamanho correto da árvore: Usando um conjunto de validação.
    - Usar métodos probabilísticos.
    
 
 
 
 
 
 

