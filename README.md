# Operadores-busca-ESDD

# Projeto de Busca Sequencial Indexada

O vídeo de apresentação do projeto esta disponivel em > https://youtu.be/HGi7fMAyk4I

Este projeto implementa uma busca sequencial indexada em C, uma técnica de pesquisa eficaz para vetores grandes e ordenados. A busca sequencial indexada otimiza a pesquisa dividindo o vetor em blocos de tamanho uniforme e criando um índice que armazena o primeiro elemento de cada bloco. Esse índice serve como uma espécie de guia, facilitando a localização do bloco onde o valor desejado pode estar. Com isso, ao invés de realizar uma busca sequencial por todo o vetor, basta navegar pelo índice para identificar o bloco correto e, em seguida, fazer uma busca sequencial somente dentro desse bloco, o que reduz o número total de comparações necessárias.

Para preparar o vetor para a busca sequencial indexada, é utilizada a ordenação com o algoritmo Merge Sort, que organiza os dados em ordem crescente, garantindo que o índice funcione corretamente. O Merge Sort, com sua complexidade de `O(n log n)`, é uma escolha eficiente e estável para lidar com grandes conjuntos de dados, além de assegurar que o vetor esteja totalmente ordenado antes de se criar o índice.

A execução do programa começa com a geração de um vetor ordenado de maneira crescente com valores aleatórios. Em seguida, o vetor é ordenado usando o Merge Sort, o que facilita a criação de um índice com base no tamanho do vetor e no número de blocos definidos. Após o índice ser criado, a busca sequencial indexada é aplicada para localizar um valor especificado no vetor. Quando o valor é encontrado, o programa retorna sua posição; caso contrário, informa que o elemento não está presente no vetor.

Durante a execução, o programa exibe o tempo de execução do Merge Sort, além da quantidade de comparações e trocas realizadas durante a ordenação. Essa exibição permite avaliar a eficiência do algoritmo e o impacto da busca sequencial indexada na otimização da pesquisa. Para compilar e executar o programa, basta usar os comandos `gcc main.c -o busca_indexada` para compilar e `./busca_indexada` para executar.

Esse projeto exemplifica de forma prática como a busca sequencial indexada pode reduzir o esforço necessário para localizar um elemento em um vetor grande e ordenado, destacando a vantagem de criar índices para agilizar a pesquisa. A implementação modular também permite que o projeto seja adaptado facilmente para diferentes tamanhos de vetor e blocos, ampliando a compreensão da técnica.

