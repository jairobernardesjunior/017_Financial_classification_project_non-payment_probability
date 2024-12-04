## Projeto non-payment probability

### Problem:
The total annual loans in Brazil is around R$ 5.3 trillion making this modality one of the most active in the financial sector. On this amount, the interest rate applies which represents the part of the profitability of the business. Thus, for success in this operation, it is necessary, logically, for the lender to receive faithfully the due interest and the borrowed amount. The certainty of receiving the profits and the loan amount must be ensured before the deal is closed.

O total de empréstimos anual no Brasil está em torno de R$ 5,3 trilhões tornando essa modalidade uma das mais ativas no setor financeiro. Sobre esse montante incide a taxa de juros que representa a parte da lucratividade do negócio. Assim para que se tenha sucesso nessa operação faz-se necessário, logicamente, para quem empresta, receber fielmente os juros devidos e o montante emprestado. A certeza de receber os lucros e o montante do empréstimo deve ser assegurado antes do negócio ser fechado.

### Motivation:
The need to know if a loan will be received properly in its entirety, with interest and adjustment, leads companies that lend money to seek ways to anticipate whether the borrower has the conditions and a profile capable of faithfully repaying the amount borrowed. For this, the company granting the loan needs to be aware of two fundamental issues for its security: to know the level of risk of the borrower and to know, according to the level of that risk, whether to lend the negotiated amount or not.

A necessidade de saber se um empréstimo será recebido devidamente em sua integralidade, com juros e correção, leva as empresas que trabalham emprestando dinheiro, procurar meios de antecipar se o tomador do empréstimo tem condições e um perfil capaz de pagar, com fidelidade, o valor tomado. Para isso a empresa que cede o empréstimo precisa estar a par de duas questões fundamentais para sua segurança: saber qual o nível do risco do tomador e saber, conforme o nível desse risco, se empresta ou não o valor negociado.

### Solution:
Through financial loan data from the company itself, we will conduct a thorough study and adjustment of this data. Various machine learning models, including deep learning, will be trained, defining and selecting the model that best generalizes in defining probabilities that reveal the level of risk in granting a specific loan to a particular person. This will enable and support the financial loan team in making the best decision regarding the security of that loan, reducing the events of default against the company.

Através de dados de empréstimos financeiros da própria empresa, faremos um estudo profundo e adequação desses dados. Será feito o treinamento de vários modelos de machine learning, como de deep learning, definindo e elegendo o modelo que melhor generaliza na definição de probabilidades que revelam o nível do risco de se fazer um determinado empréstimo para uma pessoa específica. Isso possibilitará e apoiará a equipe de empréstimos financeiros a tomar a melhor decisão com relação à segurança daquele empréstimo, reduzindo os eventos de inadimplência contra a empresa.

### Objective:
- The objective of this work is to train a classification model that can inform us of the probability of default occurring on a financial loan.

- O objetivo desse trabalho é treinar um modelo de classificação que possa nos informar qual a probabilidade de inadimplência ocorrer em um empréstimo financeiro.

### Data Origin:
- Dataset: https://www.kaggle.com/datasets/itssuru/loan-data

- publicly available data from LendingClub.com. Lending Club connects people who need money (borrowers) with people who have money (investors). Hopefully, as an investor you would want to invest in people who showed a profile of having a high probability of paying you back.

- Dados disponíveis publicamente do LendingClub.com. O Lending Club conecta pessoas que precisam de dinheiro (tomadores de empréstimo) com pessoas que têm dinheiro (investidores). Felizmente, como investidor, você gostaria de investir em pessoas que mostrassem um perfil de ter uma alta probabilidade de pagar você de volta.

- Aqui está o que as colunas representam:

credit.policy: 1 se o cliente atender aos critérios de subscrição de crédito do LendingClub.com e 0 caso contrário.

purpose: O propósito do empréstimo (assume os valores "credit_card", "debt_consolidation", "educational", "major_purchase", "small_business" e "all_other").

int.rate: A taxa de juros do empréstimo, como uma proporção (uma taxa de 11% seria armazenada como 0,11). Os mutuários considerados pelo LendingClub.com como mais arriscados recebem taxas de juros mais altas.

installment: As parcelas mensais devidas pelo mutuário se o empréstimo for financiado.

log.annual.inc: O logaritmo natural da renda anual autodeclarada do mutuário.

dti: A relação dívida/renda do mutuário (valor da dívida dividido pela renda anual).

fico: A pontuação de crédito FICO do mutuário.

days.with.cr.line: O número de dias em que o mutuário teve uma linha de crédito.

revol.bal: Saldo rotativo do mutuário (valor não pago no final do ciclo de cobrança do cartão de crédito).

revol.util: Taxa de utilização da linha rotativa do mutuário (o valor da linha de crédito usada em relação ao crédito total disponível).

inq.last.6mths: Número de consultas do mutuário por credores nos últimos 6 meses.

delinq.2yrs: Número de vezes que o mutuário atrasou um pagamento em mais de 30 dias nos últimos 2 anos.

pub.rec: Número de registros públicos depreciativos do mutuário (declarações de falência, penhoras fiscais ou julgamentos).

not.fully.paid: O empréstimo não foi totalmente pago.