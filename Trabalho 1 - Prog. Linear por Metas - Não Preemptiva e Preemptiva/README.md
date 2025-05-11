## Introdução

Este trabalho foi desenvolvido no âmbito da unidade curricular de Otimização Heurística e marcou o meu primeiro contacto com os métodos de otimização multiobjetivo, em particular com a Programação Linear por Metas — tanto na sua versão não preemptiva como preemptiva.

O objetivo principal foi aplicar estes métodos a um caso prático: apoiar a agência de publicidade Pubs na definição de um plano de publicidade televisiva para a empresa Cars, que se dedica à comercialização de automóveis. Este plano tinha de respeitar várias restrições e procurar atingir metas associadas a diferentes públicos-alvo.

Ao longo do trabalho, fui construindo e ajustando modelos matemáticos, aprendendo a interpretar os resultados obtidos e a tomar decisões com base neles. A parte prática foi feita com recurso ao Python e à biblioteca PuLP, o que também me permitiu consolidar competências na área da programação aplicada à otimização.

Mais do que chegar a uma única solução ideal, o desafio passou por explorar diferentes abordagens, perceber os seus efeitos e procurar soluções de compromisso entre os objetivos, aprendendo com o processo.



## Conclusão:

A realização deste trabalho permitiu-me aplicar pela primeira vez os conceitos de otimização multiobjetivo num problema realista.

Inicialmente, verifiquei a viabilidade das restrições hard propostas pela administração da Cars, tendo concluído que não existia uma solução que as satisfizesse todas em simultâneo.

A partir daí, relaxando as três restrições de audiência para os diferentes públicos-alvo – transformando-as em restrições soft – explorei vários resultados com recurso à Programação Linear por metas não preemptiva, criando variáveis de desvio e ajustando pesos para encontrar soluções de compromisso adequadas aos diferentes critérios.
Foram aplicadas duas metodologias principais na abordagem não preemptiva: a minimização da soma ponderada dos desvios percentuais e o objetivo MiniMax. Enquanto a primeira procura uma média ponderada entre as violações das metas, podendo aceitar desvios grandes em algumas desde que compensados por desvios pequenos noutras, o MiniMax foca-se em tornar o plano mais equilibrado, minimizando o pior desvio relativo — o que evita sacrificar demasiado uma meta em prol das outras. Esta diferença ajudou-me a perceber como a escolha da metodologia pode influenciar diretamente o tipo de compromisso alcançado.

Posteriormente a isso, realizei uma análise de dominância entre os quatro diferentes planos obtidos, com o objetivo de perceber se algum deles era claramente superior aos restantes. Essa análise permitiu concluir que, embora cada plano apresentasse vantagens em certas metas, nenhum dominava os outros em todas. Este resultado era esperado, pois os métodos utilizados têm precisamente como objetivo gerar soluções ótimas de Pareto, ou seja, soluções de compromisso onde não é possível melhorar uma meta sem piorar outra. Caso alguma solução tivesse dominado outra, isso indicaria um erro no processo de modelação e/ou na programação em Python.

Na última parte, com a programação por metas preemptiva, aprendi a lidar com prioridades rígidas, resolvendo o problema por níveis e garantindo que as metas mais importantes são respeitadas antes de considerar as restantes.

Assim, posso concluir que este trabalho ajudou-me a consolidar os conhecimentos transmitidos em aula, sobre modelação matemática, ao aplicar a formulação de problemas de otimização linear e a utilização de ferramentas computacionais para a sua resolução.
