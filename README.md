# 📊 Calculadora de Métricas de Avaliação para Modelos de Classificação

## 📖 Descrição
Este projeto consiste na implementação manual em Python das principais métricas de avaliação para modelos de classificação binária:

- **Acurácia**
- **Sensibilidade (Recall)**
- **Especificidade**
- **Precisão**
- **F1-Score**

Adicionalmente, o projeto inclui a visualização da Matriz de Confusão utilizando as bibliotecas Matplotlib e Seaborn para uma interpretação mais clara dos resultados.

---

## 🚀 Contexto
Este é um dos desafios de projeto propostos no Bootcamp Machine Learning Training, uma parceria entre a Digital Innovation One (DIO) e a BairesDev.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Ambiente:** Google Colab / Jupyter Notebook
- **Bibliotecas:**
  - NumPy: Estruturação da matriz de confusão
  - Matplotlib: Criação dos gráficos
  - Seaborn: Visualização elegante da matriz de confusão (heatmap)


## 📂 Estrutura do Projeto

O projeto está totalmente contido em um notebook Jupyter:

- `calculo_metricas.ipynb`: Notebook contendo todo o processo, desde a definição do cenário, implementação das funções, cálculo dos resultados e análise final.

---

## ▶️ Como Executar

1. Clone este repositório para sua máquina local ou baixe o arquivo `.ipynb`.
2. Abra o notebook `calculo_metricas.ipynb` no Google Colab ou em um ambiente Jupyter local.
3. Execute as células de código em ordem sequencial.

---

## 📈 Resultados

Para o cenário de teste definido com os seguintes valores:

- **Verdadeiros Positivos (VP):** 150
- **Verdadeiros Negativos (VN):** 120
- **Falsos Positivos (FP):** 80
- **Falsos Negativos (FN):** 60

As métricas de avaliação calculadas foram:

| Métrica               | Resultado |
|-----------------------|-----------|
| **Acurácia**          | 0.659     |
| **Sensibilidade**     | 0.714     |
| **Especificidade**    | 0.600     |
| **Precisão**          | 0.652     |
| **F1-Score**          | 0.682     |

---

### Matriz de Confusão

A visualização da Matriz de Confusão para o cenário acima é a seguinte:

 
<img width="653" height="553" alt="matriz_confusao" src="https://github.com/user-attachments/assets/a40c83ac-6e0b-4a21-b607-05350e72ad70" />

---

## 🧠 Análise e Conclusão

A análise das métricas revela um desempenho moderado do modelo hipotético. A acurácia de 65.9% indica que o modelo acerta mais do que erra, porém ainda distante de ser altamente confiável.

O ponto mais interessante é a relação entre precisão (65.2%) e sensibilidade (71.4%). A sensibilidade maior indica que o modelo tem uma capacidade relativamente melhor de identificar corretamente os casos positivos.

O ponto mais fraco do modelo é a especificidade (60.0%), mostrando uma dificuldade considerável em identificar corretamente os casos negativos. Em um cenário de filtro de spam, isso significaria que muitos e-mails legítimos poderiam ser classificados erroneamente como spam.

**Conclusão:** Baseado nesta análise, o modelo não seria recomendado para um ambiente de produção sem melhorias significativas. A baixa especificidade, em particular, poderia gerar uma experiência negativa para os usuários.

---

## ✍️ Autor

Johnny Passos

---

## 📄 Licença

Este projeto está sob a licença MIT.
