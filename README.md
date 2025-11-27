<h1>Amostragem Aleatória com Python — Projeto com a Base Iris</h1>

Este projeto tem como objetivo demonstrar, de forma prática, como realizar uma amostragem aleatória utilizando Python. Para isso, utilizei a clássica base iris.csv, carregada diretamente com a biblioteca pandas, que facilita a leitura e manipulação de dados tabulares. Logo ao importar a base, é possível visualizar toda a estrutura do dataset e confirmar que ele contém 150 linhas distribuídas em 5 colunas.

Para garantir que os resultados da amostragem fossem reproduzíveis em várias execuções, defini uma semente aleatória com numpy.random.seed(). Em seguida, utilizei a função numpy.random.choice() para criar uma amostra binária composta por zeros e uns. Essa amostra funciona como uma máscara que separa o conjunto de dados original em dois subconjuntos distintos: um contendo as linhas marcadas como 0 e outro contendo as linhas marcadas como 1. A divisão foi feita com uma probabilidade de 70% para o valor 0 e 30% para o valor 1, criando dois grupos proporcionais e úteis para experimentos, testes ou validações.

Cada subconjunto final foi isolado com o uso de filtragens simples via loc, gerando duas bases independentes. A primeira é composta pelas linhas associadas ao valor 0 na amostra e a segunda pelas linhas associadas ao valor 1. Essa separação permite, por exemplo, dividir a base em conjuntos de treino e teste ou simplesmente explorar técnicas de amostragem dentro do ambiente Python.

