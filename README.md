# Questions_Python_Base_Salaries

![image](https://github.com/PenseJoyce/Questions_Python_Base_Salaries/assets/77034969/c26bb73d-bcff-4359-956d-1171c12ae967)


## Objetivos

O script tem os seguintes objetivos:

1- Responder ao questionário referente ao dataset 'salaries'.

2- Verificar a correlação entre duas variáveis


## Bibliotecas 

Estas foram as bibliotecas utilizadas

```
pip install pandas
pip install seaborn
pip install matplotlib
```

## Informações da base 

O dataset está disponível no seguinte endereço: https://api.slingacademy.com/v1/sample-data/files/salaries.csv

## Os atributos são:

1. Id
2. EmployeeName
3. JobTitle
4. BasePay
5. OvertimePay
6. OtherPay
7. Benefits
8. TotalPay
9. TotalPayBenefits
10. Year
11. Notes
12. Agency
13. Status

# Introdução 

## O que é correlação de variáveis? #

A análise de correlação é uma forma descritiva que mede se há e qual o grau de dependência entre variáveis, ou seja, o quanto uma variável interfere em outra, lembrando que essa relação de dependência pode ou não ser causal. Essa medida de grau de relação é medida através de coeficientes. No caso deste post, nós vamos focar no coeficiente de Pearson.

O coeficiente de Pearson, também chamado de “coeficiente de correlação produto-momento” ou chamado de “ρ de Pearson”, mede o grau de correlação através do cálculo de direção positiva ou negativa. Este coeficiente, normalmente representado por ρ assume apenas valores entre -1 e 1.

A análise de correlação vai retornar três possíveis cenários: (1) correlação positiva; (2) correlação negativa; e (3) não há correlação.

* Correlação positiva: quando duas variáveis que possuem correlação crescem ou decrescem juntas, ou seja, que possuem uma relação direta;
* Correlação negativa: quando duas variáveis que possuem correlação mas quando uma variável cresce a outra decresce, ou vice-versa;
* Não ter correlação: quando o crescimento ou decrescimento de uma variável não tem efeito sobre outra variável.

Como podemos interpretar os valores*  que ρ pode assumir?

ρ = 0,9 a 1 : correlação muito forte; 

ρ = 0,7 a 09 : correlação forte;

ρ = 0,5 a 0,7 : correlação moderada;

ρ = 0,3 a 0,5 : correlação fraca;

ρ = 0 a 0,3 : não possui correlação.

_* Valores positivos ou negativos_

Em python, para verificar a correlação usamos a biblioteca _seaborn_. Para a análise de correlação vamos utilizar a função .corr(). Para visualizarmos a matriz de correlação, vamos utilizar a função _.heatmap()_ do pacote seaborn, essa função vai nos retornar uma forma gráfica da matriz com uma escala de cor em conjunto com uma escala numérica, as quais vão indicar o grau medido entre as variáveis.

Neste dataframe, ao verificar a correlação entre Ano, Salario e Benefícios, verificou-se o seguinte:

![image](https://github.com/PenseJoyce/Questions_Python_Base_Salaries/assets/77034969/cdafee86-2ba7-480f-b371-97fb460c062c)

Ou seja, existe forte correlação entre Salário e benefícios, e não existe correlação entre ano e salário/benefícios.




