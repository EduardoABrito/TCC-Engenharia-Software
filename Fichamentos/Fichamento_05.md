# An initial investigation of ChatGPT unit test generation capability

Guilherme, Vitor; Vincenzi, Auri. "An initial investigation of ChatGPT unit test generation capability." In Proceedings of the 8th Brazilian Symposium on Systematic and Automated Software Testing (SAST '23), pp. 15–24, Campo Grande, MS, Brazil, 2023. doi: [10.1145/3624032.3624035](https://doi.org/10.1145/3624032.3624035)

## 1. Fichamento de Conteúdo

O artigo apresenta uma investigação inicial da capacidade do ChatGPT na geração de testes de unidade de forma totalmente automatizada. A pesquisa se insere no contexto de que, embora existam ferramentas para geração de testes automáticos, a maioria não aproveita os avanços recentes em Modelos de Linguagem Grandes (_LLMs_). O trabalho propõe avaliar a qualidade dos testes gerados por um _LLM_ da OpenAI, o _gpt-3.5-turbo_, sem qualquer intervenção humana. Para isso, os pesquisadores selecionaram 33 programas Java que haviam sido utilizados em estudos anteriores, o que permitiu uma comparação direta com ferramentas tradicionais. Foram gerados 33 conjuntos de testes para cada programa, variando os parâmetros da API da OpenAI, como a _temperature_. A qualidade dos testes foi avaliada usando métricas rigorosas como cobertura de código (_code coverage_), pontuação de mutação (_mutation score_) e taxa de sucesso de execução. Os resultados foram bastante promissores, mostrando que os testes gerados pelo _LLM_ tiveram um desempenho comparável ao das ferramentas automatizadas tradicionais em todas as métricas avaliadas. A ausência de intervenção humana no processo de geração e correção dos testes torna o achado ainda mais significativo. O estudo conclui que os _LLMs_ têm grande potencial para a geração de testes de unidade, com um desempenho que já rivaliza com o de ferramentas estabelecidas no campo. Além disso, a pesquisa contribui com um conjunto de dados para que futuras comparações sejam realizadas.

## 2. Fichamento Bibliográfico

* Testes de Unidade (_Unit Testing_): Uma prática essencial no desenvolvimento de software para garantir a correção e a robustez de unidades de código individuais. (página 1)
* Cobertura de Código (_Code Coverage_): Uma métrica usada para quantificar até que ponto os testes exercitam diferentes partes do código-fonte, indicando a exaustividade da suíte de testes. (página 1)
* Pontuação de Mutação (_Mutation Score_): Uma métrica que avalia a eficácia de um conjunto de testes na detecção de falhas. É calculada medindo a capacidade dos testes de "matar" versões modificadas do código-fonte. (página 1)
* Parâmetro _Temperature_: Um recurso da API da OpenAI que controla a aleatoriedade e a criatividade das respostas geradas. Valores mais altos resultam em saídas mais variadas e imaginativas. (página 4)

## 3. Fichamento de Citações

* _"The use of automated testing generation is pursued to reduce the consequences of overlooked test cases in a software project."_ 
* _"Our findings revealed that the OpenAI LLM test set demonstrated similar performance across all evaluated aspects compared to traditional automated Java test generation tools used in the previous research."_ 
* _"The PITest tool generates all its mutants for the program under testing and executes each test set against its set of mutants, producing a comprehensive report that includes the mutation score and code coverage for each test set."_
* _"We intend to investigate the ChatGPT test generation capability fully automated, without human intervention, interacting, or correcting test cases, considering a possible scenario of no-touch testing."_ 
* _"It is a feature that allows users to control the level of randomness and creativity in the generated text."_
* _"By assessing the effectiveness and performance of the LLMs against established tools, we can gain valuable insights into their capabilities and potential advantages in generating high-quality unit tests for Java programs."_