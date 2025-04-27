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
  * Proteína, Carboidrato, Vegetal, Fruta, Laticínio, Gordura, Condimento ou Outro.
2. Organizar os dados em um arquivo .CSV em três colunas:
  * nome_receita, Ingredientes e tipos_ingredientes
3. Construir um grafo G, sendo:
  * Nós -> Ingredientes
  * Arestas -> Ingredientes que aparecem na mesma receita
  * Atributo dos nós -> Tipo do ingrediente
  * Cor do nó -> De acordo com o tipo do ingrediente
4. Analisar o coeficiente de assortatividade do tipo do ingrediente usando "networkx.attribute_assortativity_coefficient(G, 'tipo')"
## Análise da assortatividade

A assortatividade é uma medida de grafos que indicam o quanto os nós semelhantes tendem a se conectar entre si. No caso deste projeto, o quanto ingredientes do mesmo tipo se conectam. 
</br>
Para a análise quantitativa, temos as seguintes classificações:

* O valor é próximo de 1? → Homofilia: ingredientes do mesmo tipo tendem a estar juntos.
* O valor é próximo de 0? → Combinação aleatória.
* O valor é negativo? → Heterofilia: há preferência por ingredientes de tipos diferentes.
