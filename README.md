# Operadores-busca-ESDD

# Projeto de Busca Sequencial Indexada

O vídeo de apresentação do projeto esta disponivel em > https://youtu.be/HGi7fMAyk4I

Este projeto implementa uma busca sequencial indexada em C, uma técnica de pesquisa eficaz para vetores grandes e ordenados. A busca sequencial indexada otimiza a pesquisa dividindo o vetor em blocos de tamanho uniforme e criando um índice que armazena o primeiro elemento de cada bloco. Esse índice serve como uma espécie de guia, facilitando a localização do bloco onde o valor desejado pode estar. Com isso, ao invés de realizar uma busca sequencial por todo o vetor, basta navegar pelo índice para identificar o bloco correto e, em seguida, fazer uma busca sequencial somente dentro desse bloco, o que reduz o número total de comparações necessárias.

A busca indexada no código aplica a teoria de forma prática ao dividir o vetor em partes menores usando a tabela de índices, acelerando a localização do elemento procurado. Isso demonstra a eficiência da técnica em grandes conjuntos de dados ao reduzir o número de comparações necessárias. A execução do programa começa com a geração de um vetor ordenado de maneira crescente com valores aleatórios. Após o índice ser criado, a busca sequencial indexada é aplicada para localizar um valor especificado no vetor. Quando o valor é encontrado, o programa retorna sua posição; caso contrário, informa que o elemento não está presente no vetor.

Durante a execução, o programa exibe o tempo de execução do Merge Sort, além da quantidade de comparações e trocas realizadas durante a ordenação. Essa exibição permite avaliar a eficiência do algoritmo e o impacto da busca sequencial indexada na otimização da pesquisa. Para compilar e executar o programa, basta usar os comandos `gcc main.c -o busca_indexada` para compilar e `./busca_indexada` para executar.

Esse projeto exemplifica de forma prática como a busca sequencial indexada pode reduzir o esforço necessário para localizar um elemento em um vetor grande e ordenado, destacando a vantagem de criar índices para agilizar a pesquisa. A implementação modular também permite que o projeto seja adaptado facilmente para diferentes tamanhos de vetor e blocos, ampliando a compreensão da técnica.

