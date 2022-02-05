# Predict-Churn
![image](https://user-images.githubusercontent.com/94385953/152658476-6bc27f0c-1b13-4ea2-a130-d96205f93ee8.png)
<br> 

**AVISO:** O problema de negócio citado aqui é para fins de resolução de Problemas o CEO e o time de Negócios não existem

## 1. Problema de Negócio 
O CEO pediu para prevermos quantos clientes irá deixar a empresa, vamos ter que prever e tomar alguma decisão para fazer esses clientes continuar na Empresa. Precisamos construir um plano de ação forte o bastante para mantermos esse cliente dentro da nossa companhia! 

## 2. Objetivo da Análise
Prever e fazer planos de ações para clientes não saírem da empresa.

## 3. Planejamento da Solução 

![image](https://user-images.githubusercontent.com/94385953/152658713-18840091-2fb4-4ce2-a451-a1d19cc7c7e7.png)

Durante o nosso planejamento separamos uma análise descritiva para termos noção dos nossos dados. Vimos que os dados de pontuação para crédito são homogêneos, tem uma concentração para valores maiores. Idade tem uma concentração para idade mais alta. Estimativa de salários tendia a valores mais baixos (skew negtivo). 
<br> 
Isso nos da um norte dos dados que temos em mãos podemos analisar que um ponto crucial durante a nossa análise exploratória será a idade do consumidor, como também, a idade, o credit_score, e o seu salário. 

## 4. Criação da Hipótese e Mapa Mental
![image](https://user-images.githubusercontent.com/94385953/152658810-09ee3b7c-dfa5-40e4-9d13-254ccf288327.png)

Criamos um mapa mental que exemplifica algumas das hipóteses possíveis para  resolução desse problema. Fizemos um brainstorming para conseguimos desenhar de onde se originariam cada uma das hipóteses. 

Abaixo temos a hipóteses relevantes para a solução do problema 

* **H4.** Homens com salários mais altos tem mais churn: **VERDADEIRO** 
![image](https://user-images.githubusercontent.com/94385953/152658878-4846019d-a2f3-483b-8c6c-22fa33fd496e.png)
<br>
Homens com salários mais altos tem mais churn e com isso desistem mais do que homens com salários médios e baixos.

* **H5.** Clientes ativos ganham salários mais altos que a sua maioria: **VERDADEIRO**
![image](https://user-images.githubusercontent.com/94385953/152658911-94327a80-a3f8-49e6-909b-b5531f5ed4bf.png)

Como eu posso observar clientes com salários mais alto tendem a ser mais do que os médios e baixos juntos. 

* **H7.** Pessoas em ativas compram mais Produtos do que as pessoas churn: **FALSO**
![image](https://user-images.githubusercontent.com/94385953/152658953-0355532f-e8cc-40ed-88e3-5a3714455832.png)
<br>
A empresa tem sérios problemas de fidelização de clientes que compram 4 produtos diferentes. Precisamos analisar os dados a fundo para entender o que isso significa - entender mais sobre a parte logística e ofertas do consumidor.

* **H10.** Pessoas com idade mais nova dificilmente entram em churn: **VERDADEEIRO**
![image](https://user-images.githubusercontent.com/94385953/152659012-84c3487e-a622-415d-8cac-f16489c54dca.png)
<br>
A maioria dos jovens continuam ativos, enquanto a procentagem de idosos em churn é a maior de todas.

## 5. Seleção das Variáveis 
![image](https://user-images.githubusercontent.com/94385953/152659096-71b70323-2dbd-4162-8052-ad6d35e619b9.png)
As variáveis escolhida para o modelo foram essas. 

## 6. Machine Learning Modelling
![image](https://user-images.githubusercontent.com/94385953/152659124-f2fb2526-34f5-4432-9b9e-ad1a0e55540b.png)
Durante essa análise de precisão optamos por escplher o XGBoost. 

## 7. Resultados

## 7.1 Análise de Resultados
![image](https://user-images.githubusercontent.com/94385953/152659161-329e367d-643b-41f5-ba7b-0dc14b4d6306.png)

* A taxa atual de churn do Banco é de 20.37%
* A taxa mensal varia de 4.29% em média 
* Com o nosso modelo de Machine Learning conseguiríamos recuperar pelo plano de ação 32% das perdas

## 7.2 Previsão com o Modelo no Churn 
![image](https://user-images.githubusercontent.com/94385953/152659193-ec8d74fd-664c-4896-bb13-402e0d0b1d8b.png)
<br> 
Utilizando esse modelo conseguiríamos recuperar 25% do churn do banco 

## 8. Plano de Ação 

* 1- Rever quando é oferecido mais de um produto, porque quando o cliente opta por isso o seu churn aumenta. O banco precisa rever unicamente como e quando estão sendo oferecido esses produtos
* 2 - Dar vantagens para os clientes que o modelo indicou que entrariam em churn. Exemplo - os clientes que o modelo indicou a probabilidade maior do que 50% para entrar em churn oferecer menos desconto na utilização de cartão, para clientes que tem probabiliadde 90% - entender com eles o motivo que vão levar ele para esse desligamento (podemos enviar uma pesquisa caso o cliente preencher ele ganha vantagens - exemplo: cashback)
* 3 - Focar algumas campanhas de marketing para o público idoso e focar em digital midia para o público mais jovem isso é interessante tendo em vista que os mais jovens dificilmente entram em churn comparado com os idosos. 

