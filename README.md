# Jantar_dos_Filosofos
Solução do problema do jantar dos filósofos, resolvido em c.
Esse trabalho foi desenvolvido para o curso de Ciencia da Computação-UFPB na cadeira de Sistemas Operacionais. \
Fizemos duas soluções para simular o problema do jantar dos filosofos a solução com round-robin que não é comum, pois não reflete a essência principal do problema, que é a competição paralela de recursos, uma vez que a solução impede que duas threads diferentes tentem acessar recursos ao mesmo tempo, porem continua funcional. Enquanto, a solução dois é uma solução mais eficiente e reflete exateamente o problema do jantar dos filosofos. 

## Solução Nº1 - Solucao_Round-Robin 
Nesse solução, implementada em c, adotamos o metodo do Round-robin juntamente com um escalonador para evitar o deadlock e starvation. Apesar do funcionamento do código não ser o ideal já que, ele explica o modelo de maneira didática, mas na pratica não há uma competição real por recursos, pois as threads estão acessando linearmente o recurso. Entretanto, através desse modelo é possivel visualizar de maneira didática o round-robin e o real problema do jantar dos filosofos, podendo ser muito útil na explicação para novas pessoas.

Para rodar o programa:\
1- Você precisa ter o compilador GCC com suporte à PTHREAD ;\
2- Deve-se criar um arquivo.c e copiar o código nele ou baixar o codigo diretamente do github com .c; \
3- Deve ser compilado com o PTHREAD; Caso tenha baixado o arquivo do github, vá para o seu terminal linux e execute:\
gcc NomeDoArquivo.c -o NomeDoExecutavel -lpthread\
Ex: \
gcc Solucao_Round-Robin -o jantar -lpthread\
4- Agora execute o programa. Ex: ./jantar

## Solução Nº2 - Solucao_otimizada
Essa é a solução "ideal" que simula perfeitamente o problema, corrigindo as deadlocks e impedindo starvation. Nela temos uma competição real por recursos e o escalonador media esse problema.\

Para rodar o programa:\
1- Você precisa ter o compilador GCC com suporte à PTHREAD ;\
2- Deve-se criar um arquivo.c e copiar o código nele ou baixar o codigo diretamente do github com .c; \
3- Deve ser compilado com o PTHREAD; Caso tenha baixado o arquivo do github, vá para o seu terminal linux e execute:\
gcc NomeDoArquivo.c -o NomeDoExecutavel -lpthread\
Ex: \
gcc Solucao_otimizada -o jantar2 -lpthread\
4- Agora execute o programa. Ex: ./jantar2

## Interface visual
Também fizemoas uma interface gráfica, implementada com GTK. Vale frisar: essa interface tem o objeto de facilitar a visualização, **não faz parte da nossa solução principal**. Segue link com o vídeo mostrando o probblema e a implemntação associada a solução Nº1:
https://drive.google.com/file/d/1f1WEj0uQxeNqKgnN6uqZad9D__6Z5DWV/view?usp=sharing
