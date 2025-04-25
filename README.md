# Jantar_dos_Filosofos
Solução do problema do jantar dos filósofos, resolvido em c com round-robin
Esse trabalho foi desenvolvido para o curso de Ciencia da Computação-UFPB na cadeira de Sistemas Operacionais.

## Solução Nº1 - Solucao_Round-Robin 
Nesse solução, implementada em c, adotamos o metodo do Round-robin juntamente com um escalonador para evitar o deadlock. Apesar do funcionamento do código não ser o ideal já que, ele explica o modelo de maneira didática, mas na pratica não há uma competição real por recursos, pois as threads estão acessando linearmente o programa. Entretanto, através desse modelo é possivel visualizar de maneira didática o round-robin e o real problema do jantar dos filosofos, podendo ser muito útil na explicação para novas pessoas.

## Solução Nº2 - Solucao_otimizada
Essa é a solução "ideal" que simula perfeitamente o problema, corrigindo as deadlocks através do algoritmo de Dijkstra. Nela temos uma competição real por recursos e o escalonar media esse problema.
