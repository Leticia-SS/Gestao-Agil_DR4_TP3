# Relatório Técnico: TP3 (RotaViva / Métricas, Fluxo e Iniciativa de IA)

## Visão geral

Este pacote reúne as respostas dos 10 exercícios do TP3, organizadas por número de exercício, em arquivos `.md` separados. O trabalho parte do cenário do RotaViva após dois meses de Scrumban, no TP2, e avança em duas frentes: métricas de fluxo e capacidade, nos Exercícios 1 a 6, e a iniciativa de previsão de rotas com IA, nos Exercícios 7 a 10. A base conceitual usada foi a literatura de métricas ágeis (cycle time, throughput, Lei de Little, CFD, burndown, velocity e eficiência de fluxo), o Guia Scrum 2020 e as práticas de gestão de produtos de IA, sem slides da disciplina disponíveis. Os gráficos foram entregues em Mermaid, com os dados usados para construí-los, e há uma memória de cálculo para os exercícios quantitativos.

## Organização dos arquivos

- `01-Ex.md`: dados hipotéticos de dez itens, cálculo de cycle time médio e throughput semanal, o que cada métrica revela e frase de abertura para a retrospectiva.
- `02-Ex.md`: burndown de Sprint de dez dias com oito itens, gráfico Mermaid, ponto de desvio e ação esperada no dia do desvio.
- `03-Ex.md`: histórico de velocity de seis Sprints, previsão com faixa de confiança e justificativa ao Product Owner.
- `04-Ex.md`: cumulative flow diagram em Mermaid, métricas de fila em "em revisão", diagnóstico e ficha para a retrospectiva.
- `05-Ex.md`: duas melhorias de fluxo sem contratação, mecanismo de cada uma e forma de medir o efeito.
- `06-Ex.md`: comparação de eficiência antes e depois, explicação de ocupação versus eficiência e conclusão.
- `07-Ex.md`: coordenação de cerimônias na iniciativa de IA, influência da estratégia e pauta ajustada de Sprint Review.
- `08-Ex.md`: métricas do modelo, recomendação de negócio e justificativa.
- `09-Ex.md`: por que o ciclo de treinamento não é tarefa comum, planejamento da Sprint e explicação ao comercial.
- `10-Ex.md`: papel do AI PM na retrospectiva, protocolo de Review e justificativa contra conversas paralelas.

## Decisões tomadas por exercício

**Exercício 1.** Construí dez itens com entradas e saídas distribuídas ao longo de quatro semanas, com cycle time variando de 3 a 8 dias, para gerar média de 6,1 dias. O throughput ficou em 2,5 itens por semana. A frase de abertura foi escrita sem jargão, com foco no que o time sente na prática.

**Exercício 2.** O burndown foi construído com linha ideal linear e linha real com dois desvios, um no início e um no meio da Sprint, para permitir a identificação de mais de um ponto de desvio, como o enunciado permite. O gráfico foi feito em Mermaid com os dados explícitos.

**Exercício 3.** O histórico de velocity foi construído com média de 19,5 e desvio pequeno, para dar uma previsão estável. A faixa de confiança foi calculada com os cenários pessimista, central e otimista, e a justificativa ao Product Owner foi escrita em linguagem de negócio.

**Exercício 4.** O CFD foi construído de forma que a coluna "em revisão" cresça de forma monotônica, enquanto "em desenvolvimento" fica estável, o que sustenta o diagnóstico de capacidade insuficiente de revisores. As métricas de fila foram calculadas com base nos dados do CFD.

**Exercício 5.** As duas melhorias propostas foram a redução do tamanho dos lotes e a revisão em par com rodízio, ambas sem contratação. Cada uma foi justificada pelo mecanismo de redução da fila, e a forma de medir foi definida com critério de sucesso e de falha.

**Exercício 6.** Os dados dos dois cenários foram construídos com o mesmo tempo ativo e tempos de espera diferentes, para isolar o efeito da melhoria. A eficiência subiu de 40 para 67 por cento, o que confirma o efeito esperado.

**Exercício 7.** A atuação do AI PM foi descrita como tradutor entre técnico e negócio, com um ajuste explícito em relação às cerimônias técnicas anteriores, que é a etapa de tradução de métricas para decisão de negócio. A pauta de Review foi ordenada do técnico para o negócio.

**Exercício 8.** As métricas escolhidas foram erro médio absoluto, confiabilidade dentro de margem e taxa de falha em cenários complexos, o que permite uma recomendação matizada. A recomendação foi a de piloto, e não de uso geral, justificada pelos números.

**Exercício 9.** A explicação do ciclo de treinamento foi feita pela diferença entre tarefa de esforço conhecido e ciclo de aprendizado com validação, e o planejamento da Sprint foi feito com frente separada e limite de WIP próprio, coerente com o TP2.

**Exercício 10.** A retrospectiva foi estruturada em três blocos, com conexão explícita entre os problemas dos dois grupos, e o protocolo de Review foi ordenado em cinco etapas, do técnico ao negócio, com decisão explícita ao final.

## Memória de cálculo dos exercícios quantitativos

**Exercício 1.** Cycle time médio: soma dos cycle times (3 + 4 + 6 + 5 + 6 + 7 + 7 + 8 + 7 + 8 = 61) dividida por 10, igual a 6,1 dias. Throughput semanal: 2 itens na semana 1, 3 na semana 2, 2 na semana 3 e 3 na semana 4, total de 10 itens em 4 semanas, igual a 2,5 itens por semana.

**Exercício 3.** Média de velocity: (18 + 20 + 17 + 22 + 21 + 19) dividido por 6, igual a 19,5. Previsão central: 120 dividido por 19,5, igual a aproximadamente 6,2 Sprints. Cenário pessimista: 120 dividido por 17, igual a aproximadamente 7,1 Sprints. Cenário otimista: 120 dividido por 22, igual a aproximadamente 5,5 Sprints.

**Exercício 4.** Tamanho da fila em "em revisão" no dia 10: 9 itens, contra 0 no dia 1. Tempo médio de espera nos últimos cinco itens: 4,2 dias, contra 1,3 dia nos dois primeiros.

**Exercício 6.** Eficiência antes: 2 dividido por 5, igual a 40 por cento. Eficiência depois: 2 dividido por 3, igual a aproximadamente 67 por cento.

## Observações de entrega

Os gráficos de burndown e de cumulative flow diagram foram entregues em Mermaid, com os dados usados para construí-los, o que atende ao requisito de representação textual estruturada equivalente. Não há trechos incompletos ou marcados como rascunho. O pacote foi organizado por exercício, em arquivos identificados pelo número e pelo tema.
