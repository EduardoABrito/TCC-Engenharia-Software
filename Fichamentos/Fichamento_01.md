# Can ChatGPT Repair Non-Order-Dependent Flaky Tests?

CHEN, Yang; JABBARVAND, Reyhaneh. "Can ChatGPT Repair Non-Order-Dependent Flaky Tests?." In: "Proceedings of the 1st International Workshop on Flaky Tests." 2024. p. 22-29.[10.1145/3643656.3643900](https://doi.org/10.1145/3643656.3643900)

## 1. Fichamento de Conteúdo

O artigo trata do problema dos _tests flaky_, que são testes de software que podem passar ou falhar de forma não determinística, e foca nos que são não dependentes da ordem de execução (_NOD_). Esse tipo de teste é particularmente desafiador de consertar, pois suas causas podem variar muito, como problemas de concorrência, dependências do ambiente ou até mesmo condições de tempo. O estudo investiga o potencial de modelos de linguagem grandes (*LLMs*), como o ChatGPT, para resolver essa questão. Para isso, os autores propõem uma técnica chamada _NODOCTOR_, que usa o GPT-4 em um processo iterativo para gerar e validar correções de código. A técnica foi avaliada em 118 testes _NOD_ de 11 projetos reais em Java. A pesquisa concluiu que, apesar do GPT-4 ser um dos *LLMs* mais avançados, ele foi ineficaz para o reparo desses testes, especialmente na identificação das causas raiz das falhas. Apenas 2 dos 118 testes foram corrigidos com sucesso, e a ferramenta gerou 6 falsos positivos. Os resultados sugerem que o modelo tem dificuldade em identificar a causa raiz das falhas em testes _NOD_ e, embora o experimento não tenha sido um sucesso, a pesquisa oferece informações cruciais para futuras direções nessa área de pesquisa, ressaltando os desafios que ainda precisam ser superados.

## 2. Fichamento Bibliográfico

* _Tests Flaky_: São testes de software que apresentam resultados imprevisíveis, podendo passar ou falhar mesmo quando o código não muda. Isso pode confundir os desenvolvedores e fazer com que percam tempo resolvendo problemas que não existem (página 1).
* Testes Não Dependentes de Ordem (_NOD_): Uma categoria de testes _flaky_ que não é afetada pela sequência de execução. A falha pode ocorrer por diversas razões, como questões de concorrência, dependências de ambiente de execução, entre outras (página 1).
* _NODOCTOR_: Uma técnica proposta no artigo para reparar testes _NOD_, que utiliza o GPT-4 para criar e validar _patches_ (correções) de código em um processo iterativo (página 2).
* Falsos Positivos: Correções de código geradas pela ferramenta que fazem o teste passar na etapa de validação, mas na verdade não consertam a falha original. Ocorre quando a lógica do teste ou suas asserções são alteradas para enganar o sistema de validação (página 5).

## 3. Fichamento de Citações

* _"Flaky tests, which can non-deterministically pass or fail on the same code version, may mislead developers' concerns, resulting in missing some bugs or spending time pinpointing bugs that do not exist."_
* _"Our comprehensive study on 118 from the IDOFT dataset shows that ChatGPT, despite as a leading LLM with notable success in multiple code generation tasks, is ineffective in repairing NOD test flakiness, even by following the best practices for prompt crafting."_
* _"More importantly, unlike OD flaky tests-caused by polluted shared status between tests-and ID flaky tests-caused by specific API implementations, the root causes of NOD tests are various, such as concurrency issues, platform de- pendencies, runtime environments, and more."_
* _"The process of iteratively repairing a flaky test is repeated up to five times."_
* _"In some cases, although the generated patch enables the test to pass during the validation process, manual inspection reveals that the corresponding code changes do not effectively address the NOD flakiness."_
* _"We believe that our findings offer valuable insights for future research directions in this domain."_