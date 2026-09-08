ATIVIDADE AVALIATIVA – ESTRUTURAS DE DADOS
PARTE 1 – PESQUISA: BUBBLE SORT E QUICK SORT
Bubble Sort
O Bubble Sort é um algoritmo de ordenação baseado na comparação entre elementos vizinhos. O algoritmo percorre o array várias vezes, comparando dois elementos consecutivos. Quando eles estão na ordem errada, são trocados.

A cada passagem, os maiores elementos vão sendo deslocados para o final do array, como se "flutuassem" para sua posição correta.

A lógica básica é:

Percorrer o array.
Comparar elementos vizinhos.
Trocar os elementos quando estiverem fora de ordem.
Repetir o processo até que o array esteja ordenado.
Sua complexidade é:

Melhor caso: O(n), quando o algoritmo possui uma verificação que detecta que não houve trocas e o array já está ordenado.
Caso médio: O(n²).
Pior caso: O(n²).
Memória auxiliar: O(1).
A principal vantagem é sua simplicidade de implementação e compreensão. A principal limitação é o grande número de operações para arrays grandes.

É adequado para pequenos conjuntos de dados e situações educacionais. Não é recomendado para grandes quantidades de elementos quando existem algoritmos mais eficientes.

Quick Sort
O Quick Sort utiliza a estratégia de divisão e conquista. Ele escolhe um elemento chamado pivô e reorganiza os elementos de maneira que os menores que o pivô fiquem de um lado e os maiores fiquem do outro.

Depois, o mesmo processo é aplicado recursivamente às duas partes do array.

A lógica básica é:

Escolher um pivô.
Particionar o array.
Colocar os elementos menores de um lado e os maiores do outro.
Aplicar o algoritmo recursivamente às duas partes.
Continuar até que todas as partes estejam ordenadas.
Sua complexidade é:

Melhor caso: O(n log n).
Caso médio: O(n log n).
Pior caso: O(n²).
Memória: normalmente O(log n) devido à recursão, podendo chegar a O(n) no pior caso.
Sua principal vantagem é apresentar excelente desempenho médio, principalmente em conjuntos grandes. Sua principal limitação é que uma escolha ruim do pivô pode levar ao pior caso O(n²).

É adequado para ordenar grandes conjuntos de dados. Não é a melhor escolha quando é necessário garantir desempenho O(n log n) no pior caso sem técnicas adicionais para escolha do pivô.

Tabela comparativa
Característica	Bubble Sort	Quick Sort
Princípio de funcionamento	Compara e troca elementos vizinhos	Divide o array utilizando um pivô
Melhor caso	O(n)	O(n log n)
Caso médio	O(n²)	O(n log n)
Pior caso	O(n²)	O(n²)
Uso de memória	O(1)	O(log n) em média
Vantagem principal	Simples de entender e implementar	Muito eficiente em arrays grandes
Limitação principal	Muitas operações em grandes arrays	Pode atingir O(n²) com pivô ruim
Aplicação recomendada	Arrays pequenos	Arrays médios e grandes
Aplicação não recomendada	Grandes conjuntos de dados	Quando é necessário garantir O(n lo
