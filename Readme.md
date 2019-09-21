# Respostas

**a. Como foi a definição da sua estratégia de modelagem**

Inicialmente é importante explorar as variáveis tecnicamente, verificando se os dados foram carregados adequadamente e se estão no formato devido, na sequência vale entender as medidas descritivas de cada avariável para entender como cada uma delas se comporta. Uma análise bivariada ajuda a direcionar quais variáveis possuem mais relevância e por fim na parte de modelagem pode-se fazer a transformação de variáveis, engenharia de variáveis e finalmente a escolha do melhor modelo.

**b. Como foi definida a função de custo utilizada**

Considerando a qualidade como valor numérico poderíamos definir a função de custo pelo erro da predição em relação ao observado ou pela correlação do predito pelo observado, as duas medidas mais comuns são R² e o RMSE (Root Mean Squart Error - Raiz do Erro quadrático médio).
O RMSE é interessante para comparar um modelo em relação ao outro, mas é mais complicado de pensar nele por não ter uma escala específica. O R² por sua vez varia entre 0 e 1, de forma que valores mais próximos de 1 indicam maior qualidade do modelo, alguns podem colocar o ponto de corte de um modelo aceitável em 0,5, 0,6 ou mesmo em 0,7, mas na prática eu optaria pelo melhor modelo que me for possível.

**c. Qual foi o critério utilizado na seleção do modelo final**

O modelo final é escolhido pela melhor medida de qualidade, neste caso pelo maior R². 

**d. Qual foi o critério utilizado para validação do modelo Por que escolheu utilizar este método**

Uma forma de validar o modelo, para evitar coisas como overfiting, é verificar medida de qualidade num conjunto que não foi utilizado na modelagem, por isso separa-se em conjunto de treino e de validação.

**e. Quais evidências você possui de que seu modelo é suficientemente bom**

Utilizando o RMSE, quanto menor o erro melhor o modelo, em alguns aspectos a medida pode ser um pouco subjetiva, então enquanto RMSE estiver elevado (algo acima de 0,20) deveríamos buscar alternativas para melhorar o modelo, seja pela utilização de outras técnicas ou mesmo pela engenharia de variáveis.