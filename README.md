# 🤖Perceptron_Excel
  
## 📊Projeto de Perceptron em Excel  
Este projeto implementa um Perceptron utilizando o Excel, com foco em um processo de aprendizado supervisionado. Utilizamos um conjunto de dados gerados aleatoriamente, baseados no ID da universidade (RU), e ajustamos os pesos e bias até que o modelo fosse treinado.

## 🎯Objetivo do Projeto  
O objetivo é construir e treinar um Perceptron de múltiplas entradas usando o Excel, com cálculos manuais e automatizados de pesos, bias e função de ativação. O treinamento é concluído quando o erro de predição é minimizado após várias épocas de treinamento.

## 🛠️Passo a Passo da Implementação  
Seleção dos Dados de Entrada  
Os dados de entrada utilizados no treinamento são os sete números do RU (ID da universidade), que foram selecionados de forma aleatória.

Na planilha Seleção de Valores, foram gerados cinquenta amostras utilizando uma distribuição normal. Para isso, foram definidos:
Média e Desvio Padrão como parâmetros para gerar as amostras aleatórias.  
Essas amostras são usadas como entradas para o treinamento do  Perceptron.  
Atribuição de Pesos Iniciais  
Na planilha Treinamento, as cinquenta amostras geradas foram utilizadas para iniciar o processo de treinamento. Inicialmente, foram atribuídos pesos iguais a 1,000 para cada um dos sete dados de entrada.  

O objetivo nesta etapa é aplicar o cálculo do NETj e do delta para ajustarmos a taxa de aprendizado.
Cálculo do NETj e do Delta
O cálculo de NETj (a soma ponderada das entradas com os pesos) foi realizado da seguinte forma:

𝑁
𝐸
𝑇
𝑗
=
(
𝑋
1
×
𝑊
1
)
+
(
𝑋
2
×
𝑊
2
)
+
⋯
+
(
𝑋
7
×
𝑊
7
)
NETj=(X1×W1)+(X2×W2)+⋯+(X7×W7)
Para melhorar o treinamento, foi utilizada a fórmula de delta, que ajusta os pesos com base no erro observado entre a predição e o objetivo. Esse cálculo é crucial para corrigir os pesos e tornar o modelo mais preciso a cada época.

Ajuste do Bias    
Durante o processo de treinamento, ajustamos o bias, que inicialmente começou com um valor de 1,0. O bias foi ajustado gradualmente até 5,75, com o intuito de garantir que o perceptron atingisse a taxa de aprendizado ideal e melhorasse o desempenho nas predições.

Treinamento e Resultados  
A cada época, observamos os resultados de predição e objetivo, comparando-os para verificar o progresso do aprendizado.
O treinamento foi executado até atingir a época 199, quando a estrutura de entrada foi completamente treinada e os erros de predição foram zerados.

## 📁Como Usar o Arquivo  
Abra o arquivo Perceptron_Excel.xlsx.  
Na planilha Seleção de Valores, verifique os dados gerados aleatoriamente com base nos sete números do RU.  
Na planilha Treinamento, ajuste os pesos e o bias conforme necessário e observe como o Perceptron se comporta ao longo do treinamento.  
Na planilha Perceptron, realize testes com os dados de entrada:  
Se o valor de saída for 1, significa que o número de entrada é maior que o RU.  
Se o valor de saída for -1, significa que o dado de entrada é menor que o RU  
Acompanhe os cálculos de NETj, delta e bias para verificar os ajustes realizados a cada época.  
## 🤔Considerações Finais  
Este projeto exemplifica como um Perceptron pode ser implementado e treinado usando o Excel. Embora existam ferramentas mais avançadas para o desenvolvimento de redes neurais, o uso do Excel ajuda a visualizar e compreender os cálculos fundamentais por trás de modelos de aprendizado supervisionado.
