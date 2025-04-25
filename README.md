# Jantar_dos_Filosofos
Solução do problema do jantar dos filósofos, resolvido em c.
Esse trabalho foi desenvolvido para o curso de Ciencia da Computação-UFPB na cadeira de Sistemas Operacionais.

## Solução Nº1 - Solucao_Round-Robin 
Nesse solução, implementada em c, adotamos o metodo do Round-robin juntamente com um escalonador para evitar o deadlock e starvation. Apesar do funcionamento do código não ser o ideal já que, ele explica o modelo de maneira didática, mas na pratica não há uma competição real por recursos, pois as threads estão acessando linearmente o programa. Entretanto, através desse modelo é possivel visualizar de maneira didática o round-robin e o real problema do jantar dos filosofos, podendo ser muito útil na explicação para novas pessoas.

Para rodar o programa:
1- Você precisa ter o compilador GCC com suporte à PTHREAD ;
2- Deve-se criar um arquivo.c e copiar o código nele ou baixar o codigo diretamente do github com .c; 
3- Deve ser compilado com o PTHREAD; Caso tenha baixado o arquivo do github, vá para o seu terminal linux e execute:
gcc NomeDoArquivo.c -o NomeDoExecutavel -lpthread
Ex: 
gcc Solucao_Round-Robin -o jantar -lpthread
4- Agora execute o programa. Ex: ./jantar

## Solução Nº2 - Solucao_otimizada
Essa é a solução "ideal" que simula perfeitamente o problema, corrigindo as deadlocks e impedindo starvation. Nela temos uma competição real por recursos e o escalonar media esse problema.

Para rodar o programa:
1- Você precisa ter o compilador GCC com suporte à PTHREAD ;
2- Deve-se criar um arquivo.c e copiar o código nele ou baixar o codigo diretamente do github com .c; 
3- Deve ser compilado com o PTHREAD; Caso tenha baixado o arquivo do github, vá para o seu terminal linux e execute:
gcc NomeDoArquivo.c -o NomeDoExecutavel -lpthread
Ex: 
gcc Solucao_Round-Robin -o jantar -lpthread
4- Agora execute o programa. Ex: ./jantar
