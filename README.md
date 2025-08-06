📊 Calculadora de Métricas de Avaliação para Modelos de Classificação
📖 Descrição
Este projeto consiste na implementação manual em Python das principais métricas de avaliação para modelos de classificação binária: Acurácia, Sensibilidade (Recall), Especificidade, Precisão e F1-Score. O objetivo é aprofundar o entendimento sobre o funcionamento de cada métrica a partir de valores de uma Matriz de Confusão definidos arbitrariamente.

Adicionalmente, o projeto inclui a visualização da Matriz de Confusão utilizando as bibliotecas Matplotlib e Seaborn para uma interpretação mais clara e intuitiva dos resultados.

🚀 Contexto
Este é um dos desafios de projeto propostos no Bootcamp Machine Learning Training, uma parceria entre a Digital Innovation One (DIO) e a BairesDev.

🛠️ Tecnologias Utilizadas
Linguagem: Python 3

Ambiente: Google Colab / Jupyter Notebook

Bibliotecas:

NumPy: Para a estruturação da matriz de confusão.

Matplotlib: Para a criação da base dos gráficos.

Seaborn: Para a visualização elegante da matriz de confusão (heatmap).

📂 Estrutura do Projeto
O projeto é inteiramente contido no notebook Jupyter:

calculo_metricas.ipynb: Notebook contendo todo o processo, desde a definição do cenário, implementação das funções, cálculo dos resultados e a análise final.

▶️ Como Executar
Clone este repositório para sua máquina local ou baixe o arquivo .ipynb.

Abra o notebook calculo_metricas.ipynb no Google Colab ou em um ambiente Jupyter local.

Execute as células de código em ordem sequencial.

📈 Resultados
Para o cenário de teste definido com os seguintes valores:

Verdadeiros Positivos (VP): 150

Verdadeiros Negativos (VN): 120

Falsos Positivos (FP): 80

Falsos Negativos (FN): 60

As métricas de avaliação calculadas foram:

Métrica

Resultado

Acurácia

0.659

Sensibilidade (Recall)

0.714

Especificidade

0.600

Precisão

0.652

F1-Score

0.682

Matriz de Confusão
A visualização da Matriz de Confusão para o cenário acima é a seguinte:

![Matriz de Confusão](nome_da_sua_imagem.png)

Nota: Para que a imagem apareça, tire um print do seu gráfico, salve o arquivo (ex: matriz_confusao.png) na mesma pasta do projeto no GitHub e certifique-se que o nome no código acima corresponde ao nome do seu arquivo.

🧠 Análise e Conclusão
A análise das métricas revela um desempenho moderado do modelo hipotético. A Acurácia de 65.9% indica que o modelo acerta mais do que erra, mas está longe de ser altamente confiável.

O ponto mais interessante é a relação entre Precisão (65.2%) e Sensibilidade (71.4%). A sensibilidade ser maior indica que o modelo tem uma capacidade relativamente melhor de identificar corretamente os casos positivos (encontrar os "spams", em nosso exemplo) do que de garantir que, quando ele classifica um caso como positivo, ele de fato seja (evitar "alarmes falsos").

O ponto mais fraco do modelo é a Especificidade (60.0%), mostrando uma dificuldade considerável em identificar corretamente os casos negativos. Em um cenário de filtro de spam, isso significaria que uma quantidade relevante de e-mails legítimos seria classificada incorretamente como spam (Falsos Positivos).

Conclusão: Baseado nesta análise, o modelo não seria recomendado para um ambiente de produção sem melhorias significativas. A baixa especificidade, em particular, geraria uma experiência negativa para o usuário. Próximos passos incluiriam a utilização de técnicas de otimização ou a escolha de um algoritmo mais robusto para tentar aumentar a capacidade do modelo de discernir entre as classes, especialmente os casos negativos.

✍️ Autor
Johnny Passos

📄 Licença
Este projeto está sob a licença MIT.
