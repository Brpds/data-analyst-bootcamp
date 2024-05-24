# Considerações

## Um breve parágrafo...

### Sempre fico com dúvidas quando parece simples (e às vezes é), principalmente porque depois de queimar muitas sinapses tentando entender como fazer os gráficos funcionarem, as transformações foram menos complicadas.

## O que eu entendi:

### Como não precisava realizar o dashboard propriamente dito (revisei os vídeos pra ter certeza, creio que não passei batido), as transformações são diretas.

## Integração do BI com o AzureSQL:

### bem direta e relativamente simples, graças ao guia da TechLead. Dificuldades apenas com Conta Corporativa / Estudantil


## Colaboradores:

### a junção de nomes foi feita na própria tabela dos employees, simplesmente usando uma coluna personalizada com a função
### = [Fname] & " " & [LName]

### a coluna Super_ssn indica o SSN de quem é o Gerente de quem. Logo, bastava fazer a consulta cruzando SSN com Super_ssn.

### o único dado nulo foi Super_ssn para James Borg, inferindo-se que, somado ao fato de trabalhar no Headquarters, ele é o Gerente Geral.
### usando a função do PowerBI substituir valor na coluna, trocou-se null por Gerente Geral.

## Departamentos:

### bem direto, apenas feito a consulta mesclada, combinando os Dnumber(número do departamento) nas tabelas retornando apenas o Dname (nome do departamento).

### Dentro do relatório, os resultados podem ser encontrados nas tabelas OverallTable e/ou GerenteXColaborador.


### P.S.: Continuo achando que deixei passar alguma instrução em que deveria fazer o Dash...Dúvida cruel. abraços!