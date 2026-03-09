# RELATÓRIO DE IMPLEMENAÇÃO DE SERVIÇOS AWS

Data: 08/03/2026
Empresa: Accenture Dio farmaceuticas
Responsável: Rafaela Oliveira Marques

## Introdução
Este relatório apresenta a proposta de implementação de serviços da Amazon Web Services (AWS) para a Accenture DIO Farmacêutica. O foco principal é a otimização da infraestrutura tecnológica e a redução imediata de custos operacionais (OpEx) através do modelo de pagamento por uso e automação de processos.

## Descrição do Projeto
A estratégia de otimização foi dividida em três pilares fundamentais, visando armazenamento inteligente, computação sem servidor e aproveitamento de capacidade ociosa.

Etapa 1: Armazenamento Inteligente com Amazon S3
- Serviço: Amazon Simple Storage Service (S3).
- Aplicação: Armazenamento de dados de pesquisas, documentação regulatória (essencial no setor farmacêutico) e mídias.
- Otimização de Custo: Implementação de Políticas de Ciclo de Vida (Lifecycle Policies). Os dados que não são acessados frequentemente serão movidos automaticamente para classes de menor custo, como o S3 Glacier Instant Retrieval. Isso elimina gastos com hardware subutilizado e garante a durabilidade dos dados de longo prazo por uma fração do preço do armazenamento padrão.

Etapa 2: Processamento Eficiente com AWS Lambda
- Serviço: AWS Lambda (Serverless).
- Aplicação: Automação de tarefas de backend, processamento de relatórios e integração de sistemas de estoque.
- Otimização de Custo: Substituição de servidores ligados 24/7 por uma arquitetura Serverless. Com o Lambda, a empresa paga apenas pelos milissegundos de execução do código. Para tarefas agendadas e pontuais, isso reduz drasticamente o custo de manutenção de infraestrutura e elimina o tempo ocioso de instâncias EC2 ou servidores locais.

Etapa 3: Redução de Custos Computacionais com Instâncias Spot
- Serviço: Amazon EC2 Spot Instances.
- Aplicação: Ambientes de teste, pipelines de CI/CD e processamento de grandes lotes de dados (Batch Jobs) farmacêuticos.
- Otimização de Custo: Utilização da capacidade computacional excedente da AWS com até 90% de desconto em comparação aos preços de instâncias On-Demand. Como esses ambientes suportam interrupções, o uso de instâncias Spot é a escolha ideal para maximizar o poder de processamento sem comprometer o orçamento do projeto.



## Conclusão
A implementação destes serviços na Accenture DIO Farmacêutica resultará em uma infraestrutura mais ágil, escalável e economicamente sustentável. Espera-se uma redução significativa nos custos fixos de TI e um aumento na velocidade de entrega de novos serviços. Recomendamos a monitoração contínua via AWS Cost Explorer para identificar novas oportunidades de economia conforme a demanda crescer.

## Referências
https://aws.amazon.com/pt/s3/
https://aws.amazon.com/pt/lambda/
https://aws.amazon.com/pt/ec2/spot/


Assinatura do Responsável pelo Projeto: Rafaela Oliveira Marques
