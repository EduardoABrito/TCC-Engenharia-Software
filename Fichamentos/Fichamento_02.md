# A Comparative Evaluation on the Quality of Manual and Automatic Test Case Generation Techniques for Scientific Software - A Case Study of a Python Project for Material Science Workflows

D. Trübenbach, S. Müller and L. Grunske, "A Comparative Evaluation on the Quality of Manual and Automatic Test Case Generation Techniques for Scientific Software - a Case Study of a Python Project for Material Science Workflows," 2022 IEEE/ACM 15th International Workshop on Search-Based Software Testing (SBST), Pittsburgh, PA, USA, 2022, pp. 6-13, doi: [10.1145/3526072.3527523](https://doi.org/10.1145/3526072.3527523)


## 1. Fichamento de Conteúdo

O artigo investiga a eficácia de técnicas de geração automática de casos de teste (TCG) para _software_ científico, em comparação com a criação de testes de forma manual. O problema abordado é que, no campo das ciências naturais, os cientistas muitas vezes não possuem formação em engenharia de _software_, o que torna a criação de testes manuais uma tarefa cara e demorada. O estudo foca no projeto _Python Atomic Simulation Environment (ASE)_, usado em ciência de materiais computacional, e no pacote _exciting_. Os pesquisadores avaliaram quatro algoritmos de TCG (MIO, DynaMOSA, Whole Suite e FD-random) implementados na ferramenta Pynguin. A metodologia incluiu a criação de uma suíte de testes manual como "padrão-ouro" para comparação, e a execução dos algoritmos automáticos 50 vezes cada, com um tempo limite de 600 segundos. As métricas usadas para a avaliação foram a cobertura de _branch_ e a cobertura de mutação. Os resultados mostraram que, embora todas as abordagens automáticas tenham superado a suíte de testes original do projeto ASE, nenhuma delas se aproximou da cobertura alcançada pela suíte criada manualmente. A hipótese dos autores é que isso ocorre porque as ferramentas automáticas não foram projetadas para lidar com os tipos de entradas complexas e estruturadas exigidas pelo _software_ científico. Concluíram que mais trabalho é necessário na área para que a geração automática de testes seja eficaz nesse tipo de contexto.

## 2. Fichamento Bibliográfico

* Geração Automática de Casos de Teste (TCG): O TCG é visto como um problema de otimização onde métricas de cobertura (como linha, _branch_ ou mutação) são maximizadas dentro de um orçamento de tempo ou computação limitado (página 6).
* _Pynguin_: Uma ferramenta de protótipo que implementa abordagens de TCG de ponta para a linguagem de programação Python de tipagem dinâmica. Ele inclui algoritmos como Whole Test Suite Generation, DynaMOSA e MIO (página 6).
* _Atomic Simulation Environment (ASE)_: Um pacote de _software_ em Python usado em ciência de materiais computacional para simular propriedades físicas de estruturas moleculares. É o sistema sob teste utilizado no estudo (página 7).
* Cobertura de _Branch_: Uma das métricas de cobertura utilizadas para avaliar a eficácia dos algoritmos de TCG. A métrica mede a porcentagem de ramificações de código que foram executadas pelos testes (página 8).
* Cobertura de Mutação: A segunda métrica de cobertura utilizada na avaliação. Ela mede o quão sensível a suíte de testes é para detectar pequenas modificações (mutantes) no código (página 8).

## 3. Fichamento de Citações

* "Writing software tests is essential to ensure a high quality of the software project under test. However, writing tests manually is time consuming and expensive."
* "We find that while all evaluated approaches are able to improve upon the original test suite of ASE, none of the automated test case generation algorithms manage to come close to the coverages reached by the manually created test suite."
* "We hypothesize this may be due to the fact that none of the employed test case generation approaches were developed to work on complex structured inputs."
* "The goal of automatic test case generation (or TCG for short) is to generate a test suite without interacting with a user while still reaching high coverage metrics."
* "We can confirm that automatic TCG algorithms are able to improve upon the baseline test suite. We must, however, note that a manually created test suite reaches the maximum value possible for the branch coverage metric and gets close to the maximum in the mutation coverage."
* "Furthermore, the manually created test suite provides the developers with more feedback through meaningful naming schemes that the automatic TCG algorithms are not able to match." 