# MALTA
Código-fonte da Tese de Doutorado da PUC Minas
A ausência de dados é um problema comum na área de Aprendizado de Máquina, podendo levar a estimativas tendenciosas de parâmetros, perda de informação e diminuição do poder estatístico. Existem diversas atividades aplicadas no tratamento de dados ausentes, mas a identificação do mecanismo causador da omissão e a imputação de valores podem ser desafios para os pesquisadores. Neste contexto, este trabalho propõe um método chamado MALTA (Método para Análise e Tratamento de Dados Ausentes) para análise e tratamento de dados ausentes, com o objetivo de auxiliar na identificação do mecanismo de ausência e na imputação de valores ausentes. MALTA permite desde a visualização dos dados ausentes, a geração artificial de ausências nos três mecanismos (\textit{Missing Completely at Random} (MCAR), \textit{Missing at Random} (MAR) e \textit{Missing Not at Random} (MNAR), a identificação do mecanismo (testes de Little, Dixon, Homocedasticidade e \textit{Regression-Based}), a imputação de dados ausentes (métodos média, \textit{k - Nearest Neighbor} (KNN), \textit{MissForest}, múltipla, clusterização \textit{K-Means}, regressão, Redes Generativas Adversárias) e Cópula Gaussiana), a predição por meio de classificadores (Árvore de Decisão, \textit{Random Forest}, \textit{Multilayer Perceptron} e \textit{Support Vector Machine}) e a avaliação da imputação utilizando-se as métricas de avaliação (\textit{Root Mean Square Error}, precisão, sensibilidade e \textit{F1 Score}). O MALTA foi validado a partir de experimentos realizados em uma base de dados privada com altas taxas de ausência produzida por meio da pesquisa intitulada \textit{Survey of Inmates in State and Federal Correctional Facilities} (SISFCF), nos Estados Unidos da América, que fornece em nível nacional dados representativos sobre prisioneiros de instalações estaduais e federais. Além disso, foram utilizados 46 conjuntos da dados públicos fornecidas pelo \textit{UCI Machine Learning} com ausências geradas sob os três mecanismos existentes. Os experimentos indicaram que o teste de Little é altamente eficaz na identificação do mecanismo de ausência MCAR, com 92\% de acurácia, seguido pelo método \textit{Regression-Based} com 76\%. Os métodos de imputação múltipla e KNN obtiveram os melhores resultados. Assim, foi definido um protocolo de tratamento de dados ausentes com base nos métodos mais eficazes. É importante lembrar que a escolha do método de tratamento adequado depende das características da base de dados e do mecanismo de ausência presente, e que a avaliação da qualidade dos resultados por parte do especialista é essencial para garantir que a imputação não introduza vieses ou distorções nos resultados da análise. A implementação do MALTA está disponível em https://github.com/fmartinssp/MALTA.