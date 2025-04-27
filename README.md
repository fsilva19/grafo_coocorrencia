# Análise de Assortatividade em Grafos de Ingredientes da Culinária Brasileira (U1T2)
---
Disciplina: Algoritmos e Estruturas de Dados II
</br>Discente: Felipe Gabriel B. da Silva

---
</br>
O presente projeto tem como objetivo analisar a assortatividade em um grafo de co-ocorrência de ingredientes em 50 receitas populares da culinária brasileira, bem como reforçar os conceitos sobre grafos aprendidos em sala de aula, utilizando a biblioteca NetworkX. 
</br>
Outras bibliotecas importantes que também são utilizadas no projeto:

*   Matplotlib
*   Google.colab
*   Collections
*   Pandas
</br>

## Requisitos
1. Utilizar algum modelo de linguagem para gerar, a partir de uma imagem da receita, a listagem dos ingredientes utilizados, bem como classificar o ingrediente em uma das categorias abaixo:
  - Proteína, Carboidrato, Vegetal, Fruta, Laticínio, Gordura, Condimento ou Outro.
2. Organizar os dados em um arquivo .CSV em três colunas:
  - nome_receita, Ingredientes e tipos_ingredientes
3. Construir um grafo G, sendo:
  - Nós -> Ingredientes
  - Arestas -> Ingredientes que aparecem na mesma receita
  - Atributo dos nós -> Tipo do ingrediente
  - Cor do nó -> De acordo com o tipo do ingrediente
4. Analisar o coeficiente de assortatividade do tipo do ingrediente usando "networkx.attribute_assortativity_coefficient(G, 'tipo')"
## Análise da assortatividade

A assortatividade é uma medida de grafos que indicam o quanto os nós semelhantes tendem a se conectar entre si. No caso deste projeto, o quanto ingredientes do mesmo tipo se conectam. 
</br>
Para a análise quantitativa, temos as seguintes classificações:

- O valor é próximo de 1? → Homofilia: ingredientes do mesmo tipo tendem a estar juntos.
- O valor é próximo de 0? → Combinação aleatória.
- O valor é negativo? → Heterofilia: há preferência por ingredientes de tipos diferentes.

## Resultados

Feito o código, foram geradas algumas informações importantes:
```
Número de nós (ingredientes): 133
Número de arestas (coocorrências): 1195
Coeficiente de assortatividdade: -0.022807771993952845
```
Imagem do grafo gerado:
</br>
![grafo](https://github.com/user-attachments/assets/b7ad1cde-9207-452f-bc92-9e36cd0acf7f)

## Discussão 
O coeficiente de assortatividade do grafo, considerando o atributo de tipo, é aproximadamente -0.02, indicando que as receitas não possuem um padrão na escolha dos ingredientes a partir do seu tipo. Embora o valor seja negativo, o que indicaria uma preferência por heterogeneidade, ele está bem próximo de zero, não tendo um efeito considerável. Em outras palavras, a culinária popular brasileira, analisada em uma amostra aleatória de 50 receitas, não demonstra um padrão claro na busca de juntar ingredientes do mesmo tipo, nem uma preferência por tipos diferentes.

</br>

_Link para o vídeo_ -> _httpsskmsk. smc_
