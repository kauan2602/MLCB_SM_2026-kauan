Resultados Aula 05
 Exercício 1 — Esteira de Limpeza Avançada e Lemmatization
 Frase original

Gostaria de saber se vocês estão DEVOLVENDO os valores das mesas compradas!!!
Resultado

gostar saber devolver valor meso comprada

O texto foi convertido para letras minúsculas, teve caracteres especiais e pontuação removidos, as stop words foram filtradas e foi aplicada a lemmatization utilizando o SpaCy.


Exercício 2 — Sentence Embeddings com Mean Pooling

Foi utilizado o modelo glove-wiki-gigaword-50 para transformar as mensagens em vetores densos.
 Resultado

Formato da Matriz de Vetores Densos (Exemplos, Dimensões): (32, 50)

Isso significa que as 32 mensagens do dataset foram transformadas em vetores com 50 dimensões cada.

Exercício 3 — Regressão Logística e Fallback

Teste 1

Frase: "Quero saber o valor do frete do sofá"

Resultado: FALLBACK_HUMANO

Confiança: 35,52%

Como a confiança ficou abaixo do limiar de 50%, a mensagem foi encaminhada para o fallback humano.

Teste 2

Frase: "Gostaria de ver receitas de bolo de cenoura"

Resultado: vendas_orcamento

Confiança: 69,10%

Nesse caso, o modelo classificou a frase como 'vendas_orcamento', mesmo sendo uma mensagem fora do domínio de móveis. Isso demonstra uma limitação do modelo, pois ele precisa escolher uma das classes disponíveis.

 Exercício 4 — Comparativo entre Regressão Logística e KNN

 Resultados

Regressão Logística (Linear): 93,75%
KNN (Distância K=3): 56,25%

Reflexão

A Regressão Logística apresentou melhor desempenho na base utilizada, alcançando 93,75% de acurácia, enquanto o KNN com K=3 alcançou 56,25%. O KNN utiliza a distância entre os vetores para classificar as frases, podendo ser útil quando existem exemplos próximos no espaço vetorial. Porém, neste conjunto de dados, a Regressão Logística apresentou uma separação mais eficiente entre as classes.

---

## Conclusão

Os exercícios demonstraram etapas de pré-processamento de texto, lemmatization, representação vetorial por embeddings, classificação com Regressão Logística, uso de limiar de confiança para fallback e comparação com KNN.
