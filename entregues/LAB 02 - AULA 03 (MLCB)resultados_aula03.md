--- RESULTADOS DO LAB 02 (AULA 03) ---

--- Relatório de Classificação ---
                     precision    recall  f1-score   support

horario_atendimento       0.50      1.00      0.67         1
        localizacao       0.00      0.00      0.00         1
    troca_devolucao       0.00      0.00      0.00         1

           accuracy                           0.33         3
          macro avg       0.17      0.33      0.22         3
       weighted avg       0.17      0.33      0.22         3

--- Matriz de Confusão ---
[[1 0 0]
 [1 0 0]
 [0 1 0]]

 # Resultados — Aula 03

* **Acurácia:** 0,33 (33%), ou seja, o modelo acertou 1 das 3 previsões.
* **Precision:** foi 0,50 para `horario_atendimento` e 0,00 para as outras classes.
* **Recall:** `horario_atendimento` teve 1,00, enquanto `localizacao` e `troca_devolucao` tiveram 0,00.
* **F1-Score:** `horario_atendimento` = 0,67; `localizacao` = 0,00; `troca_devolucao` = 0,00.
* **Matriz de Confusão:** apenas uma previsão foi correta. As outras duas mensagens foram classificadas incorretamente.
* **Conclusão:** o modelo apresentou baixo desempenho, com apenas **33% de acurácia**, conseguindo identificar corretamente somente uma das três mensagens do conjunto de teste.
